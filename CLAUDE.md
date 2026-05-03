# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the marketing/landing page for [EmpiriQal.ai](https://empiriqal.ai) — a static single-page site with no build tooling, no framework, and no dependencies beyond Google Fonts.

## Development

Open `index.html` directly in a browser — no server or build step required.

## Architecture

Everything lives in a single file: [index.html](index.html).

- **CSS** — inline `<style>` block using CSS custom properties (`--crimson`, `--ink`, `--off-white`, etc.) for the design system. Typography uses Cormorant Garamond (serif) and Instrument Sans (sans-serif) from Google Fonts.
- **HTML** — sections in order: nav, hero, problem, solution, audience, traction, founder, contact, footer.
- **JS** — two small inline scripts at the bottom: an IntersectionObserver for `.reveal` scroll animations, and a contact form handler that opens a `mailto:` link (no backend).

## Deployment

Hosted on GitHub Pages. The `CNAME` file points the custom domain to `empiriqal.ai`. Pushing to `main` deploys automatically.
