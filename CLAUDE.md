# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static portfolio website for Marc Bernet (marcbernet.com), deployed via GitHub Pages. No build process — all files are ready to serve as-is.

## Local Development

```bash
docker-compose up
# Serves at http://localhost:8080
```

## Architecture

The entire website lives in `docs/` (GitHub Pages root). Four HTML pages share a consistent layout using Bootstrap 3 + jQuery.

- `docs/css/style.css` — all custom styles
- `docs/js/script.js` — menu toggle and portfolio shuffle/filter logic
- `docs/CNAME` — points GitHub Pages to marcbernet.com

### Photography page
`docs/photography.html` uses **jQuery Shuffle** (`jquery.shuffle.min.js`) for filterable grid layout and **Lightbox Plus jQuery** (`lightbox-plus-jquery.js`) for modal image viewing.

## Deployment

Push to `main` → GitHub Pages auto-deploys from `docs/`.
