---
name: done-network-exposure-probe
description: >-
  Probe a host's externally reachable surface with _done — open TCP ports and their services,
  the CORS permissions an endpoint grants, and the security headers it returns. Three paid calls,
  $0.01 each.
api: _done
provider: https://underscoredone.com
operations:
  - scan_scan_post               # port-scanner POST /scan
  - handler_check_post           # cors-header-checker POST /check
  - handler_check_post           # http-header-checker POST /check
source: openapi/_original/done-{port-scanner,cors-header-checker,http-header-checker}-openapi.json
generated: '2026-08-11'
method: generated
---

# Probe a host's exposure with _done

> **Authorisation first.** `port-scanner` runs an active TCP scan from _done's infrastructure
> against a target you name. Only scan hosts you own or are explicitly permitted to test. _done
> publishes no acceptable-use policy (`/terms` → 404), so the responsibility is entirely yours.

## Steps

1. **Scan the ports.** `POST https://port-scanner.underscoredone.com/scan` (`scan_scan_post`) with
   `{"target": "scanme.nmap.org", "ports": "1-1000", "scan_type": "tcp_connect", "timeout": 30}`.
   - `target` is a hostname or IP.
   - `ports` accepts a range (`"1-1000"`), a comma list (`"22,80,443"`), or a mix.
   - `scan_type` currently supports only `tcp_connect`.
   - `timeout` is bounded by the schema (5–120 seconds); a wide range needs a high timeout.

2. **Check the CORS grant.** `POST https://cors-header-checker.underscoredone.com/check`
   (`handler_check_post`) with `{"url": "https://api.github.com", "origin": "https://myapp.com"}`.
   Returns exactly which cross-origin permissions that server grants that origin.

3. **Read the security headers.** `POST https://http-header-checker.underscoredone.com/check`
   (`handler_check_post`) with `{"url": "https://example.com", "method": "GET",
   "follow_redirects": true}` and inspect HSTS, CSP, X-Frame-Options and cookie flags. Note this
   is a *different* service from step 2 despite sharing the operationId `handler_check_post`.

## Rules

- Three paid calls ($0.03) per host. All are payment-gated — see `done-pay-a-402-call`.
- A wide port range is one call, not one per port; widen `ports` rather than looping.
- These operations act on third-party infrastructure. Log the target, the requester and the
  authorisation basis before running step 1.
- `400` is a rejected target or malformed range; `422` is a missing/mistyped field. Neither
  carries a machine-readable code — read `detail`.
