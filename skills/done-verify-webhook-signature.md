---
name: done-verify-webhook-signature
description: >-
  Verify an inbound webhook's HMAC signature with constant-time comparison, and validate/repair
  its JSON body — using _done's hashing suite and JSON suite. Two paid calls, $0.01 each.
api: _done
provider: https://underscoredone.com
operations:
  - handler_hash_post            # hash-hmac POST /hash
  - handler_json_post            # json-suite POST /json
source: openapi/_original/done-hash-hmac-openapi.json, openapi/_original/done-json-suite-openapi.json
generated: '2026-08-11'
method: generated
---

# Verify a webhook with _done

## Steps

1. **Verify the signature.** `POST https://hash-hmac.underscoredone.com/hash`
   (`handler_hash_post`) with the raw request body as `input`, the algorithms you need, and an
   `hmac` block carrying `algorithm`, the shared secret as `key`, and the sender's
   `expected_signature`. The service compares in constant time and reports the match.
   - `input_encoding`: `utf-8` for text, `base64` for binary — base64-encode binary first.
   - `algorithms`: any of `md5`, `sha1`, `sha224`, `sha256`, `sha384`, `sha512`, `crc32` and the
     others the spec enumerates.
   - `output_encoding`: `hex` (default), `base64` or `base64url`.

2. **Only then parse the body.** `POST https://json-suite.underscoredone.com/json`
   (`handler_json_post`) with `{"op": "validate", "data_raw": "<the raw body>"}`. Use `data_raw`
   for `validate` and `repair`; use `data` (a real JSON value) for every other op.

3. **Extract what you need.** Re-call with `{"op": "query", "data": {...},
   "options": {"jsonpath": "$.order.items[*].sku"}}`. Available ops are `validate`, `repair`,
   `format`, `canonicalize`, `convert`, `query` and `diff`.

## Rules

- **Verify before you parse.** Never run step 2 on a body whose signature has not passed step 1.
- Sending a shared secret to a third party is a real trust decision. _done is keyless and
  publishes no terms of service, privacy policy or security.txt — for production secrets, compute
  the HMAC locally and use this flow for diagnosis only.
- Both calls are payment-gated ($0.02 per verification round trip); see `done-pay-a-402-call`.
- Both operations are pure functions with no stored state — but there is no idempotency key, so
  every retry is charged.
