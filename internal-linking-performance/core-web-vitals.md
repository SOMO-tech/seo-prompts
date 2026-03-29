# Core Web Vitals & Performance

Optimize the site for Core Web Vitals and page speed to improve SEO rankings.

## Images

- Use next/image or equivalent with native lazy loading
- Serve WebP with format fallbacks
- Always include width and height attributes to prevent layout shift (CLS)
- Use blur-up placeholders for above-the-fold LCP images

## Fonts

- Set `font-display: swap` on all custom fonts
- Preload critical font files
- Subset fonts to only the character sets needed
- Consider a system font stack for body text

## JavaScript

- Code-split by route
- Defer all non-critical scripts
- Audit and remove unused dependencies

## CSS

- Inline critical above-the-fold CSS
- Purge unused CSS rules
- Avoid CSS that causes layout shifts

## Monitoring

- Log Core Web Vitals (LCP, INP, CLS) in production
- Set up alerts for performance regressions

## Resource hints

- `<link rel="preconnect">` for critical third-party origins
- `<link rel="prefetch">` for likely next navigations
- `<link rel="preload">` for critical assets (fonts, hero image)

## Build-time audit

Create a checklist that audits each of these and reports issues.
