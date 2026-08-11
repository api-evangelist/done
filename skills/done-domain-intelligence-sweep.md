---
name: done-domain-intelligence-sweep
description: >-
  Profile one or more domains end to end with _done — registration status, age and expiry, full
  DNS + WHOIS records, and the network operator behind the resolved address. Four paid calls,
  $0.01 each, no account.
api: _done
provider: https://underscoredone.com
operations:
  - check_check_post             # domain-availability-checker POST /check
  - handler_lookup_post          # domain-age-checker POST /lookup
  - handler_lookup_post          # dns-whois-lookup POST /lookup
  - handler_lookup_post          # asn-lookup POST /lookup
source: openapi/_original/done-{domain-availability-checker,domain-age-checker,dns-whois-lookup,asn-lookup}-openapi.json
generated: '2026-08-11'
method: generated
---

# Sweep a domain with _done

> `operationId`s collide across _done specs — `handler_lookup_post` is used by three different
> services. Always address an operation by **host + path**, never by operationId alone.

## Steps

1. **Is it registered?** `POST https://domain-availability-checker.underscoredone.com/check`
   (`check_check_post`) with `{"domains": ["example.com", "mybrand.ai"]}` — 1 to 10 plain domains,
   no scheme. Uses RDAP. An unregistered domain ends the sweep for that name.

2. **How old is it, and when does it lapse?**
   `POST https://domain-age-checker.underscoredone.com/lookup` (`handler_lookup_post`) with
   `{"domains": ["google.com", "openai.com", "github.com"]}`. Returns registration date,
   expiration date, age and time remaining.

3. **Everything DNS and WHOIS.** `POST https://dns-whois-lookup.underscoredone.com/lookup`
   (`handler_lookup_post`) with `{"domains": ["onescales.com", "hillms.com"]}` — up to 10 domains,
   all 13 DNS record types plus full WHOIS registration data in one call.

4. **Who runs the address?** Take an A/AAAA record from step 3 and
   `POST https://asn-lookup.underscoredone.com/lookup` (`handler_lookup_post`) with
   `{"query": "8.8.8.8"}`. Returns ASN, holder, country, RIR and the CIDR prefix. The same
   endpoint accepts an ASN directly (`AS15169` or `15169`) — it detects which you sent.

## Rules

- Every call is preceded by an HTTP 402 challenge — run `done-pay-a-402-call` first for each one.
  Budget four payments ($0.04) per domain sweep, plus one extra ASN call per distinct IP.
- Batch aggressively: steps 1–3 all take arrays, so ten domains cost the same as one.
- All four operations are **read-only**; a retry is safe for correctness, but each retry is a
  fresh charge because there is no idempotency key.
- On `422`, read `detail[].loc` to find the offending array element — the bulk operations report
  per-item validation errors.
