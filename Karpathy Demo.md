---
type: topic
tags: [guide, demo]
updated: 2026-10-06
sources: []
related: [index, log, brew-ratio, homeomorphism, avalanche-safety-kit, aeropress]
---

# Karpathy Demo

A guided tour of [karpathy.app](https://karpathy.app) using this vault. Each chapter says what a feature does, links
to a page here that shows it, and gives you something to try.

> [!tip] How to use this guide
> Tap a link, look around, then press **Back**: you return to the same place in this guide. Switch to **Read** mode
> (top of the note) for the nicest view. The app keeps that mode for every note you open next.

## 1. The vault

A vault is a Git repository full of Markdown notes, the same folder Obsidian opens. This one has three parts:

- `Sources/` — raw material: trip reports, clipped articles, course notes, and the pictures in `Sources/media/`.
  Nobody edits these.
- `Wiki/` — pages the AI writes from the sources. [[index]] lists them all, and [[log]] shows what changed when.
- `AGENTS.md` — the house rules the AI follows in this vault: folders, page format, and how to ingest a source.

The topics are deliberately unrelated: [[mountains]] (ski tours, huts, safety), [[coffee]] and [[mathematics]]
([[topology]]). **Everything is example data**, so it's not route or safety advice.

## 2. Getting in

- **Token:** the app asks for an access token once and keeps it on this device.
- **QR login:** on a phone or iPad, scan the login QR code and you're in without typing the token.
- **Install it:** *Share → Add to Home Screen* (Safari) or *Install app* (Chrome). It then opens full screen, like
  a native app.
- **Updates:** a new version installs itself the next time you open the app. The settings dialog (⚙) shows which
  version is running.

## 3. Vaults and settings

Open **⚙ Vaults & settings**:

- **Vaults:** one app, several vaults, each a GitHub repo (`owner/name`, branch, optional sub-folder). Before
  attaching a repo, the app checks it can reach it and that it has `Sources/` and `Wiki/`, and offers to create
  missing folders.
- **Switch vault** from the vault menu under the logo. Your open note is saved first.
- **Settings:** the AI model, the GitHub token (**Test token** checks it without saving), the commit reminder, and
  **Web access** (see chapter 13).

## 4. Files and notes

- **File tree:** folders first, collapsed until you open them. Try `Wiki → entities → brewers`.
- **Sort** (⇅ next to *Notes*): by **Name** (A → Z or Z → A) or by **Last changed** (newest or oldest first). Under
  *Last changed*, folders with recent changes inside move up, so you see where the activity is without opening
  anything.
- **Filter** (the funnel): show only notes changed by the **AI** or by a **Human**. A chip under *Notes* says a
  filter is on; its ✕ turns it off. Under a filter, *Last changed* means the last change by that author: *Human +
  newest first* puts your own latest edit on top, even if the AI touched the note after you. Your choices are
  remembered on this device.
- **New note:** the ✎ button next to *Notes*. **Delete** is the bin icon; you can undo a delete until you commit.
- **Autosave:** every edit is saved 1.5 s after you stop typing. The footer says *Saving… / Saved*. If the
  connection drops, your edit waits on the device and is saved when you're back online.
- **Live updates:** when the AI or a pull from GitHub changes the note you're reading, it reloads by itself, unless
  you have unsaved changes.

*Try it:* sort by **Last changed, newest first** and open the top folders: the last pages written show first. Then
do chapter 12's brew-log prompt, set the filter to **AI**, and the tree shows just what the AI changed. (The AI
filter only knows changes from version 0.0.11 on; before the AI's first edit it says "No notes changed by the AI
yet".)

## 5. Write mode and Read mode

Every note has two modes, switched at the top:

- **Write:** the Markdown text, with a live preview: headings, bold and links are styled as you type. The text
  stays exactly as written, so Obsidian and git see clean diffs.
- **Read:** the rendered page: properties as a table, images and players, clickable links.

The mode **sticks**: choose Read once and every note you open after that (from the tree, search, chat or a link)
opens in Read, even after a reload. Switching modes keeps your place in the note.

*Try it:* open [[topology]], scroll halfway down, switch Write ↔ Read, and you stay on the same paragraph.

## 6. Links

- **Wikilinks** `[[page]]` open a page by its name, wherever it lives: [[aeropress]].
- **Alias:** `[[page|other text]]` shows other text — [[coffee-mug-and-donut|why a coffee mug is a doughnut]].
- **Heading:** `[[page#Heading]]` jumps to a section — [[avalanche-safety-kit#Checklist|the checklist on the safety-kit page]].
- **Missing pages** are marked: [[euler-characteristic]] links to [[homology]], which nobody has written yet. Tap
  it and the app says so. To the AI, such a link marks a gap to fill.
- **Properties link too:** in Read mode, the `related` and `sources` values in a page's properties table are links
  ([[aeropress]] has a big one).
- **External links** open in a new tab. **Back** returns you to the same scroll position, after any link.

## 7. Obsidian-style Markdown

The app renders what Obsidian renders. Open these pages in Read mode:

| Feature | Syntax | Where to see it |
|---|---|---|
| Properties (frontmatter) | `---` block at the top | [[aeropress]] (method, filter, brew time …) |
| Tables, also wide ones that scroll sideways | `\| a \| b \|` | [[grind-size]], the tours table in [[index]] |
| Callouts | `> [!warning] Title` | [[avalanche-safety-kit]], and the tip at the top of this page |
| Task lists | `- [x]` / `- [ ]` | [[avalanche-safety-kit]], section "Checklist" |
| Highlights | `==text==` | [[brew-ratio]] |
| Footnotes | `[^1]` | [[brew-ratio]] (after "Gold Cup default") |
| Hidden comments | `%% … %%` | [[brew-ratio]]: hidden in Read mode, visible in Write mode |

## 8. Pictures, video and PDFs

Notes show their media inline, as Obsidian does. These pages hold it:

- **Pictures:** almost every brewer, tour and mathematician page has one, e.g. [[aeropress]], [[chemex]],
  [[wildspitze]], [[emmy-noether]]. The topic hubs [[coffee]] and [[topology]] have several.
- **Picture with a set width** (`![[photo.jpg|320]]`) **and a PDF:** [[brew-ratio]]. The PDF shows as a card
  with **Open** (the browser's PDF viewer, in a new tab) and **Download**.
- **Video:** [[homeomorphism]], where a coffee mug turns into a doughnut. It plays inline, on the iPhone too.
- **Both syntaxes work:** Obsidian's `![[file]]` and Markdown's `![alt](path/to/file.jpg)`.

*Try it:*

1. In [[aeropress]], tap the photo: it opens on its own. **Back** returns you to where you were in the note.
2. Switch to **Write** mode: the picture sits below its line, and the line itself stays editable text.
3. In the file tree, open `Sources/media/` and tap any `.jpg`, `coffee-brew-card.pdf` or
   `topology-mug-torus-morph.mp4`. Media files open in a viewer, not an editor.
4. Ask the chat: *"Reply with the AeroPress photo as an embed."* An embed in an AI answer shows the picture in the
   chat too.

Details: files over 50 MB load only when you tap **Load anyway**. Images from other websites are not loaded
(privacy: no tracking pixels). Offline, media shows a placeholder card.

## 9. Search

**Search** finds notes by their text and their file name:

- one word: `aeropress`;
- several words find notes that contain **all** of them: `spring snow`, `kenya natural`;
- `"quotes"` match an exact phrase: `"Gold Cup"`.

Tapping a hit opens the note at that line. In Read mode it scrolls to the matching paragraph and highlights it
briefly.

## 10. Chat with the AI

The ✦ button opens the chat. The AI reads this vault (and only this vault) and answers with links to the pages it
used. Try:

- *"Which ski tours in the vault suit late April, and why?"* (compare with
  [[similaun-vs-cevedale-late-april]], which the AI wrote earlier)
- *"Which brewer should I use for a natural-process Ethiopian coffee?"* (see [[which-brewer-for-which-bean]])
- *"Explain a homeomorphism to a ten-year-old, using pages from the vault."*

While it works, you see:

- **chips** for every file it reads or changes (tap a changed one to open it);
- a collapsible **Thinking** section;
- a footer listing the pages it changed.

Other things to know:

- **Stop** ends a turn early.
- Every chat is kept in the chat list. Resume one later, also on another device, even while it's still answering.
- One turn runs per vault at a time; a second chat waits its turn.
- On a wide screen the **⇄** button swaps the columns, so the chat becomes the big main column and the note moves to
  the side.

## 11. The AI opens notes for you

Ask *"Open the AeroPress page"* or *"Show me my tour log"*. The AI opens the note in the editor: right away on a
wide screen, or after its reply on a phone, and never while you're typing.

## 12. The AI maintains the wiki

This is the point of the vault: you add raw material, and the AI keeps the wiki pages up to date, following
`AGENTS.md`.

- **Logs:** *"Log a V60 brew: Kenya, 15 g / 250 g, 3:40, sweet and juicy."* The AI updates [[brew-log]].
  *"I did the Wildspitze tour last Saturday"* goes into [[tour-log]] and sets `done` on the tour page.
- **Ingest:** add a file to `Sources/` (or ask the AI to fetch a web page, chapter 13), then say *"Ingest the
  new source"*. The AI writes a summary page and updates the pages it touches, [[index]] and [[log]].
- **Analyses:** *"Compare V60 and Chemex"* can become a page in `Wiki/synthesis/`, like
  [[topological-invariants-overview]].
- **Lint:** *"Lint the wiki"* reports dead links (such as [[homology]]), orphan pages and contradictions.

### Commands

Skills are ready-made instructions for the AI. Type **/** in the chat box and a list of them opens, each with what it
does, filtered as you type. Pick one and add what it should work on, e.g. `/research …`. A new, empty chat also shows
the commands as one-tap chips; the ones you used last in this vault come first. A chip only fills in the command and
sends nothing.

- Commands tagged **app** come with karpathy.app and work in every vault.
- Commands tagged **vault** are the vault's own skills in `.agents/skills/`. They sync through git and work in
  Claude Code on the Mac too.
- A vault that still keeps its skills in Claude Code's layout (`CLAUDE.md`, `.claude/skills/`) is moved to
  `AGENTS.md` and `.agents/skills/` when you open it. A notice lists what moved; **Review** shows the changes, which
  wait for your commit like any other edit.

### Deep research

`/research <topic>` researches a topic on the web and writes it into the wiki, in two steps:

1. The AI reads what the wiki already knows, looks around the web a little, and writes a **plan note** in
   `Research/` with 3–6 open questions, then stops.
2. Edit the note if you like and reply **go**. The AI searches the web, saves each useful page as a source in
   `Sources/` (a summary with short quotes and the address), writes or updates the wiki pages that cite them, and
   ticks off the questions. Reply **continue** for more (at most 8 sources per answer).

`/research Research/<plan note>` picks a plan up again, in any chat, days later. It needs **Web access** (chapter 13).

*Try it:* type `/` in a new chat, pick **research** and add *pour-over grind size*. Read the plan note, reply
**go**, then open the new pages from the chips.

Nothing the AI does is final: its edits wait in **Changes** until you commit (chapter 14).

## 13. The AI on the web

With **Web access** on (⚙ → Settings; on by default), the AI can search the web and read web pages:

- *"What's the latest news on the Wildspitze glacier? Search the web."* shows a chip `searched the web: "…"`.
- *"Read https://en.wikipedia.org/wiki/AeroPress and add anything new to the AeroPress page."* shows a chip
  `fetched en.wikipedia.org/wiki/AeroPress`, and tapping the chip opens the page.
- *"Open the Wikipedia page on the AeroPress for me"* (with the address in the chat) shows an **Open** chip
  `open en.wikipedia.org/…`. Tap it and the page opens in a new browser tab; the AI itself reads nothing. This works
  with Web access off too, because your browser loads the page, not the server.

Safety rules:

- The AI may only read or offer addresses that are already in the chat: pasted by you, or found in a note or a
  search result. It can't make up an address to send your notes somewhere.
- At most 20 searches and 20 page reads per answer.
- Switch Web access off and the AI has no web tools at all.

## 14. Changes, commit and push

Nothing reaches GitHub until you say so:

- The status pill (bottom left) shows *N uncommitted* or *All committed*.
- **Changes** lists every changed file with a diff. **Discard** undoes one file.
- **Commit & Push** proposes a commit message written by the AI. Edit it, then commit: the changes go to GitHub, and
  from there to Obsidian on your other devices.
- After a number of changes (set in Settings), a reminder suggests committing.

*Try it:* in [[avalanche-safety-kit#Checklist|avalanche-safety-kit › Checklist]], switch to Write mode and change a `[ ]` to `[x]`. Open
**Changes**, look at the diff, then **Discard** it.

## 15. Conflicts

If the same note changes in Obsidian (pushed to GitHub) and in the app (not committed yet), the app shows a
conflict banner. For each file you see both versions and choose **Keep mine**, **Keep theirs** or **Keep both**.
While a conflict is open, the AI can read but not change notes.

## 16. Phone and iPad

- **Phone:** one column at a time, switched with the tab bar at the bottom (Files, Search, Chat, Changes).
- **iPad and desktop:** the file tree, the note and the chat side by side.
- **Offline:** the notes you opened before stay readable. Edits wait on the device; search and chat need a
  connection.

## 17. What it can't do yet

- No graph view, canvas or plugins.
- No renaming or moving of notes, and no note transclusion: `![[Other note]]` shows a link.
- Shell commands and Python scripts in AI skills don't run.

---

New topics, sources and pages appear in [[index]]. The history of the vault is in [[log]].
