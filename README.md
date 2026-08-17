# DSA Panel for Mac

**Showcase repository — project overview only. Source code is closed.**

Anyone prepping for coding interviews knows the mess: problems solved on
LeetCode, notes in a random Notion page, a timer running separately on
your phone, and a spreadsheet you update maybe once a week if you
remember. Nothing talks to anything else, and it's hard to see what
you've actually covered versus what you've been quietly avoiding.

DSA Panel keeps all of it in one native Mac app instead.

## What it does

**Dashboard analytics** — overall progress across curricula and practice
sets, a real-time streak counter, a GitHub-style contribution heatmap
over the last 6 months, a weekly solved-per-day chart, and a queue of
what's due for revision based on spaced repetition.

**Markdown notes editor** — a block-based editor per problem, with
automatic language detection on paste (C++/Java/Python/JS get wrapped
in correctly syntax-highlighted code blocks automatically), reorderable
notes, and silent autosave.

**A real sketch board, not a whiteboard photo** — vector drawing tools
(pencil, shapes, text, a hand tool for panning) with true undo/redo:
every change to the canvas is a fully reversible snapshot, not a
best-effort undo stack. Exports straight to PNG.

**Time tracking** — subject-wise time logging with color-coded tracks,
an hour-grid timeline, and a fullscreen focus-timer view for practicing
under actual interview time pressure.

**Full keyboard-driven navigation** — global search, sidebar toggle, and
direct jumps to every major view, all bound to `⌘`-key shortcuts, so it
stays fast to use without reaching for the trackpad.

**Everything stays on your machine** by default, with an optional
Google Drive-backed backup you control.

## Built with

Flutter, compiled to a native macOS app.

| Concern | Package |
|---|---|
| State management | `flutter_riverpod` |
| Local database | `drift` (SQLite) |
| Charts | `fl_chart` |
| Notes rendering | `flutter_markdown` |
| Backup | Google Sign-In + Drive API |
| Motion | `flutter_animate` |

This is the public dependency surface, not the implementation — the
spaced-repetition scheduling, the snapshot-based undo engine behind the
sketch board, and the rest of the app's internals stay out of this repo.

## About this repository

This is a **showcase-only** repo — a description of what the app does,
published to share the project publicly without exposing the
implementation. The actual source lives in a private repository.
Screenshots to be added.

## License

All rights reserved. The name, design, and underlying application are
proprietary; nothing in this repository is licensed for reuse.
