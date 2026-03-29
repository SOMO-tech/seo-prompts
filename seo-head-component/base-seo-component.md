# Base SEO Component

Build a reusable SEO component using react-helmet-async that can be dropped into any page of my React app. It should:

## Props (all optional with smart defaults)

- `title` → automatically appends " | My Site Name" unless overridden
- `description` → capped at 160 characters, falls back to a global default
- `keywords` → accepts a string array
- `canonicalUrl` → if omitted, auto-generates from the current route path
- `ogImage` → falls back to a site-wide default image
- `ogType` → defaults to "website", accepts "article" for blog content
- `noindex` → boolean flag, false by default
- `structuredData` → accepts a raw JSON-LD object for injection

## Meta tag coverage

- **Standard:** title, description, keywords, robots, viewport, charset
- **Open Graph:** title, description, image, url, type, site_name
- **Twitter Cards:** card type, title, description, image, site handle
- **Canonical:** link element

## JSON-LD structured data support

Built-in schema generators for:

- Organization (homepage)
- WebPage (default on all pages)
- Article / BlogPosting (blog content)
- Product (product pages)
- BreadcrumbList
- FAQPage

Include utility functions that generate the correct schema for each page type automatically.

## Setup

Wrap the root App component with `HelmetProvider`.

Use my production domain as the base for all absolute URLs. Add full TypeScript typings for the props interface.
