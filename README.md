# RP Project Lifecycle

**Videography Project Lifecycle Manager** — a PWA for planning every phase of a video production, from first insight through delivery.

Built for [Rubinstein Productions](https://github.com/risaac09).

**Live:** [risaac09.github.io/rp-lifecycle](https://risaac09.github.io/rp-lifecycle/)

## What It Does

A structured 10-phase template for videography projects:

| Phase | Name |
|-------|------|
| 00 | Creative Brief |
| 01 | Pre-Production |
| 02 | Emotion & Image |
| 03 | Color Science |
| 04 | Film Theory |
| 05 | Grade Workflow |
| 06 | Plugins & Tools |
| 07 | Production Checklist |
| 08 | Delivery |
| 09 | Self-Direction / Quantum Mirror |

Each phase contains specialized fields, checklists, tables, and reference material tailored to a professional videography workflow — shot lists, camera settings, color pipelines, editing grammar, gear checklists, and more.

## Features

- **Multiple Projects** — Save and switch between projects, all stored in localStorage
- **Version History** — Snapshot any point in your project and restore later
- **AI Prefill** — Describe your project in a few lines and Claude populates the lifecycle fields via the Anthropic API
- **Project Dashboard** — Overall progress bar, per-phase completion, field stats
- **Export / Import** — Single project or full backup as JSON
- **Keyboard Shortcuts** — Press `?` to see all hotkeys (Cmd+S save, Cmd+K search, 1-0 phase nav, arrow keys, etc.)
- **Project Search** — Filter projects by name or client
- **Drag Reorder** — Reorder shot list rows by dragging
- **Mobile-First** — Bottom tab bar, swipe between phases, touch-optimized targets
- **Offline Support** — Service worker caches the app for offline use
- **Print Styles** — Clean print layout with all phases expanded

## Tech

Single-file vanilla JS PWA. No build step, no dependencies, no framework.

- `index.html` — the entire app (HTML + CSS + JS)
- `sw.js` — service worker for offline caching
- `manifest.json` — PWA manifest
- `icon-192.png` / `icon-512.png` — app icons

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `1`-`0` | Jump to phase 0-9 |
| `Left` / `Right` | Previous / next phase |
| `Cmd+S` | Save project |
| `Cmd+N` | New project |
| `Cmd+K` | Search projects |
| `Cmd+B` | Toggle sidebar |
| `Cmd+D` | Dashboard overview |
| `Cmd+I` | AI Prefill |
| `?` | Keyboard shortcuts |
| `Esc` | Close modal / sidebar |

## Deploy

Push to `main` — GitHub Pages serves from the root.

## License

MIT
