---
name: ingest
description: Ingest the sources waiting in Input/ into the wiki, then move each one to Sources/.
---

# Ingest the waiting sources

Every folder in `Input/` is one source not ingested yet; its text is in `index.md` next to its files.

For each folder in `Input/`, one after the other, finish it completely before the next:

1. If its `index.md` frontmatter still lists `unresolved_links`, skip it: the server is still fetching its links. Say
   which folders you skipped at the end.
2. Ingest it as `AGENTS.md` describes (Workflows › Ingest): write `Wiki/sources/<slug>.md`, create or update the pages
   it touches, add new pages to `Wiki/index.md`, add an entry on top of `Wiki/log.md`. Cite the source as
   `Sources/<folder>/index.md`, the place it moves to in the next step.
3. Move the folder: call the tool `move_to_sources` with the folder name. Where that tool doesn't exist (Claude Code on
   a Mac), run `mv Input/<folder> Sources/<folder>`.

Handle every folder in one go, whatever the number. Don't commit.
