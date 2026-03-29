# International / Multilingual SEO

Implement full international SEO for a multilingual site.

## Hreflang tags

- Add hreflang link elements for every language/region variant
- Include x-default for the fallback language
- Support language codes (en, es, fr) and language-region codes (en-US, en-GB) as needed

## URL structure

Pick one and implement consistently:

- Subdirectories: `/en/`, `/es/`, `/fr/` (recommended)
- Subdomains: `en.site.com`, `es.site.com`
- Query params: `?lang=en` (not recommended)

## Sitemaps

Either create per-language sitemaps or a single sitemap with hreflang annotations.

## HTML and headers

- Set the `html lang` attribute correctly per page
- Include `Content-Language` response header

## Localized SEO content

- Translate and localize meta titles and descriptions per language
- Don't just translate, adapt for local search intent

## Language detection and redirect

- Detect via Accept-Language header
- Optional geo-IP detection
- Always allow manual user override
- Never trap users in a language they didn't choose

## Language switcher component

- Links to the equivalent page in each language
- Indicates the currently active language
- Accessible markup
