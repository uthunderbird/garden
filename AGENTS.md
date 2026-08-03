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

## Editorial discipline
- Не переписывать существующие тексты без прямого разрешения автора, если текст уже существует в `content/` и отличается только редактурой/стилистикой.
- Если нужно изменить черновик, сначала зафиксируй цель правки по содержанию, затем выполняй точечные правки по согласованному списку.

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

## Publication procedure ("опубликуй")

When the author says "опубликуй" / "publish" about a garden text, this means the FULL procedure, not just flipping a flag. Run every step:

1. **Decide note vs evergreen.** Curated, well-framed, standalone-meaningful → `evergreen/` (high bar). Situational/chronological/incomplete → stays `notes/`. A continuation of an evergreen text goes to evergreen too.
2. **Remove the `draft` flag.** Delete the `draft:` line entirely (published siblings have no `draft:` line), don't just set `false`.
3. **Move if needed.** If the decision is evergreen but the file is in `notes/`, `git mv` it into `content/evergreen/`.
4. **Cross-links.** Add the links the text earns — at minimum, if it continues/answers another published text, add a FORWARD link from that text to this one (the back-link usually already exists), so the arc is navigable both ways.
5. **Index entry.** Add the page to the relevant category list in `content/evergreen/index.md` (currently the only category index; place it near related pieces, e.g. adjacent to part 1 of an arc). Also update root `INDEX.md` if the page is canonical enough to belong there.
6. **Commit scope discipline.** Stage and commit ONLY the publication-related files. Never sweep in unrelated uncommitted changes that happen to be in the working tree.
7. **Commit and push** to `main` (direct commit to `main` is the normal publication path for the garden).
8. **Verify deployment and cache.**
   - The site is built by the `garden-site` repository. A push to `garden` triggers a GitHub Action that updates the submodule in `garden-site` and deploys to GitHub Pages (`dus.garden`).
   - **Important:** The server uses `cache-control: max-age=600`. The browser will aggressively cache pages for 10 minutes. If changes do not appear immediately, do a hard refresh (`Cmd + Shift + R`), use Incognito, or check headers directly via `curl -I https://dus.garden/path`.
   - **Local pipeline:** The local build environment is located at `~/Projects/garden-site/`. To sync it manually, run `git pull && git submodule update --remote content` in that directory.

## Continuity
- Read [STATE.md](./STATE.md) first.
- Then read [NEXT.md](./NEXT.md).
- Use [INDEX.md](./INDEX.md) for navigation.
