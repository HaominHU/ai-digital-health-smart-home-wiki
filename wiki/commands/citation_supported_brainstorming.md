---
title: Citation-Supported Brainstorming Command
type: command
status: ready
privacy: private
last_updated: 2026-07-14
---

# Citation-Supported Brainstorming

Use when the user says:

- "I am brainstorming a paper about..."
- "Suggest citations for this paper idea."
- "Generate a citation-supported prompt."
- "Create a Zotero/EndNote import list from the wiki."
- "Give me citations for intro/background/significance."

## Command

Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, `wiki/references/README.md`, and `wiki/workflows/citation_supported_brainstorming.md`.

Use wiki-first mode by default: start with stored citation records and relevant wiki evidence pages, then assess coverage quality. Do not use a fixed citation-count threshold. Identify whether the wiki is missing foundational, recent state-of-the-art, population, condition, technology, or writing-role coverage.

If the user asks to include searched citations, or approves external seed search, keep those results separate from wiki citations and label them as external candidates, not yet ingested.

Produce:

1. Topic interpretation.
2. Citation coverage assessment.
3. Wiki citation map grouped by writing role.
4. Separate searched external candidate citation map when requested or approved.
5. AI feed prompt for introduction/background/significance or the requested writing section.
6. Separate Zotero/EndNote-compatible RIS export content for wiki citations and external candidates when enough metadata is available.
7. Backfill notes for missing reference records or incomplete citation metadata.

Do not invent citations, DOIs, author lists, venues, findings, or study details.

Save durable prompt files only when the user asks for files or when the result is explicitly meant to be preserved under `outputs/`. Use `wiki/templates/citation_supported_brainstorming_output_template.md` for durable Markdown outputs. Generated RIS files are local-only by default; track a specific export only when the user explicitly asks to preserve or publish it.
