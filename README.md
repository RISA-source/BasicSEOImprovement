# SEO Fundamentals — Live Reference

A single-page SEO reference guide that teaches every foundational search engine optimisation technique while implementing each one live on itself. Every concept described in the page is actively demonstrated in the page's own source code.

**Live site:** https://risa-source.github.io/BasicSEOImprovement/

---

## What This Is

This is not a static article about SEO. The HTML is annotated with detailed comments at every relevant point — open DevTools alongside the guide and follow every concept in the actual source. The robots.txt and sitemap.xml are correct, production-ready files that complement the main page.

---

## Repository Structure

```
.
├── index.html          # SEO guide + live implementation
├── style.css           # Referenced by index.html
├── robots.txt          # Crawler directives (production URL)
├── sitemap.xml         # XML sitemap (production URLs)
└── optimized-image.jpg # Page image asset
```

---

## Topics Covered

**Head Tags**
- `charset` and `viewport` — the non-negotiables
- `<title>` — the most impactful on-page SEO element
- `<meta name="description">` — click-through rate signal
- `<meta name="robots">` — index/noindex/follow/nofollow
- `<link rel="canonical">` — duplicate content prevention
- `<meta name="author">` and `<meta name="theme-color">`

**Social Sharing**
- Open Graph protocol — Facebook, LinkedIn, Slack, iMessage
- Twitter Card meta tags — `summary_large_image` vs `summary`
- og:image sizing and hosting requirements

**Structured Data**
- JSON-LD format and why Google recommends it over Microdata
- Schema.org types: Article, Product, FAQPage, LocalBusiness, Person, Event, BreadcrumbList
- How to trigger rich results in the SERP
- Testing with Google's Rich Results Test

**Technical Files**
- `robots.txt` — syntax, User-agent targeting, Disallow patterns, Crawl-delay, blocking AI scrapers
- `sitemap.xml` — `<loc>`, `<lastmod>`, `<changefreq>`, `<priority>` explained
- What to include and exclude from a sitemap

**Content & Markup**
- Heading hierarchy — one H1, logical nesting, never skip levels
- Semantic HTML element reference with SEO signal weight per element
- `lang` attribute on `<html>`

**Image Optimisation**
- `alt` text — how to write it, what to avoid
- `width` and `height` attributes — preventing Cumulative Layout Shift
- `loading="lazy"` vs `loading="eager"` — when to use each
- `decoding="async"` — off-thread image decode
- `<figure>` and `<figcaption>` for semantic context

**Core Web Vitals**
- LCP (Largest Contentful Paint) — target: &lt; 2.5s
- CLS (Cumulative Layout Shift) — target: &lt; 0.1
- INP (Interaction to Next Paint) — target: &lt; 200ms
- `dns-prefetch`, `preconnect`, non-render-blocking CSS
- `font-display: swap`

---

## Useful Testing Tools

| Tool | Purpose |
|---|---|
| [Google Rich Results Test](https://search.google.com/test/rich-results) | Validate JSON-LD structured data |
| [PageSpeed Insights](https://pagespeed.web.dev/) | Core Web Vitals measurement |
| [Google Search Console](https://search.google.com/search-console) | Sitemap submission, index coverage |
| [Open Graph Debugger](https://developers.facebook.com/tools/debug/) | Preview OG card rendering |
| [Twitter Card Validator](https://cards-dev.twitter.com/validator) | Preview Twitter Card rendering |
| [schema.org Validator](https://validator.schema.org/) | Validate structured data |
