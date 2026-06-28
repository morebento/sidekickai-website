build a website based on the spec below - it should only be a single index.html file 

# Sidekick AI — Placeholder Page Spec
## Overview
A single, static HTML page. No CMS, no framework, no dependencies. The page serves as a professional holding presence while the product is in development. It should feel like a confident company that knows exactly what it's doing — not a startup that hasn't launched yet.
---
## Page Structure
Single full-viewport page. No scrolling required on any standard screen size.
**Elements (top to bottom, vertically centred):**
1. **Logo / Wordmark** — "Sidekick AI" as styled text (no image asset needed). See Typography below.
2. **Horizontal rule** — short (`width: 3rem`), separating wordmark from tagline.
3. **Tagline** — one line, see copy below.
4. **Date stamp** — small, uppercase, muted. Current month and year (e.g. "June 2026").
5. *(Contact details to be added in a future iteration.)*
No navigation. No hero image. No background illustration. No social icons (unless Ben specifically requests later).
---
## Copy
**Wordmark:**
Sidekick <em>AI</em>

**Tagline:**
> Purpose-built AI tools for professionals.
---
## Typography
- **Font:** [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) loaded from Google Fonts (`ital,wght@0,700;0,900;1,400`). Fallback: `Georgia, serif`.
- **Wordmark:** `font-size: clamp(2.2rem, 5.5vw, 4rem)`, `font-weight: 900`, `letter-spacing: -0.025em`, `line-height: 1.0`. "AI" is italicised (`font-style: italic`, `font-weight: 700`) and set in a lighter colour (`#5C574F`).
- **Tagline:** `font-size: clamp(1rem, 2.5vw, 1.25rem)`, `font-weight: 400`, `font-style: italic`, `letter-spacing: 0.01em`, `line-height: 1.5`.
- **Date stamp:** `font-size: 0.72rem`, `font-family: Georgia, serif`, `letter-spacing: 0.14em`, `text-transform: uppercase`.
---
## Colour
| Token | Value | Usage |
|---|---|---|
| Background | `#EDEAE3` | Warm parchment |
| Wordmark | `#252220` | Near-black |
| "AI" in wordmark | `#5C574F` | Lighter, italicised |
| Tagline | `#4A453E` | Slightly softened |
| Rule | `#C0B8AD` | Muted separator |
| Date stamp | `#9A9189` | Very muted |

No stark black or white anywhere.
---
## Layout
- Content block centred both horizontally and vertically (`display: flex; align-items: center; justify-content: center; min-height: 100vh`).
- Inner content block: `max-width: 640px`, left-aligned text (not centred — left-aligned reads more confident for a B2B product).
- Generous padding on mobile: `padding: 2rem`.
---
## Behaviour
- Fully responsive. Looks correct on mobile, tablet, desktop.
- No animations, no transitions.
- No cookies, no tracking, no analytics (until Ben requests).
- No JavaScript required.
---
## Meta / SEO
```html
<title>Sidekick AI</title>
<meta name="description" content="Purpose-built AI tools for professionals.">
<meta name="robots" content="noindex">
```
`noindex` until ready to be discovered publicly.
---
## Deliverable
**Implementation constraint: plain HTML and CSS only. No frameworks, no build tools, no npm, no preprocessors.**
- Single `index.html` file.
- All CSS inline in a `<style>` block in the `<head>` — no external stylesheet.
- Font loaded via `<link>` to Google Fonts.
- No JavaScript.
- File should be deployable by dropping onto any static host (Netlify, GitHub Pages, Cloudflare Pages).
---
## Out of Scope
- Contact form / email capture
- Animation or scroll effects
- Multiple pages
- CMS integration
- Dark mode toggle

*These can be added in a future iteration.*
---
*Spec prepared June 2026. Contact Ben Moretti with questions.*
