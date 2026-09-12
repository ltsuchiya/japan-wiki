# Japan Relocation Wiki — Claude Code Context

This is a personal knowledge wiki built with [Quartz 5](https://quartz.jzhao.xyz), tracking research for a Japan relocation. It deploys to GitHub Pages at `ltsuchiya.github.io/japan-wiki`.

## Content structure

Processed wiki pages live under `content/`. The folder layout is:

```
content/
  cars/          # importing, buying, or registering a vehicle in Japan
  real-estate/   # renting, buying property, neighborhoods
  taxes/         # income tax, import duties, residency rules
  phones/        # SIM cards, carrier plans, porting numbers
  timeline/      # notes tied to a specific stage of the relocation process

inbox/           # raw/unprocessed research notes — repo root, gitignored
```

`inbox/` is a staging area at the repo root (not inside `content/`). Drop raw notes there and run `/process-inbox` to file them. It is gitignored — inbox contents are not committed.

## Frontmatter schema

Every page in `content/` (except `inbox/`) must have this frontmatter:

```yaml
---
title: <Page Title>
tags: [<topic>, <optional sub-topic>]
date: <YYYY-MM-DD created>
updated: <YYYY-MM-DD last modified>
---
```

- `tags[0]` should match the parent folder name (e.g. `cars`, `taxes`).
- Do not repeat the `title` as an `# H1` in the body — the title frontmatter renders as the page heading.

## Page conventions

- **Filenames**: kebab-case, descriptive — `importing-a-us-car.md`, not `notes1.md`.
- **One concept per page**: prefer several focused pages over one giant topic page.
- **Wikilinks**: use `[[page-name]]` syntax to link related pages. Cross-topic links are encouraged when content overlaps (e.g. a car-import page linking to an import duties taxes page).
- **Comparisons**: use markdown tables for any side-by-side comparisons (Japan vs. US rules, option A vs. B, etc.).
- **References**: every page should end with a `## References` section linking to the reputable sources the information is drawn from (official government sites, authoritative guides, etc.). A page without sources can't be validated.
- **No trailing slashes** in internal links — Quartz outputs `.html` files; a trailing slash won't resolve correctly on GitHub Pages.
- Do not commit generated build output (`public/`). Only markdown, config, and workflow files are tracked.

## Key files

| File | Purpose |
|------|---------|
| `quartz.config.yaml` | Site config — title, baseUrl, plugins |
| `.github/workflows/deploy.yml` | Builds and deploys to GitHub Pages on push to `main` |
| `content/` | All wiki pages |

## Available slash commands

- `/process-inbox` — reads files in `content/inbox/`, restructures them into proper wiki pages, and removes the originals.
