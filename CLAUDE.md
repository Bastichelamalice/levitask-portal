# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Status

This is an early-stage static HTML project — no build system, no package manager, no framework. Open HTML files directly in a browser or use any static file server (e.g. `python3 -m http.server`).

## Architecture

Two standalone HTML pages with all CSS inlined in `<style>` tags:

- **product-knowledge.html** — science/research content page with a design-system layout, study cards, stats grid, and a dark/light color mode toggle
- **training-certification.html** — two-column layout with a fixed 240px sidebar for module navigation, main content area, and certification status tracking (locked / in-progress / complete)

### Design System

Defined via CSS custom properties at the top of each file:

| Token | Value | Use |
|---|---|---|
| `--color-bg` | `#0a0a0a` | Page background |
| `--color-surface` | `#161616` / `#1e1e1e` | Card/panel backgrounds |
| `--color-accent` | `#e8622a` | Primary orange accent |
| `--color-accent-green` | `#4a7c59` / `#6dbf86` | Secondary green |
| `--color-text` | `#f0ece4` | Primary text (cream) |
| `--color-text-secondary` | `#8a8480` | Muted text |

Fonts: **Cormorant Garamond** (serif headings) and **DM Sans** (body), loaded from Google Fonts.

Both pages share the same visual language — when adding new pages or components, mirror the CSS variable names and typographic scale already established.
