---
name: done-pay-a-402-call
description: >-
  Make a paid call to any _done API using the x402 protocol — the universal first step for all 26
  services. An unpaid POST returns HTTP 402 with a base64 payment challenge; sign a USDC transfer
  authorization on Base or Solana and retry the identical request with an X-PAYMENT header.
api: _done
provider: https://underscoredone.com
operations:
  - handler_lookup_post          # asn-lookup — used here as the worked example
source: >-
  https://underscoredone.com/llms.txt, openapi/_original/done-asn-lookup-openapi.json, and a live
  402 challenge observed 2026-08-11 from POST https://asn-lookup.underscoredone.com/lookup
generated: '2026-08-11'
method: generated
---

# Pay a _done call over x402

Every _done endpoint is payment-gated. There is no API key, no account and no signup — the
$0.01 payment IS the authentication. This flow is identical for all 26 services; only the host,
path and body change.

## Steps

1. **Send the request unpaid.** `POST https://asn-lookup.underscoredone.com/lookup` with
   `Content-Type: application/json` and the body the spec's `Request` schema requires —
   for ASN Lookup that is `{"query": "8.8.8.8"}` (operation `handler_lookup_post`).

2. **Expect HTTP 402, not an error.** The body is an empty object `{}`. The payload is in the
   response **header** `payment-required` — base64-encoded JSON. (The OpenAPI declares the header
   as `X-Payment-Response`; the live service sends `payment-required`. Read both.)

3. **Decode the challenge.** It contains `x402Version: 2`, a `resource` block describing the
   endpoint, an `accepts[]` array of payment rails, and an `extensions.bazaar` block whose
   `schema` is a JSON Schema 2020-12 description of the exact request body plus a worked
   response example — use it to validate your body before paying.

4. **Pick a rail from `accepts[]`.** Two are offered on every endpoint:
   - Base Mainnet — network `eip155:8453`, asset `0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913` (USDC)
   - Solana Mainnet — network `solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp`, asset `EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v`

   Both quote `amount: "10000"` — 0.01 USDC at 6 decimals — with `maxTimeoutSeconds: 300`.

5. **Sign the transfer authorization** for that amount to the challenge's `payTo` address. The
   Base rail's `extra` block (`{name: "USD Coin", version: "2"}`) is the EIP-712 domain, i.e. an
   EIP-3009 `transferWithAuthorization` signature. A facilitator is available at
   `https://api.cdp.coinbase.com/platform/v2/x402`.

6. **Retry the identical request** with the `X-PAYMENT` header carrying the signed payload. On
   success you get `200` and the service's `Response` object, which always includes `api_version`.

7. **Optionally reuse the session.** Each spec declares a `siwx` security scheme — a
   `SIGN-IN-WITH-X` header carrying a CAIP-122 wallet signature "for repeat access after payment".
   The docs do not describe its message format, so treat it as undocumented until the provider
   publishes it.

## Rules and hazards

- **There is no idempotency key.** If a call times out you cannot tell whether the $0.01 settled.
  Never blind-retry a paid call; re-quote first by sending unpaid and reading the fresh 402.
- **`400` / `422` are free-text.** `400` returns `{"detail": "<string>"}`, `422` returns
  `{"detail": [ValidationError...]}`. There is no error-code registry — branch on HTTP status only.
- **No rate limits are published and no `RateLimit-*`/`Retry-After` headers are returned.** The
  only backpressure is cost. Budget by call count, not by quota.
- **No 5xx or 429 is documented** on any operation. Treat any non-{200,400,402,422} status as
  undefined behaviour and stop.
- Validate your body against the `bazaar` JSON Schema *before* paying — a malformed body after
  payment is a wasted $0.01 with no published refund policy.
