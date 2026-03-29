# Article SEO Extension

Extend the base SEO component to fully support article and blog post pages.

## Additional meta tags

- `article:published_time`
- `article:modified_time`
- `article:author`
- `article:section`
- `article:tag` (support multiple tags)

## Article JSON-LD schema

Include the following fields:

- headline, description, image
- datePublished, dateModified
- author as a Person schema
- publisher as an Organization schema (include logo)
- mainEntityOfPage reference

## Extra features

- Estimate reading time from the post's word count
- Support multiple co-authors
- Auto-generate breadcrumbs based on the article's category hierarchy
