# _done (done)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

_done is an agent-native catalog of 26 single-purpose utility REST APIs — network and DNS lookups, domain intelligence, email-authentication checks, HTTP and SEO inspection, OCR, screenshots, hashing, JSON tooling, web3 resolution and finance calculators. There are no accounts, no signups and no API keys: every call is metered individually at $0.01 in USDC over the x402 protocol, settled on Base Mainnet or Solana Mainnet through the Coinbase CDP facilitator. Each service runs on its own subdomain, exposes a single POST operation, and publishes its own OpenAPI 3.1.0 spec annotated for AI agents with x-ai-instructions, x-guidance, x-pricing and x-402 payment metadata. Discovery is served from /.well-known/x402.json, /llms.txt, robots.txt and sitemap.xml. There is no MCP server, no A2A agent card, no SDK, no changelog, no status page and no published terms of service.

**APIs.json:** [https://done.apievangelist.com/apis.yml](https://done.apievangelist.com/apis.yml)

## Tags

- developer-tools
- utility-apis
- ai-agents
- agent-native
- x402
- pay-per-call
- web3
- crypto-payments
- dns
- domains
- email-security
- network-security
- seo
- ocr
- data
- fintech-calculators

## Timestamps

- **Created:** 2026-08-10
- **Modified:** 2026-08-11

## APIs

### _done Catalog

Single-page agent-native catalog of the 26 _done pay-per-call utility APIs. Publishes a real llms.txt, a robots.txt, a sitemap.xml and an x402 resource manifest at /.well-known/x402.json listing every payment-gated endpoint with its price, chain, asset, payTo address, OpenAPI URL and info page. The aggregate https://underscoredone.com/openapi.json is a valid OpenAPI 3.1.0 document but its paths object is EMPTY — the real contracts are the 26 per-service specs on the service subdomains.

- **Human URL:** [https://underscoredone.com](https://underscoredone.com)
- **Base URL:** `https://underscoredone.com`

#### Tags

- api-catalog
- agent-native
- llms-txt
- x402
- discovery
- pay-per-call

#### Properties

- [Documentation](https://underscoredone.com)
- [L L Ms Txt](llms/done-llms.txt)
- [Well Known](well-known/done-well-known.yml)
- [Postman Collection](collections/done-asn-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-asn-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-bimi-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-bimi-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-cors-header-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-cors-header-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-cpi-report-us.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-cpi-report-us.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-curl-http-request.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-curl-http-request.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-directory-submission-lite.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-directory-submission-lite.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-dmarc-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-dmarc-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-dns-whois-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-dns-whois-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-domain-age-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-domain-age-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-domain-availability-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-domain-availability-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-ens-resolver.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-ens-resolver.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-hackernews-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-hackernews-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-hash-hmac.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-hash-hmac.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-http-header-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-http-header-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-http-status-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-http-status-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-json-suite.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-json-suite.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-leetspeak-translator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-leetspeak-translator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-mortgage-amortization.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-mortgage-amortization.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-ocr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-ocr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-port-scanner.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-port-scanner.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-qr-code-generator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-qr-code-generator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-screenshots.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-screenshots.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-seo-data-extractor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-seo-data-extractor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-shopify-ai-rank-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-shopify-ai-rank-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-sitemap-url-extractor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-sitemap-url-extractor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/done-url-uptime-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-url-uptime-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ASN Lookup

Look up the network operator, country, and address block behind any IP address or ASN number. Given an internet address (IP) or a network identification number (ASN), this tool returns who operates that piece of the internet: the network number, the owner's name, the country it's registered in, the regional registry that manages it, and the exact address range it belongs to. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /lookup.

- **Human URL:** [https://underscoredone.com/asn_lookup/](https://underscoredone.com/asn_lookup/)
- **Base URL:** `https://asn-lookup.underscoredone.com`

#### Tags

- network
- asn
- lookup
- ip-address
- autonomous-system
- threat-intel
- abuse-reporting
- infrastructure-mapping
- whois
- cidr
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/asn_lookup/)
- [API Reference](https://underscoredone.com/asn_lookup/)
- [OpenAPI](openapi/done-asn-lookup-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-asn-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-asn-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://asn-lookup.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-asn-lookup-overlay.yaml)

### BIMI Checker

Checks whether a website's email branding setup is correct so its logo shows up in inboxes. Checks one or more website addresses to see if they are properly set up to show a brand logo next to emails in inboxes like Gmail, Apple Mail, and Yahoo. It looks up the special settings the domain has published, checks that the logo picture follows the required format, checks that a security certificate for the logo (if any) is valid and not expired, and confirms the domain has strict enough email protection rules turned on. It returns a clear pass or fail for each domain along with a plain list of what is broken if something fails. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/bimi_checker/](https://underscoredone.com/bimi_checker/)
- **Base URL:** `https://bimi-checker.underscoredone.com`

#### Tags

- bimi
- bimi-checker
- email-branding
- dmarc
- vmc-certificate
- email-authentication
- brand-indicators-for-message-identification
- logo-validation
- email-deliverability
- svg-validation
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/bimi_checker/)
- [API Reference](https://underscoredone.com/bimi_checker/)
- [OpenAPI](openapi/done-bimi-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-bimi-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-bimi-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://bimi-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-bimi-checker-overlay.yaml)

### CORS Header Checker

Send a URL and origin, get back exactly which cross-origin permissions that server grants. Sends a real request to any URL you provide, attaches an Origin header, and reads back all six standard cross-origin permission headers the server returns. Tells you whether cross-origin requests are enabled at all, whether your specific origin is permitted, and shows you every permission value exactly as the server sent it. Perfect for figuring out why a browser is blocking a request, confirming a freshly deployed service is configured correctly, or auditing whether a public API allows credentialed cross-origin calls. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/cors_header_checker/](https://underscoredone.com/cors_header_checker/)
- **Base URL:** `https://cors-header-checker.underscoredone.com`

#### Tags

- network
- cors
- header
- checker
- cross-origin
- access-control
- cors-debug
- browser-blocked
- preflight
- origin-allowed
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/cors_header_checker/)
- [API Reference](https://underscoredone.com/cors_header_checker/)
- [OpenAPI](openapi/done-cors-header-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-cors-header-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-cors-header-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://cors-header-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-cors-header-checker-overlay.yaml)

### US CPI Data & Inflation Report

Returns the latest, a specific month's, or a historical range of official US inflation (CPI) figures from BLS . Gives you official United States inflation numbers from the government's BLS Consumer Price Index. Ask for the newest reading, a specific month in the past, or a whole range of months, and get back clear percentages for overall inflation and 'core' inflation (which ignores food and energy prices), plus a plain-English summary sentence. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /cpi.

- **Human URL:** [https://underscoredone.com/cpi_report_us/](https://underscoredone.com/cpi_report_us/)
- **Base URL:** `https://cpi-report-us.underscoredone.com`

#### Tags

- cpi-report
- cpi-consumer-price-index
- consumer-index-number
- consumer-index-price
- consumer-index-rate
- consumer-price-index-figures
- cpi-index-report
- cpi-price-index
- current-price-index
- price-index-consumer
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/cpi_report_us/)
- [API Reference](https://underscoredone.com/cpi_report_us/)
- [OpenAPI](openapi/done-cpi-report-us-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-cpi-report-us.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-cpi-report-us.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://cpi-report-us.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-cpi-report-us-overlay.yaml)

### Curl HTTP Request

Make a real HTTP request from the cloud and get back the status code, headers, and body instantly. Send an HTTP request to any URL from our servers and receive the full response — including the status code, all response headers, and the body content. Supports GET, POST, PUT, PATCH, DELETE, and HEAD. Automatically follows up to 3 redirects. Useful for testing endpoints, verifying servers are responding correctly, debugging redirect chains, or fetching raw data without needing a local setup. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /curl.

- **Human URL:** [https://underscoredone.com/curl_http_request/](https://underscoredone.com/curl_http_request/)
- **Base URL:** `https://curl-http-request.underscoredone.com`

#### Tags

- network
- curl
- http-request
- fetch-url
- check-endpoint
- status-code
- response-headers
- redirect-follow
- api-tester
- debug-server
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/curl_http_request/)
- [API Reference](https://underscoredone.com/curl_http_request/)
- [OpenAPI](openapi/done-curl-http-request-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-curl-http-request.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-curl-http-request.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://curl-http-request.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-curl-http-request-overlay.yaml)

### Directory Submission Lite

Places an order to have a website submitted to twenty directories, returning a confirmation number to track it. Places an order to have a website submitted to twenty directories that publish a link back to it, and returns a confirmation number so the order can be checked later for free. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 2 operation(s): POST /submit, POST /status.

- **Human URL:** [https://underscoredone.com/directory_submission_lite/](https://underscoredone.com/directory_submission_lite/)
- **Base URL:** `https://directory-submission-lite.underscoredone.com`

#### Tags

- network
- directory-submission
- backlinks
- seo
- indexing
- link-building
- new-website
- search-engine-discovery
- site-submission
- order
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/directory_submission_lite/)
- [API Reference](https://underscoredone.com/directory_submission_lite/)
- [OpenAPI](openapi/done-directory-submission-lite-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-directory-submission-lite.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-directory-submission-lite.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://directory-submission-lite.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-directory-submission-lite-overlay.yaml)

### Bulk DMARC Record Lookup

Check email security (DMARC) configuration for one or many domains in a single request. Give this tool a list of domain names and it will instantly check each one's DMARC email security record. DMARC is a standard that tells email providers how to handle fake or spoofed emails pretending to come from your domain. For each domain you submit, you get back whether a valid record exists, what the policy is (none, quarantine, or reject), whether reporting addresses are set up, and the full raw record text. Perfect for auditing many domains at once without any setup. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /dmarc-lookup.

- **Human URL:** [https://underscoredone.com/dmarc_lookup/](https://underscoredone.com/dmarc_lookup/)
- **Base URL:** `https://dmarc-lookup.underscoredone.com`

#### Tags

- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/dmarc_lookup/)
- [API Reference](https://underscoredone.com/dmarc_lookup/)
- [OpenAPI](openapi/done-dmarc-lookup-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-dmarc-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-dmarc-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://dmarc-lookup.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-dmarc-lookup-overlay.yaml)

### DNS & WHOIS Lookup

Look up all 13 DNS record types plus full WHOIS registration data for up to 10 domains in one call. Send up to 10 domain names and get back every DNS record type (A, AAAA, MX, CNAME, TXT, NS, PTR, SOA, SRV, CAA, NAPTR, DS, TLSA) plus the full WHOIS registration profile (registrar, dates, contacts, status, nameservers) for each one. URLs are accepted and automatically stripped down to the bare domain. Duplicate domains are quietly removed before processing. Results come back as one flat row per domain, ready to drop into a spreadsheet, database, or pipeline. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /lookup.

- **Human URL:** [https://underscoredone.com/dns_whois_lookup/](https://underscoredone.com/dns_whois_lookup/)
- **Base URL:** `https://dns-whois-lookup.underscoredone.com`

#### Tags

- network
- dns
- whois
- domain-lookup
- dns-records
- domain-audit
- mx-record
- spf-dkim-dmarc
- domain-expiry
- migration-verification
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/dns_whois_lookup/)
- [API Reference](https://underscoredone.com/dns_whois_lookup/)
- [OpenAPI](openapi/done-dns-whois-lookup-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-dns-whois-lookup.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-dns-whois-lookup.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://dns-whois-lookup.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-dns-whois-lookup-overlay.yaml)

### Domain Age Checker

Give it a list of domains and get back registration date, expiration date, age, and time remaining — instantly. Send a list of domain names and this tool tells you exactly how old each one is, when it was first registered, when it expires, and how much time is left before expiration. Great for spotting brand-new suspicious domains, researching competitors, or evaluating domains before buying or linking to them. Works with over 100 domain extensions worldwide. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /lookup.

- **Human URL:** [https://underscoredone.com/domain_age_checker/](https://underscoredone.com/domain_age_checker/)
- **Base URL:** `https://domain-age-checker.underscoredone.com`

#### Tags

- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/domain_age_checker/)
- [API Reference](https://underscoredone.com/domain_age_checker/)
- [OpenAPI](openapi/done-domain-age-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-domain-age-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-domain-age-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://domain-age-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-domain-age-checker-overlay.yaml)

### Domain Availability Checker

Check whether 1–10 domain names have an active registration record using the official RDAP protocol. Give this API up to 10 domain names and it will tell you whether each one has a registration record on file with the official registry. It uses RDAP — the modern, structured replacement for WHOIS — so there is no messy free-text parsing. Each domain comes back labeled 'registered', 'unregistered', or 'indeterminate' (when the registry does not support RDAP for that ending). Important: 'unregistered' means no record was found, which usually means the name is available — but reserved or premium names can also return no record. This API tells you registration status only; it does not tell you price, premium status, or whether a registrar will actually let you buy the name. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/domain_availability_checker/](https://underscoredone.com/domain_availability_checker/)
- **Base URL:** `https://domain-availability-checker.underscoredone.com`

#### Tags

- network
- domain
- availability
- checker
- rdap
- whois
- domain-lookup
- tld
- registration-status
- name-search
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/domain_availability_checker/)
- [API Reference](https://underscoredone.com/domain_availability_checker/)
- [OpenAPI](openapi/done-domain-availability-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-domain-availability-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-domain-availability-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://domain-availability-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-domain-availability-checker-overlay.yaml)

### ENS Resolver

Resolve an ENS name to an Ethereum address, or an address back to its ENS name. Look up an ENS name or an Ethereum address and get back the matching one, automatically figuring out which direction you need. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /resolve.

- **Human URL:** [https://underscoredone.com/ens_resolver/](https://underscoredone.com/ens_resolver/)
- **Base URL:** `https://ens-resolver.underscoredone.com`

#### Tags

- network
- ens
- resolver
- ethereum
- wallet-address
- ens-name-lookup
- blockchain-identity
- reverse-resolve
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/ens_resolver/)
- [API Reference](https://underscoredone.com/ens_resolver/)
- [OpenAPI](openapi/done-ens-resolver-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-ens-resolver.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-ens-resolver.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://ens-resolver.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-ens-resolver-overlay.yaml)

### Hacker News Data

Fetch Hacker News stories by category, or scan all stories/jobs/polls from a specific date, with optional nested comments. This tool reads live information from Hacker News, a popular website where people share and discuss technology news. You can either ask for a current list of stories (like the Top, New, Best, Ask, Show, or Job lists) or ask for every story, job posting, and poll that was posted on one specific calendar day in the past. You can also choose to pull in the discussion comments underneath each story, including nested replies several levels deep. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /fetch.

- **Human URL:** [https://underscoredone.com/hackernews_data/](https://underscoredone.com/hackernews_data/)
- **Base URL:** `https://hackernews-data.underscoredone.com`

#### Tags

- network
- hackernews
- hacker-news
- hn-api
- stories
- comments
- jobs
- polls
- date-scan
- developer-news
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/hackernews_data/)
- [API Reference](https://underscoredone.com/hackernews_data/)
- [OpenAPI](openapi/done-hackernews-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-hackernews-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-hackernews-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://hackernews-data.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-hackernews-data-overlay.yaml)

### Hashing, HMAC & Checksum Suite

Compute cryptographic hashes, HMAC signatures, and checksums — and verify webhook signatures with constant-time comparison. Give this API any text or binary data and it instantly returns its fingerprint under whichever hash algorithms you choose — SHA-256, SHA-512, MD5, BLAKE2, CRC32, and more. It also signs data with a secret key (HMAC) and, most importantly, safely verifies whether an incoming signature matches — using a timing-safe comparison that prevents secret-leaking attacks. Language models cannot perform hashing: they produce a string of the right length and character set that looks correct but is simply wrong. Every webhook verification, idempotency key, cache fingerprint, or integrity check that relies on a hallucinated hash is silently broken. This API is the cure. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /hash.

- **Human URL:** [https://underscoredone.com/hash_hmac/](https://underscoredone.com/hash_hmac/)
- **Base URL:** `https://hash-hmac.underscoredone.com`

#### Tags

- security
- hash
- hmac
- checksum
- sha256
- webhook-verification
- content-fingerprint
- idempotency-key
- signature-verify
- blake2
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/hash_hmac/)
- [API Reference](https://underscoredone.com/hash_hmac/)
- [OpenAPI](openapi/done-hash-hmac-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-hash-hmac.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-hash-hmac.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://hash-hmac.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-hash-hmac-overlay.yaml)

### HTTP Header Checker

Fetches any web address and returns its response headers, status code, and redirect path. Sends a request to a web address you provide and reports back everything the server said in response: the status code, all the response headers, how many times it got redirected, and how long the whole thing took. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/http_header_checker/](https://underscoredone.com/http_header_checker/)
- **Base URL:** `https://http-header-checker.underscoredone.com`

#### Tags

- network
- http-header-checker
- headers
- url-lookup
- redirect-check
- security-headers
- cache-control
- status-code
- web-debugging
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/http_header_checker/)
- [API Reference](https://underscoredone.com/http_header_checker/)
- [OpenAPI](openapi/done-http-header-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-http-header-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-http-header-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://http-header-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-http-header-checker-overlay.yaml)

### HTTP Status Code Checker

Check the live status of up to 10 URLs at once and detect redirects instantly. Give this API a list of up to 10 web addresses and it will visit each one to tell you whether it is working, broken, or redirecting visitors somewhere else. You get back the exact status number (like 200 for OK, 404 for not found, 500 for server error), whether the address redirects, and where it redirects to. Great for finding broken links, verifying website migrations, and running quick SEO audits without writing any code. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/http_status_checker/](https://underscoredone.com/http_status_checker/)
- **Base URL:** `https://http-status-checker.underscoredone.com`

#### Tags

- network
- http
- status
- checker
- redirect
- broken-links
- seo-audit
- link-validation
- website-migration
- url-health
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/http_status_checker/)
- [API Reference](https://underscoredone.com/http_status_checker/)
- [OpenAPI](openapi/done-http-status-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-http-status-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-http-status-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://http-status-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-http-status-checker-overlay.yaml)

### JSON Validate, Repair, Convert, Query & Diff

One endpoint to validate, repair, format, query, diff, convert, and canonicalize JSON — the most common operation in every agent workflow. Every AI agent and developer runs into broken or confusing JSON constantly. This tool handles all the most common JSON headaches in one place: check if JSON is valid (with exact error location), fix near-JSON that has typos or formatting mistakes, pretty-print or minify, pull out specific values using a path expression, compare two JSON documents and see exactly what changed, convert to and from YAML or CSV, produce a byte-stable canonical form for hashing or signing, validate against a schema, and get size and structure statistics. Same input always gives the same output — fully predictable, no side effects. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /json.

- **Human URL:** [https://underscoredone.com/json_suite/](https://underscoredone.com/json_suite/)
- **Base URL:** `https://json-suite.underscoredone.com`

#### Tags

- parsing
- json
- validate
- repair
- jsonpath
- diff
- canonicalize
- convert
- yaml
- csv
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/json_suite/)
- [API Reference](https://underscoredone.com/json_suite/)
- [OpenAPI](openapi/done-json-suite-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-json-suite.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-json-suite.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://json-suite.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-json-suite-overlay.yaml)

### Leetspeak Translator

Converts regular text into leetspeak or decodes leetspeak back into normal readable text. Takes a piece of text and either turns it into leetspeak (swapping some letters for numbers and symbols, like 'hello' becoming 'h3110') or turns leetspeak back into normal, easy-to-read words. The same words always produce the same result, so answers never change unexpectedly. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /translate.

- **Human URL:** [https://underscoredone.com/leetspeak_translator/](https://underscoredone.com/leetspeak_translator/)
- **Base URL:** `https://leetspeak-translator.underscoredone.com`

#### Tags

- text
- leetspeak
- translator
- leet
- encode-text
- decode-text
- text-obfuscation
- character-substitution
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/leetspeak_translator/)
- [API Reference](https://underscoredone.com/leetspeak_translator/)
- [OpenAPI](openapi/done-leetspeak-translator-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-leetspeak-translator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-leetspeak-translator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://leetspeak-translator.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-leetspeak-translator-overlay.yaml)

### Mortgage & Loan Amortization Calculator

Get the exact monthly payment and full period-by-period breakdown for any fixed-rate loan — results an AI model cannot reliably compute on its own. Give this API a loan amount, an interest rate, and a repayment term, and it hands back the precise monthly payment plus a complete schedule showing — for every single month — how much goes to interest, how much reduces the balance, and what you still owe. You can also ask 'what if I pay an extra $300 a month?' or 'what if I make a $10,000 lump payment in month 24?' and it will tell you exactly how many months you save and how much interest you avoid. Every number is computed with banker's rounding and a pinned arithmetic rule so that two correct systems running the same inputs produce identical results, down to the cent. No rate lookups, no market data — you supply the rate, the API does the math. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /calculate.

- **Human URL:** [https://underscoredone.com/mortgage_amortization/](https://underscoredone.com/mortgage_amortization/)
- **Base URL:** `https://mortgage-amortization.underscoredone.com`

#### Tags

- math
- mortgage
- amortization
- loan
- monthly-payment
- repayment-schedule
- interest-calculation
- extra-payment
- lump-sum
- real-estate
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/mortgage_amortization/)
- [API Reference](https://underscoredone.com/mortgage_amortization/)
- [OpenAPI](openapi/done-mortgage-amortization-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-mortgage-amortization.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-mortgage-amortization.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://mortgage-amortization.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-mortgage-amortization-overlay.yaml)

### OCR Text Extractor

Extract text from any image using Tesseract OCR. Send a picture, either as a public web address or as base64-encoded image data, and get back the plain text found inside it. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /read.

- **Human URL:** [https://underscoredone.com/ocr/](https://underscoredone.com/ocr/)
- **Base URL:** `https://ocr.underscoredone.com`

#### Tags

- text
- ocr
- read
- image-to-text
- extract-text
- screenshot-reader
- document-scan
- receipt-reader
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/ocr/)
- [API Reference](https://underscoredone.com/ocr/)
- [OpenAPI](openapi/done-ocr-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-ocr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-ocr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://ocr.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-ocr-overlay.yaml)

### TCP Port Scanner

Send a host and port range, get back a clean list of which ports are open and what services are running on them. Give this API a hostname or IP address and it will try connecting to each port in your requested range. For every port that answers, it tells you whether it is open or blocked, which service is likely running there (like a web server or SSH), and what software version was detected. This saves you from installing network tools, parsing messy command-line output, or writing socket loops yourself. Only scan hosts you own or have permission to scan — this tool does not check that for you. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /scan.

- **Human URL:** [https://underscoredone.com/port_scanner/](https://underscoredone.com/port_scanner/)
- **Base URL:** `https://port-scanner.underscoredone.com`

#### Tags

- network
- port
- scanner
- tcp
- open-ports
- service-detection
- nmap
- infrastructure
- security-audit
- firewall-check
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/port_scanner/)
- [API Reference](https://underscoredone.com/port_scanner/)
- [OpenAPI](openapi/done-port-scanner-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-port-scanner.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-port-scanner.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://port-scanner.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-port-scanner-overlay.yaml)

### Bulk QR Code Generator

Turn a list of text, URLs, or any strings into QR code images instantly — one call, many codes. Send a list of texts — website addresses, phone numbers, plain words, WiFi details, anything — and get back a ready-to-use QR code image for each one. Every QR code comes as a base64-encoded PNG you can drop straight into a webpage or save to disk. Great for marketing campaigns, event tickets, product labels, menus, or any situation where you need many QR codes in one go. Empty entries are quietly skipped. Each input is limited to 700 characters. You must send at least one non-empty entry. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /generate.

- **Human URL:** [https://underscoredone.com/qr_code_generator/](https://underscoredone.com/qr_code_generator/)
- **Base URL:** `https://qr-code-generator.underscoredone.com`

#### Tags

- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/qr_code_generator/)
- [API Reference](https://underscoredone.com/qr_code_generator/)
- [OpenAPI](openapi/done-qr-code-generator-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-qr-code-generator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-qr-code-generator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://qr-code-generator.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-qr-code-generator-overlay.yaml)

### Screenshots

Capture a screenshot of a fully rendered webpage, including JavaScript-heavy pages. Renders a webpage exactly as a real browser would, including all its scripts and dynamic content, then takes a picture of it. You can capture just the visible area or the whole scrollable page, choose the screen size, wait for slow-loading images to finish, and hide cookie banners or popups before the picture is taken. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /capture.

- **Human URL:** [https://underscoredone.com/screenshots/](https://underscoredone.com/screenshots/)
- **Base URL:** `https://screenshots.underscoredone.com`

#### Tags

- network
- screenshots
- url-to-screenshot
- url-to-secreenshot
- webpage-capture
- browser-rendering
- full-page-screenshot
- website-image
- puppeteer
- headless-browser
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/screenshots/)
- [API Reference](https://underscoredone.com/screenshots/)
- [OpenAPI](openapi/done-screenshots-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-screenshots.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-screenshots.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://screenshots.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-screenshots-overlay.yaml)

### SEO Data Extractor

Fetch a webpage and instantly extract all key SEO fields: title, meta tags, headings, canonical URL, and more. Give this API a web address and it will visit that page, then hand back everything an SEO professional needs to know: the page title, meta description, meta keywords, robots instructions, canonical link, H1/H2/H3 headings, how many links are on the page, and the HTTP status code. No setup required — just paste a URL and get structured data back in under two seconds. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /extract.

- **Human URL:** [https://underscoredone.com/seo_data_extractor/](https://underscoredone.com/seo_data_extractor/)
- **Base URL:** `https://seo-data-extractor.underscoredone.com`

#### Tags

- parsing
- seo
- data
- extractor
- meta-tags
- title-tag
- canonical
- headings
- seo-audit
- competitor-analysis
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/seo_data_extractor/)
- [API Reference](https://underscoredone.com/seo_data_extractor/)
- [OpenAPI](openapi/done-seo-data-extractor-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-seo-data-extractor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-seo-data-extractor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://seo-data-extractor.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-seo-data-extractor-overlay.yaml)

### Shopify AI Rank Checker

Check exactly where your Shopify product ranks when AI shopping assistants like ChatGPT and Gemini search for it. Checks how well a Shopify store's products show up when AI shopping assistants such as ChatGPT, Gemini, Perplexity, Grok, and Copilot search for products, and reports the store's rank and its closest competitors. Searches Shopify's real Global Catalog — the same product index AI assistants read from. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /rank.

- **Human URL:** [https://underscoredone.com/shopify_ai_rank_checker/](https://underscoredone.com/shopify_ai_rank_checker/)
- **Base URL:** `https://shopify-ai-rank-checker.underscoredone.com`

#### Tags

- network
- shopify-rank-checker
- ai-shopping-visibility
- chatgpt-product-rank
- gemini-shopping-search
- shopify-seo
- global-catalog
- ucp-mcp
- product-rank-tracker
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/shopify_ai_rank_checker/)
- [API Reference](https://underscoredone.com/shopify_ai_rank_checker/)
- [OpenAPI](openapi/done-shopify-ai-rank-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-shopify-ai-rank-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-shopify-ai-rank-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://shopify-ai-rank-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-shopify-ai-rank-checker-overlay.yaml)

### Sitemap URL Extractor

Give it a sitemap.xml link and get back every URL listed in it — including nested sub-sitemaps — with metadata like last modified date and change frequency. Give this API a link to any website's sitemap.xml file and it will fetch and parse it, returning every URL found inside. If the sitemap links to other sitemaps (called sitemap indexes), it will follow and extract those too. Each URL is returned with any extra information available, such as when the page was last updated and how often it changes. Useful for SEO audits, content inventories, broken link checks, and competitive research. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /extract.

- **Human URL:** [https://underscoredone.com/sitemap_url_extractor/](https://underscoredone.com/sitemap_url_extractor/)
- **Base URL:** `https://sitemap-url-extractor.underscoredone.com`

#### Tags

- parsing
- sitemap
- url-extractor
- seo-audit
- content-inventory
- site-crawl
- sitemap-index
- xml-parsing
- broken-link-check
- competitive-analysis
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/sitemap_url_extractor/)
- [API Reference](https://underscoredone.com/sitemap_url_extractor/)
- [OpenAPI](openapi/done-sitemap-url-extractor-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-sitemap-url-extractor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-sitemap-url-extractor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://sitemap-url-extractor.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-sitemap-url-extractor-overlay.yaml)

### URL Uptime Checker

Checks whether a website or web address is currently reachable and reports how fast it responded. Pay-per-call at $0.01 USDC over x402 on Base or Solana — no account, no API key. OpenAPI 3.1.0; 1 operation(s): POST /check.

- **Human URL:** [https://underscoredone.com/url_uptime_checker/](https://underscoredone.com/url_uptime_checker/)
- **Base URL:** `https://url-uptime-checker.underscoredone.com`

#### Tags

- network
- url-uptime-checker
- website-status
- reachability-check
- uptime-monitor
- url-validator
- site-down-detector
- http-status-check
- x402
- pay-per-call
- agent-native
- utility-apis
- developer-tools

#### Properties

- [Documentation](https://underscoredone.com/url_uptime_checker/)
- [API Reference](https://underscoredone.com/url_uptime_checker/)
- [OpenAPI](openapi/done-url-uptime-checker-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/done-url-uptime-checker.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/done-url-uptime-checker.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://url-uptime-checker.underscoredone.com/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Overlay](overlays/done-url-uptime-checker-overlay.yaml)

## Common Properties

- [M C P Server](mcp/done-mcp.yml)
- [Developer Portal](https://underscoredone.com)
- [Documentation](https://underscoredone.com)
- [API Reference](https://underscoredone.com/#apis)
- [GitHub Organization](https://github.com/underscoredone)
- [Support](https://forms.gle/5KzuSFH7p8hHtDmz7)
- [L L Ms Txt](llms/done-llms.txt)
- [Well Known](well-known/done-well-known.yml)
- [Authentication](authentication/done-authentication.yml)
- [Conventions](conventions/done-conventions.yml)
- [Error Catalog](errors/done-problem-types.yml)
- [Lifecycle](lifecycle/done-lifecycle.yml)
- [Conformance](conformance/done-conformance.yml)
- [Domain Security](security/done-domain-security.yml)
- [Agentic Access](agentic-access/done-agentic-access.yml)
- [Agent Skill](skills/_index.yml)
- [Examples](examples/done-examples.yml)
- [Data Model](data-model/done-data-model.yml)
- [Plans](plans/done-plans-pricing.yml)
- [Pricing](https://underscoredone.com/#apis)
- [Rate Limits](rate-limits/done-rate-limits.yml)
- [Packages](packages/done-packages.yml)

## Maintainers

**FN:** _done
**Email:** info@underscoredone.com
**URL:** https://underscoredone.com
