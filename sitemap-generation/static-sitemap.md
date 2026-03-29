# Static Sitemap

Generate a sitemap.xml file for a fully static site with no database-driven pages.

## Requirements

- Place the file at the public root directory
- List every public page with its full canonical URL using https
- Set lastmod to the actual last-modified date (or today if unknown)
- Assign changefreq: daily for the homepage, weekly for main sections, monthly for rarely-updated pages
- Assign priority: 1.0 homepage, 0.8 primary sections, 0.6 subpages

## Pages to include

- / (homepage)
- [list your static routes here, e.g. /about, /pricing, /contact, /features, /blog]

## XML structure

Use proper XML formatting: declaration, urlset with xmlns namespace, correctly escaped URLs.

The output must validate against the sitemap protocol spec.
