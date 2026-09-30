---
name: Replit Jekyll preview SEO
description: Distinguishes Replit's live Jekyll preview behavior from a GitHub Pages production build.
---

When a Jekyll site targets GitHub Pages, verify its sitemap, robots output, and SEO against a standalone Jekyll build using the site's configured URL. Do not assume the Replit preview response represents production indexing behavior.

**Why:** The live Replit preview added an `X-Robots-Tag: noindex` header, and Jekyll's bound preview host/port appeared in generated sitemap URLs. A standalone static build correctly used the configured GitHub Pages domain.

**How to apply:** Before changing site code to address an SEO warning, compare the preview response with the standalone build. Keep Replit's proxy-only `noindex` header out of production source and confirm the generated sitemap and robots file use the production URL.