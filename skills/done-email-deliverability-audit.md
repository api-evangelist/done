---
name: done-email-deliverability-audit
description: >-
  Audit a domain's email authentication and inbox branding with _done — bulk DMARC policy lookup
  plus BIMI/VMC verification. Two paid calls, $0.01 each.
api: _done
provider: https://underscoredone.com
operations:
  - handler_dmarc_lookup_post    # dmarc-lookup POST /dmarc-lookup
  - handler_check_post           # bimi-checker POST /check
source: openapi/_original/done-dmarc-lookup-openapi.json, openapi/_original/done-bimi-checker-openapi.json
generated: '2026-08-11'
method: generated
---

# Audit email deliverability with _done

## Steps

1. **DMARC first.** `POST https://dmarc-lookup.underscoredone.com/dmarc-lookup`
   (`handler_dmarc_lookup_post`) with `{"domains": ["onescales.com", "google.com"]}`. Bare domain
   names only — no `http://`, no paths. One call handles one or many domains.

2. **Read the policy, not just the presence.** A published record with `p=none` is monitoring,
   not enforcement. Escalation order is `none` → `quarantine` → `reject`.

3. **Then BIMI.** `POST https://bimi-checker.underscoredone.com/check` (`handler_check_post`) with
   `{"domains": ["example.com", "brand.co"], "selector": "default", "check_vmc": true}` — up to 10
   domains. `selector` is almost always `default`; only change it if the domain publishes a
   non-default BIMI selector. Set `check_vmc: false` for a faster check that skips certificate
   verification.

4. **Sequence matters.** BIMI only renders when DMARC is at enforcement, so a BIMI pass on a
   `p=none` domain is not a working inbox logo. Report step 1's policy alongside step 3's result.

## Rules

- Both calls are payment-gated — see `done-pay-a-402-call`. Two payments ($0.02) per audit,
  regardless of how many domains you batch.
- Both are read-only DNS lookups; safe to repeat, but each repeat is charged.
- `400` means the input failed validation (commonly a URL where a bare domain was required);
  `422` means a field is missing or the wrong type. Both return their reason in `detail`.
