# Standard Robots.txt

Create a robots.txt file for the public root of my site.

## Rules

- Allow all major search engine crawlers full access to public content
- Disallow crawling of:
  - `/api/*` (backend routes)
  - `/admin/*` (admin panel)
  - `/_next/*` (framework internals, if applicable)
  - `/private/*` (any protected routes)
  - Query strings that create duplicate content (`?ref=`, `?utm_*`, etc.)

## Sitemap

Point to the sitemap at `https://yourdomain.com/sitemap.xml`

## Additional directives

- Add a crawl-delay directive for aggressive bots if needed
- Specific bot rules:
  - Googlebot: allow all public content
  - Bingbot: allow all public content
  - AI training bots (GPTBot, ChatGPT-User, CCBot): block

## Format

Use the standard syntax:
```
User-agent: [bot]
Allow: /
Disallow: /path
Sitemap: https://yourdomain.com/sitemap.xml
```
