---
title: Ingest Source Command
type: command
status: ready
privacy: private
last_updated: 2026-05-18
---

# Ingest Source

Use when the user says:

- "Ingest this source"
- "Add this paper to the wiki"
- "Process this PDF"
- "Integrate these conference notes"
- "Update the wiki from this report"

## Command

Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and `wiki/workflows/ingest_source.md`.

Identify source context, evidence type, privacy level, and whether human review is required.

For major sources, create an ingest preview under `outputs/ingest_previews/` and ask for confirmation before updating wiki pages.

For short low-risk notes, update the relevant wiki pages directly if source context is clear.

Always track sources, separate evidence from interpretation, respect the clinical decision boundary, update `INDEX.md` when needed, and append to `LOG.md`.
