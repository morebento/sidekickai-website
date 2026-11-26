# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single static `index.html` — the one-page site for Sidekick AI. No build step, no dependencies, no framework.

## Deployment

Hosted on GitHub Pages, deploying automatically on push to `main`. Drop `index.html` onto any static host to deploy elsewhere.

`_config.yml` keeps `CLAUDE.md`, `instructions.md` and `README.md` out of the published site. Add any new working notes to its `exclude` list.

`instructions.md` is the original June 2026 spec; where it differs from this file, this file is current.

## Constraints

- All CSS lives in a `<style>` block in `<head>` — no external stylesheet.
- No JavaScript.
- Font loaded via Google Fonts `<link>`.
- No personal names and no contact details anywhere on the website.
- `noindex` meta tag stays in place until the product is ready for public discovery.

## Design

- Font: Playfair Display (serif). Fallback: Georgia, serif.
- Colour palette — background: `#EDEAE3` (warm parchment); wordmark: `#252220`; "AI" in wordmark: `#5C574F`; tagline: `#4A453E`; rule: `#C0B8AD`; date stamp: `#9A9189`. Muted tones throughout — no stark black or white.
- Wordmark renders as `Sidekick <em>AI</em>` — "AI" is italicised and set in a lighter colour (`#5C574F`).
- A short horizontal rule (`width: 3rem`, `1px solid #C0B8AD`) separates the wordmark from the tagline.
- No byline or service list. Below the rule is a placeholder customer login (`.login`): email, password and a "Log in" button. It is decorative, with all fields and the button `disabled`, and must stay inert: no `<form>`, no `name` attributes, `type="button"`, so nothing typed is ever sent.
- A small uppercase date stamp (Georgia, `0.72rem`, `letter-spacing: 0.14em`) sits below the login in `#9A9189`.
- An abstract geometric composition (`.shape`, inline SVG, decorative and `aria-hidden`) uses only palette colours: overlapping circles, a triangle, a quarter curve and a diagonal line with a dot.
- Layout: flex-centred viewport, `max-width: 640px`, left-aligned text. Above 900px the shape sits to the right of the text; at 900px and below it stacks above the text, aligned right. The page may scroll on short screens.
- Font sizes use `clamp()` for fluid scaling: wordmark `clamp(2.2rem, 5.5vw, 4rem)`.
- Google Fonts weights loaded: `ital,wght@0,400;0,700;0,900;1,400`.
