# Instructions for the AI

This vault is a personal knowledge base maintained by an AI. It can hold any number of topics; mountains (ski
tours and hikes) is the first one. Write everything in English.

## Layout

- `Sources/` — raw material: clipped articles, guidebook excerpts, own trip reports, course notes. **Never edit or
  delete a source.** New sources are named `YYYY-MM-DD-slug.md` (the date the material was added).
- `Wiki/` — pages you write and keep up to date:
  - `entities/` — things with a name: `tours/`, `regions/`, `huts/` (later also people, tools, …).
  - `concepts/` — ideas and principles (e.g. spring snow, aspect).
  - `topics/` — hub pages for a subject area, plus logs such as the tour log.
  - `sources/` — one summary page per file in `Sources/`.
  - `synthesis/` — comparisons and analyses across pages.
  - `index.md` — catalog of all pages; `log.md` — what was ingested or changed, newest first.

## Page format

Every wiki page starts with YAML frontmatter:

```yaml
type: entity | concept | topic | source | synthesis
tags: [ ... ]
updated: YYYY-MM-DD
sources: [ ... ]   # files in Sources/ that back this page
related: [ ... ]   # other wiki pages
```

Tour pages add: `kind: tour`, `activity: ski-tour | hike`, `region`, `start_m`, `summit_m`, `aspect`, `glacier`
(true/false), `difficulty`, `best_months` (list of three-letter months) and `done` (date of the last time done, or
`null`). Keep `done` in sync with `Wiki/topics/tour-log.md`.

Link pages with `[[wikilinks]]`. If a page you link to doesn't exist yet, leave the link: it marks a gap.

## Workflows

- **Ingest** a new source: write `Wiki/sources/<slug>.md`, create or update the entity and concept pages it
  touches, add new pages to `Wiki/index.md`, add an entry on top of `Wiki/log.md`. Note contradictions with
  existing pages on both pages instead of overwriting.
- **Answer a question:** start from `Wiki/index.md`, read the relevant pages, answer with `[[links]]` to the pages
  you used. Say what the vault doesn't know. You have no web access: for current conditions (snow, avalanche
  danger, hut opening) tell the user to check the official bulletins.
- **Lint:** report dead links, orphan pages, pages without sources, `done` fields that disagree with the tour log,
  and contradictions; fix only after the user agrees.

Never commit or push; the user reviews your changes and commits them in the app.
