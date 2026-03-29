# Canonical URL Handling

Implement robust canonical URL handling across the entire site.

## Canonical link tag

Add a canonical `<link>` element to every page via the SEO component.

## Scenarios to handle

- Query parameters: strip tracking params (`?utm_*`, `?ref=`) from the canonical
- Pagination: page 1 canonical = base URL, page 2+ includes the page param
- Trailing slashes: pick one convention (no trailing slash recommended) and enforce it
- Protocol: always https
- WWW vs non-www: pick one (non-www recommended), redirect the other
- Case: lowercase all URL paths

## Utility function

Build a `getCanonicalUrl(path, params)` function that:

- Constructs the full canonical URL from a relative path
- Strips unwanted query parameters
- Normalizes format (slash, case, protocol)

## Self-referencing canonical

Every page must include a self-referencing canonical.

## Pagination links

For paginated content, implement `rel="prev"` and `rel="next"` link elements (still used by Bing and others).
