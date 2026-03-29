# Static OG Images

Set up static Open Graph images for a site that already has pre-designed images.

## Directory structure

Create a `/public/og/` directory with:

- `default.png` (1200×630, site-wide fallback)
- `home.png` (homepage-specific)
- `[page-name].png` for each key page

## SEO component updates

Update the SEO component to:

- Check if a page-specific OG image exists in `/og/`
- Fall back to `default.png` if not
- Always use absolute URLs with the canonical domain

## Image requirements

- Exactly 1200×630 pixels
- Under 1 MB file size
- PNG or JPG format

## Build-time validation

Add a helper that validates OG images exist for all critical pages and warns about missing ones.

Based on the current site structure, list which pages should have custom OG images.
