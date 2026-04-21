# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll-based academic personal website for Ziteng Ji, built on the Academic Pages template (fork of Minimal Mistakes theme). Deployed to GitHub Pages at `https://zitengji0618.github.io/academicpage`.

## Development Commands

```bash
# Install dependencies
bundle install

# Start local dev server (does NOT auto-reload _config.yml changes — restart required)
jekyll serve -l -H localhost

# Docker alternative
docker build -t jekyll-site .
docker run -p 4000:4000 --rm -v $(pwd):/usr/src/app jekyll-site

# Build/minify JavaScript
npm run build:js
```

## Architecture

**Static site generator**: Jekyll with Kramdown (GFM) markdown, deployed via GitHub Pages.

**Content collections** (defined in `_config.yml`):
- `_publications/` — Research papers. Files named `YYYY-MM-DD-title-number.md`. Frontmatter: title, category (books/manuscripts/conferences), date, venue, paperurl, teaser.
- `_portfolio/` — Project showcase (mix of `.md` and `.html`). Frontmatter: title, excerpt, area.
- `_talks/` — Conference presentations. Frontmatter: title, venue, date, location, type.
- `_teaching/` — Course pages.
- `_posts/` — Blog posts.

**Pages**: `_pages/` contains top-level site pages. The homepage is `_pages/about.md` (permalink: `/`).

**Templates**: `_layouts/` (default, single, talk, archive) and `_includes/` (reusable HTML partials like author-profile, navigation, footer).

**Styling**: `_sass/` contains modular SCSS files compiled to compressed CSS.

**Data files**: `_data/navigation.yml` controls header nav. `_data/authors.yml` for author profiles. `_data/ui-text.yml` for localized UI strings.

**Site config**: `_config.yml` holds site metadata, author info, collection definitions, and plugin config. The `baseurl` is `/academicpage`.

**Publication categories** in `_config.yml` under `publication_category`: books, manuscripts (journal articles), conferences.

## Content Generation Utilities

`markdown_generator/` contains Python scripts and Jupyter notebooks that auto-generate collection markdown files from structured data:
- `publications.py` / `publications.ipynb` — from `publications.tsv`
- `talks.py` / `talks.ipynb` — from `talks.tsv`
- `PubsFromBib.ipynb` — from BibTeX
- `talkmap.py` / `talkmap.ipynb` — generates geographic visualization of talk locations
