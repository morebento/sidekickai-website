# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single static `index.html` — the placeholder page for Sidekick AI. No build step, no dependencies, no framework.

## Deployment

Hosted on GitHub Pages, deploying automatically on push to `main`. Drop `index.html` onto any static host to deploy elsewhere.

## Constraints

- All CSS lives in a `<style>` block in `<head>` — no external stylesheet.
- No JavaScript.
- Font loaded via Google Fonts `<link>`.
- `noindex` meta tag stays in place until the product is ready for public discovery.

## Design

- Font: Playfair Display (serif). Fallback: Georgia, serif.
- Colour palette — background: `#EDEAE3` (warm parchment); wordmark: `#252220`; "AI" in wordmark: `#5C574F`; tagline: `#4A453E`; rule: `#C0B8AD`; date stamp: `#9A9189`. Muted tones throughout — no stark black or white.
- Wordmark renders as `Sidekick <em>AI</em>` — "AI" is italicised and set in a lighter colour (`#5C574F`).
- A short horizontal rule (`width: 3rem`, `1px solid #C0B8AD`) separates the wordmark from the tagline.
- Tagline is italic. A small uppercase date stamp (Georgia, `0.72rem`, `letter-spacing: 0.14em`) sits below in `#9A9189`.
- Layout: flex-centred viewport, `max-width: 640px`, left-aligned text.
- Font sizes use `clamp()` for fluid scaling: wordmark `clamp(2.2rem, 5.5vw, 4rem)`, tagline `clamp(1rem, 2.5vw, 1.25rem)`.
