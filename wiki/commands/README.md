---
title: Command Templates
type: command_index
status: ready
privacy: private
last_updated: 2026-06-30
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
- `wiki/commands/lint_wiki.md`: Default `health check`; run the Karpathy-style wiki knowledge lint for contradictions, stale claims, structural gaps, knowledge gaps, source tracking, privacy, and conceptual consistency.
- `wiki/commands/repo_health_check.md`: Run only for `repo health check`; check repository/worktree/git hygiene and then ask whether to commit and push.
- `wiki/commands/generate_research_prompt.md`: Generate an evidence-aware research or writing prompt.
- `wiki/commands/generate_design_spec_prompt.md`: Generate a system design, research prototype, or spec prompt.
- `wiki/commands/citation_supported_brainstorming.md`: Suggest citations from wiki citation memory, generate an AI feed prompt, and prepare Zotero/EndNote-compatible RIS content.

## Suggested Daily Flow

1. Add source or quick note.
2. Run targeted wiki query.
3. Generate research/design prompt if needed.
4. Use citation-supported brainstorming when moving from an idea to a manuscript-specific Zotero/EndNote collection.
5. File durable synthesis back into the wiki when useful.
6. Run wiki health checks periodically, including contradictions, stale claims, structural gaps, knowledge gaps, stale living overviews, synthesis pages, reference plans, workflow files, index, and memory.
7. Run repo health checks only when preparing publication or when the user explicitly asks for repository/git health.

## Maintenance Guardrail

When ingesting or linting, check whether `wiki/overview/domain_map.md`, `wiki/overview/caregiver_system_core_sota_synthesis.md`, relevant reference plans, `INDEX.md`, `MEMORY.md`, and workflow or command files need updates. Update affected pages in the same turn, or log an explicit deferral in `LOG.md`.
