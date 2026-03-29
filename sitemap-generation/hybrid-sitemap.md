# Hybrid Sitemap

Create a sitemap system for a site that combines static pages with a small amount of dynamic content stored in Supabase (under 1,000 items per entity).

## Edge function

Build an edge function at `/functions/v1/sitemap` that:

- Queries each dynamic entity from Supabase in a single call
- Merges results with a hardcoded list of static page URLs
- Returns the full sitemap as valid XML
- Caches the response for 1 hour
- Uses the site's canonical domain for all URLs

## Static pages to include

- [list your routes]

## Dynamic entities to include

- [list your entity types and URL patterns]

## URL entries

Each `<url>` entry must contain:

- `loc` (full canonical URL)
- `lastmod` (from the database updated_at field, or a fixed date for static pages)
- `changefreq` (matched to content type)
- `priority` (matched to page importance)

## Sitemap index

Create a static sitemap.xml in the `public/` folder that uses a `<sitemapindex>` pointing to the edge function URL.
