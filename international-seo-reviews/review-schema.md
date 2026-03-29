# Review & Social Proof Schema

Implement structured data for reviews and ratings to enable rich results in search.

## AggregateRating schema

- ratingValue, bestRating, worstRating
- ratingCount, reviewCount
- itemReviewed (link to the product, organization, or service)

## Individual Review schema

- author, datePublished, reviewBody
- reviewRating (nested Rating schema)
- itemReviewed

## Reviews display component

- Renders user reviews visually
- Automatically generates the matching JSON-LD schema
- Calculates aggregate rating dynamically from review data

## Testimonials section

Display testimonials with proper Review schema markup.

## Star rating component

- Visual star display
- Screen reader accessible text
- Outputs schema-compliant data attributes
