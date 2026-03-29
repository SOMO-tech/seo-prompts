# SEO Prompts for AI-Assisted Development

A curated collection of **17 ready-to-use prompts** designed to implement comprehensive technical SEO in any React, Next.js, or modern web project using AI coding assistants (Claude, Cursor, Copilot, etc.).

## Why this exists

Setting up proper technical SEO is tedious and easy to get wrong. These prompts give your AI assistant the exact instructions it needs to generate production-grade SEO infrastructure in minutes instead of hours.

Each prompt is self-contained, copy-paste ready, and written to produce clean, typed, maintainable code.

## What's included

| # | Prompt | What it builds |
|---|--------|---------------|
| 1 | Base SEO Component | Reusable `<SEOHead>` with react-helmet-async, meta tags, OG, Twitter Cards, JSON-LD |
| 2 | Article SEO Extension | Blog/article meta tags, Article schema, reading time, multi-author |
| 3 | Static Sitemap | Hand-coded sitemap.xml for static sites |
| 4 | Hybrid Sitemap | Edge function + Supabase for mixed static/dynamic content |
| 5 | Single Function Sitemap | One edge function for up to 50K URLs |
| 6 | Paginated Sitemap | Sitemap index with pagination for 50K+ URLs |
| 7 | Standard Robots.txt | Search engine rules, disallows, sitemap reference |
| 8 | Robots.txt + AI Bots | Extended rules for GPTBot, CCBot, and other AI crawlers |
| 9 | Dynamic OG Images | API route that generates 1200×630 OG images on the fly |
| 10 | Static OG Images | Directory structure and fallback logic for pre-made OG images |
| 11 | Canonical URLs | URL normalization, trailing slashes, query param stripping |
| 12 | JSON-LD Library | TypeScript functions for 9 schema types (Organization, Article, Product, FAQ, etc.) |
| 13 | Internal Linking | Breadcrumbs, heading audit, semantic HTML, related content |
| 14 | Core Web Vitals | Image, font, JS, CSS optimization + performance monitoring |
| 15 | Error Pages | SEO-friendly 404/500 pages, redirect map, broken URL monitoring |
| 16 | International SEO | Hreflang, multilingual URL structure, language switcher |
| 17 | Review Schema | AggregateRating, Review JSON-LD, star rating component |

## How to use

1. Pick the prompt you need from the table above
2. Open the corresponding file in the `prompts/` directory
3. Copy the prompt into your AI coding assistant
4. Replace any `[bracketed placeholders]` with your project details
5. Review the generated code and ship it

## Project structure
```
prompts/
├── 01-seo-head-component.md
├── 02-article-seo-extension.md
├── 03-static-sitemap.md
├── 04-hybrid-sitemap.md
├── 05-single-function-sitemap.md
├── 06-paginated-sitemap.md
├── 07-standard-robots-txt.md
├── 08-robots-txt-ai-bots.md
├── 09-dynamic-og-images.md
├── 10-static-og-images.md
├── 11-canonical-urls.md
├── 12-json-ld-library.md
├── 13-internal-linking.md
├── 14-core-web-vitals.md
├── 15-error-pages.md
├── 16-international-seo.md
└── 17-review-schema.md
```

## Customize them

These prompts are starting points. For best results:

- **Add your domain** where you see placeholder references
- **List your actual pages** in sitemap and robots.txt prompts
- **Specify your tech stack** if it differs from React/Next.js
- **Include your brand colors** in the OG image prompt
- **Add your entity types** in the structured data prompts

## Tech stack assumptions

The prompts assume a modern JS/TS stack, but most adapt easily:

- **Framework:** React, Next.js, or any SPA
- **Helmet:** react-helmet-async (swap for your framework's head manager)
- **Backend:** Supabase edge functions (swap for Vercel, Cloudflare Workers, etc.)
- **Language:** TypeScript preferred, works with JavaScript too

## Contributing

Found a way to improve a prompt? PRs welcome.

- Keep prompts generic (no hardcoded domains or project-specific details)
- Test the prompt with at least one AI assistant before submitting
- Follow the existing format and naming conventions

## License

MIT — use these prompts however you want, commercially or otherwise.

---

Built by [SOMO Software](https://somo-tech.com) — custom software development powered by AI.
