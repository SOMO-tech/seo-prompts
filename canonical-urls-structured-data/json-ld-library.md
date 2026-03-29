# JSON-LD Structured Data Library

Create a library of TypeScript functions that generate JSON-LD structured data objects for common page types. Each function should return a ready-to-inject JSON-LD object.

## Schemas to support

### 1. Organization (homepage / about page)

- name, url, logo, sameAs (social profile URLs)
- contactPoint, address if applicable

### 2. WebSite (homepage)

- name, url, potentialAction with SearchAction for site search

### 3. WebPage (all pages)

- name, description, url, isPartOf

### 4. BreadcrumbList (every non-homepage page)

- Auto-generate from URL path or accept a custom hierarchy
- Proper position numbering

### 5. Article / BlogPosting

- headline, description, image, datePublished, dateModified
- author (Person), publisher (Organization with logo)
- articleSection, keywords

### 6. Product (e-commerce pages)

- name, description, image, sku
- offers: price, availability, currency
- aggregateRating, review

### 7. FAQPage

- Array of Question/Answer pairs
- Auto-generate from structured FAQ content

### 8. LocalBusiness (if applicable)

- name, address, telephone, openingHours
- geo coordinates

### 9. HowTo (tutorial/guide content)

- steps, totalTime, tools, supplies

## Multi-sche
