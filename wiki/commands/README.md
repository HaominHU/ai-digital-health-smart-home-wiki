---
title: Command Templates
type: command_index
status: ready
privacy: private
last_updated: 2026-05-18
---

# Command Templates

These commands are short triggers for Codex CLI/Desktop.

They rely on:

- `AGENTS.md`
- `MEMORY.md`
- `INDEX.md`
- `wiki/workflows/`

Use them instead of repeating long setup prompts. Long prompts are for major architecture changes only. Daily maintenance should use short commands.

## Available Commands

- `wiki/commands/ingest_source.md`: Process a paper, report, note, document, PDF, or other source.
- `wiki/commands/quick_note.md`: Add a short idea, takeaway, meeting note, or personal research thought.
- `wiki/commands/ask_wiki.md`: Answer a question using the maintained wiki.
- `wiki/commands/lint_wiki.md`: Health-check source tracking, privacy, and conceptual consistency.
- `wiki/commands/generate_research_prompt.md`: Generate an evidence-aware research or writing prompt.
- `wiki/commands/generate_design_spec_prompt.md`: Generate a system design, research prototype, or spec prompt.

## Suggested Daily Flow

1. Add source or quick note.
2. Run targeted wiki query.
3. Generate research/design prompt if needed.
4. File durable synthesis back into the wiki when useful.
5. Run lint periodically.
