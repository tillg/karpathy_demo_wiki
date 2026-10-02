# Instructions for the AI

This vault is a personal knowledge base maintained by an AI. It holds several unrelated topics — today
mountains (ski tours, hikes, via ferratas), coffee, and mathematics (topology) — and more will come. Write
everything in English.

## Layout

- `Sources/` — raw material: clipped articles, guidebook excerpts, own trip reports, course notes. **Never edit or
  delete a source.** New sources are named `YYYY-MM-DD-slug.md` (the date the material was added).
- `Wiki/` — pages you write and keep up to date:
  - `entities/` — things with a name, one subfolder per kind: `tours/`, `regions/`, `huts/`, `organizations/`
    (mountains); `origins/`, `varieties/`, `brewers/` (coffee); `mathematicians/`, `theorems/` (mathematics).
    Add a new subfolder when a new kind of thing appears.
  - `concepts/` — ideas and principles of any topic (e.g. spring snow, extraction, homeomorphism).
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

Tour pages add: `kind: tour`, `activity: ski-tour | hike | via-ferrata | alpine-tour`, `region`, `start_m`, `summit_m`, `aspect`, `glacier`
(true/false), `difficulty`, `best_months` (list of three-letter months) and `done` (date of the last time done, or
`null`). Keep `done` in sync with `Wiki/topics/tour-log.md`.

Slugs (file names) are unique across the whole wiki, because `[[wikilinks]]` resolve by file name. Link pages
with `[[wikilinks]]`. If a page you link to doesn't exist yet, leave the link: it marks a gap.

## Workflows

- **Ingest** a new source: write `Wiki/sources/<slug>.md`, create or update the entity and concept pages it
  touches, add new pages to `Wiki/index.md`, add an entry on top of `Wiki/log.md`. Note contradictions with
  existing pages on both pages instead of overwriting.
- **Answer a question:** start from `Wiki/index.md`, read the relevant pages, answer with `[[links]]` to the pages
  you used. Say what the vault doesn't know. You have no web access: for current conditions (snow, avalanche
  danger, hut opening) tell the user to check the official bulletins.
- **New topic:** create `Wiki/topics/<topic>.md` as its hub, use the existing folders, add a section to
  `Wiki/index.md`.
- **Lint:** report dead links, orphan pages, pages without sources, `done` fields that disagree with the tour log,
  and contradictions; fix only after the user agrees.

Never commit or push; the user reviews your changes and commits them in the app.
