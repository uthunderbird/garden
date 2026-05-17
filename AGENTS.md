# AGENTS.md

## Project intent
Keep this project as a curated publication layer rather than a dumping ground for all writing-related material.

## Operating rules
- Preserve the distinction between curated content and upstream drafting systems.
- Do not merge `garden` with `writing-lab` or `editorial-lab`.
- Prefer adding section maps and explicit publication rationale before restructuring content.
- Update [INDEX.md](./INDEX.md) when new canonical pages appear.
- Keep the curation threshold high: notes promoted here should already have clear framing, context, and a reason to live in the public-facing layer.

## File handling
- Public-facing content belongs under `content/`.
- Project-level coordination docs belong at the project root.
- Do not place private planning or raw notes inside `content/`.

## Decision rules
- If uncertain whether a text belongs here or in a writing project, prefer leaving it in the writing project and linking it later.
- Avoid creating duplicate copies of texts that are still actively evolving elsewhere.
- Do not move half-processed fragments here; if a note belongs in `garden`, it should already be contextualized and reachable through curated navigation such as [INDEX.md](./INDEX.md).

## Frontmatter conventions

All content files use this standard frontmatter:

```yaml
title: "..."
description: "..."        # required for essays; optional for poems/notes
date: YYYY-MM-DD
tags: ["tag1", "tag2"]    # always array, never plain string
type: essay | note | poem | page | index   # metadata only — Quartz does not use this field for rendering or filtering without custom components
lang: ru | en
draft: true               # remove before publishing
translation_of: /path     # only if this is a translation
```

Notes on `type`:
- This field is a metadata convention for future use or custom components.
- Quartz does not currently filter or render differently based on `type`.
- Do not add `type` expecting visual differentiation on the site — it won't happen without a custom Quartz component.

Notes on `templates/`:
- Templates use Obsidian Templater syntax (`<% ... %>`).
- Always create new files via Templater — do not copy templates manually, or Templater syntax will appear as literal text.
- Templater plugin must be installed in Obsidian and pointed at the `templates/` folder.

## Content structure

- `content/evergreen/` — curated, published texts with clear framing. High curation bar.
- `content/notes/` — situational, chronological, or draft material. Lower bar. May be incomplete.
- `content/templates/` — Obsidian Templater templates. Not published (in `ignorePatterns`).

## Continuity
- Read [STATE.md](./STATE.md) first.
- Then read [NEXT.md](./NEXT.md).
- Use [INDEX.md](./INDEX.md) for navigation.
