# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GreenSeal.dev is a Jekyll static site for a sustainability consulting company (GreenSeal Lda., Portugal). It promotes Green Software Practices (GSP) certification and consulting services. Hosted on GitHub Pages.

## Build Commands

```bash
bundle install            # Install Ruby dependencies
bundle exec jekyll serve  # Build and serve locally (http://localhost:4000)
bundle exec jekyll build  # Production build (output in _site/)
```

No test framework is configured.

## Architecture

**Stack:** Jekyll + Bootstrap 5.3.2 + SCSS, hosted on GitHub Pages via the `github-pages` gem.

### Layout Hierarchy

`base.html` (HTML shell, analytics, SEO meta) → `default.html` (header/footer/nav) → page-specific layouts (`home.html`, `service.html`, `blog.html`, `gsp.html`, `certified-company.html`, `team.html`, etc.)

### Collections (defined in `_config.yml`)

- **`_services/`** — Service offerings. Sorted by `weight` frontmatter. Output to `/services/`.
- **`_team/`** — Team members. Files prefixed with `_` are drafts/templates.
- **`_certified/`** — GSP-certified organizations. Permalink: `/gsp/certified/:name/`.
- **`/blog/`** — Blog posts. Date-prefixed filenames (`YYYY-MM-DD-slug.md`), layout `blog`.

### Data-Driven Content (`_data/`)

- `menus.yml` — Main and footer navigation menus (items have `weight` for ordering).
- `certification_levels.yml` — GSP certification tier definitions.
- `contact.yml` — Contact details used in templates.
- `social.json` — Social media links.
- `seo.yml` — SEO metadata.

### Styles (`_sass/` + `assets/css/style.scss`)

`style.scss` is the entry point — defines color variables, imports a selective subset of Bootstrap 5 (many components are commented out), then custom component and page SCSS files.

**Brand colors:** Primary `#427F69`, Primary Dark `#2C4436`, Secondary `#A3BDB3`.
**Fonts:** Helvetica/Arial (body), Playfair Display via Google Fonts (headings).

### JavaScript

Minimal — only `assets/js/scripts.js` handling mobile hamburger menu toggle. No build tooling or bundler.

## Content Conventions

### Adding a Service

Create a `.md` file in `_services/` with frontmatter: `title`, `weight` (sort order), `summary`, `date`. Layout defaults to `service` via `_config.yml`.

### Adding a Blog Post

Create `/blog/YYYY-MM-DD-slug.md` with frontmatter: `title`, `layout: blog`, `date`, `author`, `image`.

### Adding a Certified Organization

Create a `.md` file in `_certified/` with relevant frontmatter. Layout defaults to `certified-company`. Permalink pattern: `/gsp/certified/:name/`.

### Navigation

Edit `_data/menus.yml`. Items need `name`, `url`, and `weight` fields.

## Key Details

- Files prefixed with `_` in collections (e.g., `_consulting.md`, `_sage-kirk.md`) are drafts/templates and not output by Jekyll.
- The GSP section (`/gsp/`) has its own sub-navigation via `_includes/gsp-nav.html`.
- Cookie consent is opt-in (analytics denied by default). See `_includes/cookie-banner.html` and `_layouts/base.html`.
- Plugins: `jekyll-environment-variables`, `jekyll-sitemap`.
