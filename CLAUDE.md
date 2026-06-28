# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single static `index.html` — the placeholder page for Sidekick AI. No build step, no dependencies, no framework.

## Deployment

Drop `index.html` onto any static host (Netlify, GitHub Pages, Cloudflare Pages). No build command needed.

## Constraints

- All CSS lives in a `<style>` block in `<head>` — no external stylesheet.
- No JavaScript.
- Font (Inter) loaded via Google Fonts `<link>`.
- `noindex` meta tag stays in place until the product is ready for public discovery.
