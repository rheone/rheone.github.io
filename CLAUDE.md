# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a static personal website and portfolio repository for Robert H. Engelhardt, deployed as a GitHub Pages site at https://rheone.github.io/. The site is built with vanilla HTML, CSS, and JavaScript (no build tools or frameworks required).

## Architecture & Structure

**Core Pages:**
- `index.html` - Main landing page with bio, social links, and navigation
- `resume.html` - Detailed resume page with qualifications and experience
- `projects.html` - Portfolio of open-source projects
- `attributions.html` - Third-party library and resource credits
- `hobbies.html` - Hidden page (commented out in nav)

**Styling:**
- `styles/site.css` - Minimal custom CSS (only monospace font override)
- Bootstrap 5.3.3 (CDN) - Primary UI framework
- Fira Code font (CDN) - Monospace font for code/terminals
- Font Awesome 6.7.2 (CDN) - Icons throughout the site

**Data:**
- `resume.md` - Markdown source for resume content (mirrors resume.html)
- `resume.old.md` - Previous version of resume
- `images/` - Avatar and other image assets
- `humans.txt`, `robots.txt`, `sitemap.xml` - SEO/discovery files

**Static Hosting:**
- GitHub Pages (master/main branch auto-deploys)
- No build process required
- Direct HTML/CSS deployment

## Development Workflow

Since there's no build tool, changes are made directly to source files:

1. **HTML Pages:** Edit `.html` files directly and test in browser
2. **Styling:** Add CSS to `styles/site.css` (currently only 3 lines)
3. **Resume Updates:** Keep both `resume.md` (source of truth) and `resume.html` (rendered version) in sync
4. **Testing:** Open `.html` files in a browser or use `python -m http.server 8000` for local preview

## Key Technologies & Dependencies

All dependencies are served via CDN (no npm/package.json):
- **Bootstrap 5.3.3** - Responsive layout and components
- **Font Awesome 6.7.2** - Icon library
- **Fira Code 6.2.0** - Monospace font

No local build, test, lint, or dev servers required.

## Deployment

The repository is a GitHub Pages site. Any commits to the main branch automatically deploy to https://rheone.github.io/. Verify changes locally before pushing.

## Content Maintenance Notes

- Resume content is maintained in both Markdown (`resume.md`) and HTML (`resume.html`). Keep them in sync when updating professional experience or qualifications.
- Social links in `index.html` are hardcoded; update them if contact information changes.
- The `projects.html` page references open-source projects; ensure links remain current.
