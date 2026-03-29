# Paginated Sitemap

Build a paginated sitemap system using Supabase edge functions for a site with more than 50,000 URLs.

## Main function

Create an edge function at `/functions/v1/sitemap` that:

- Queries entity counts from Supabase to calculate pagination
- Returns a `<sitemapindex>` listing sub-sitemap URLs like `/functions/v1/sitemap-posts?page=1`, `?page=2`, etc.
- Includes one entry per entity type per page (1,000 URLs per page)
- Caches the response for 1 hour
- Returns `Content-Type: application/xml`

## Per-entity functions

For each entity type (e.g. `/functions/v1/sitemap-posts`):

- Accept a `?page=N` query parameter
- Query Supabase for that batch of 1,000 records
- Return a `<urlset>` XML with those URLs
- Include lastmod from `updated_at`
- Set appropriate changefreq and priority
- Use the production canonical domain

## Entity types

- [list them with URL patterns]

## Sitemap index

Create a static sitemap.xml in `public/` using `<sitemapindex>` pointing to the main edge function.
