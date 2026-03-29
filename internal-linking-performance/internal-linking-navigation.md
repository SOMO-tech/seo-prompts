# Internal Linking & Navigation SEO

Improve the site's internal linking and semantic structure for SEO.

## Breadcrumb component

- Generates breadcrumbs from the URL path or a custom hierarchy
- Injects JSON-LD BreadcrumbList schema
- Uses a `<nav>` element with `aria-label="Breadcrumb"`
- Links all items except the current page

## Heading hierarchy audit

- Enforce a single `<h1>` per page
- No skipped heading levels (e.g. h1 → h3 with no h2)
- Log a dev-mode warning when violations are detected

## Semantic HTML5 structure

- `<header>` for the site header
- `<nav>` for navigation (use distinct aria-labels when there are multiple navs)
- `<main>` for primary content
- `<article>` for self-contained content blocks
- `<aside>` for sidebars
- `<footer>` for the site footer

## Related content component

- Displays 3 to 5 related pages or posts
- Uses descriptive anchor text (never "click here")
- Includes a brief description for each link

## Internal link hygiene

- Descriptive anchor text everywhere
- Full paths, not just fragments
- No orphan pages (every page reachable from at least one other page)
