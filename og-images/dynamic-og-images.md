# Dynamic OG Images

Build an API route or edge function at `/api/og` that generates dynamic Open Graph images for social sharing.

## Input (query parameters)

- `title` (required)
- `description` (optional)
- `type` ("article", "product", "default")
- `image` (optional background or featured image URL)

## Output

- 1200×630 px PNG image
- Site branding: logo, brand colors
- Dynamic title text that auto-sizes to fit the canvas
- Optional description line
- Gradient or branded background
- Optional composited featured image

## Technical requirements

- Use @vercel/og, Satori, or equivalent for server-side image rendering
- Cache generated images with appropriate headers
- Return `Content-Type: image/png`

## Edge cases to handle

- Very long titles → truncate with ellipsis
- Missing parameters → use sensible defaults
- Invalid image URLs → fall back to default background

## Pre-built templates

- Blog post: title + author name + publish date
- Product: title + price + product image
- Default: title + site name

## Integration

Update the SEO component to use this endpoint as the fallback OG image when no custom image is provided.
