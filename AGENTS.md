# AGENTS.md

## Overview
This is a Jekyll-based personal portfolio site hosted on GitHub Pages at `evias.be`. The site is built and deployed automatically when changes are pushed to the `main` branch (via GitHub Pages default workflow).

## Key directories and structure

- `_config.yml` — Jekyll configuration; defines site title, remote theme (portfolYOU), collections (projects, posts), and plugins (jemoji)
- `_posts/` — Blog posts with front matter (date prefix required: `YYYY-MM-DD-Title.md`)
- `_projects/` — Portfolio projects; each is a collection item with front matter and markdown content
- `_data/` — YAML data files for timeline, skills, social media (auto-loaded as site.data.*)
- `pages/` — Static pages: blog.html, projects.html, tags.html, hire-me.md, sponsor-me.md, privacy-policy.md, etc.
- `assets/` — Images and static files (CSS/JS handled by remote theme)

## Important notes for agents

### Front matter conventions
- **Posts** (in `_posts/`): Require `---` delimiters, `title`, `tags`, `style`, `color`, `description`, and optional `external_url` (links to Medium or GitHub)
- **Projects** (in `_projects/`): Require `name`, `tools` (list), `image` (URL), `description`; content is rendered below front matter
- **Pages** (in `pages/`): Vary by type (some are .html collections, some are .md with front matter)

### Jekyll quirks and gotchas
- **Filenames matter**: Post files must follow `YYYY-MM-DD-*.md` to be recognized as blog entries
- **Theme limitations**: Remote theme is `YoussefRaafatNasry/portfolYOU`; CSS/JS are not in this repo; customizations are limited to config and front matter
- **Markup parsing**: Recent commits show fixes for Jekyll markdown parsing issues with divs and links; avoid wrapping content in `<div>` tags and prefer markdown links `[text](url)` over HTML `<a>` tags
- **Emoji support**: Plugin `jemoji` is enabled in `_config.yml`
- **No build step**: Unlike most web projects, there is no `npm install`, `make`, or `bundle install` workflow visible in recent commits; GitHub Pages handles Jekyll build automatically

### Content conventions (from recent commits)
- Use markdown link syntax `[text](url)` instead of HTML `<a>` tags
- Avoid `<div>` wrappers; let Jekyll/theme handle layout
- Keep descriptions concise; Jekyll theme renders them with truncation

### Deployment
- Site is auto-deployed on every push to main via GitHub Pages
- CNAME record points to `evias.be`
- No manual deploy steps required

## No tests, CI, or lint
This repo has no test suite, linter, or CI pipeline. Changes are not validated before merge.

## Recent pattern
Commits are typically content updates (new posts, project descriptions) or markup/parsing fixes. Structure changes are rare.
