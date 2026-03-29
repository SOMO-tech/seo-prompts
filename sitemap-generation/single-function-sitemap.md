# Single Function Sitemap

Create a single Supabase edge function at `/functions/v1/sitemap` that outputs a complete sitemap with up to 50,000 URLs.

## The function should

- Query all dynamic entities from Supabase
- Merge with hardcoded static page URLs
- Return one `<urlset>` XML document containing every URL
- Pull lastmod from each record's `updated_at` column
- Set changefreq and priority appropriate to each content type
- Cache the result for 1 hour
- Return `Content-Type: application/xml`
- Use the production canonical domain throughout

## Static pages

- [list them]

## Dynamic entities

- [list entity types and their URL patterns]

## Constraints

Keep total URL count under the 50,000 sitemap protocol ceiling.

## Sitemap index

Create a static sitemap.xml in `public/` using `<sitemapindex>` that references this edge function.
