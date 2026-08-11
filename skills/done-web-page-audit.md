---
name: done-web-page-audit
description: >-
  Audit a web page or a whole site with _done — discover URLs from the sitemap, check live status
  and redirects, extract SEO metadata, inspect response headers, and capture a rendered
  screenshot. Up to five paid calls, $0.01 each.
api: _done
provider: https://underscoredone.com
operations:
  - handler_extract_post         # sitemap-url-extractor POST /extract
  - check_urls_check_post        # http-status-checker POST /check
  - handler_extract_post         # seo-data-extractor POST /extract
  - handler_check_post           # http-header-checker POST /check
  - handler_capture_post         # screenshots POST /capture
source: openapi/_original/done-{sitemap-url-extractor,http-status-checker,seo-data-extractor,http-header-checker,screenshots}-openapi.json
generated: '2026-08-11'
method: generated
---

# Audit a page or site with _done

> Two of these operations are both called `handler_extract_post` (sitemap and SEO extractor).
> Address them by host, not by operationId.

## Steps

1. **Enumerate the site (optional).**
   `POST https://sitemap-url-extractor.underscoredone.com/extract` (`handler_extract_post`) with
   `{"sitemap_url": "https://example.com/sitemap.xml"}`. Follows nested sub-sitemaps and returns
   each URL with lastmod and changefreq.

2. **Check liveness and redirects.**
   `POST https://http-status-checker.underscoredone.com/check` (`check_urls_check_post`) with
   `{"urls": ["https://example.com", "https://example.com/pages/contact"]}` — **1 to 10 URLs per
   call**, each must include the scheme. Chunk step 1's output into batches of 10.

3. **Extract SEO fields.** `POST https://seo-data-extractor.underscoredone.com/extract`
   (`handler_extract_post`) with `{"url": "https://www.example.com"}`. Optional
   `timeout_seconds` (1–120 per the schema) for slow pages. Returns title, meta tags, headings
   and canonical URL. One URL per call — this one does not batch.

4. **Inspect response headers.** `POST https://http-header-checker.underscoredone.com/check`
   (`handler_check_post`) with `{"url": "https://example.com", "method": "GET",
   "follow_redirects": true}`. Use `method: "HEAD"` when you only need headers. This is where you
   read HSTS, CSP, cache and cookie headers.

5. **Capture the rendered page.** `POST https://screenshots.underscoredone.com/capture`
   (`handler_capture_post`) with `{"url": "https://example.com", "full_page": false,
   "viewport": {"width": 1920, "height": 1080}, "wait_until": "networkidle0",
   "allow_popups": false, "load_lazy": true}`. `wait_until` accepts `load`, `domcontentloaded`,
   `networkidle0`, `networkidle2`. Set `load_lazy: true` for image-heavy pages and
   `allow_popups: false` to suppress cookie banners before capture.

## Rules

- Five paid calls per full audit ($0.05 per page, plus $0.01 per batch of 10 in step 2). Only
  step 2 batches; steps 3–5 are one URL per payment.
- All five are read-only fetches. Retrying is safe for correctness but is charged again.
- These operations make _done fetch a caller-supplied URL. Do not point them at hosts you are not
  authorised to fetch, and note the provider publishes **no terms of service** governing this
  (`https://underscoredone.com/terms` → 404).
- `422` on step 2 usually means more than 10 URLs, or a URL missing its scheme.
