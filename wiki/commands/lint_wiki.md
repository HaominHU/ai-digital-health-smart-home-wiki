---
title: Wiki Health Check Command
type: command
status: ready
privacy: private
last_updated: 2026-06-30
---

# Wiki Health Check

Use when the user says:

- "Health check"
- "Lint the wiki"
- "Health-check the wiki"
- "Check source tracking"
- "Check privacy risks"
- "Find gaps"

Do not use this command when the user says "repo health check"; use `wiki/commands/repo_health_check.md` instead.

## Command

Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, `LOG.md`, and `wiki/workflows/lint_wiki.md`.

Run the Karpathy-style wiki knowledge lint:

- Contradictions across compiled pages.
- Stale claims superseded or narrowed by newer sources.
- Structural gaps such as orphan pages, missing backlinks, weak cross-references, and stale index entries.
- Knowledge gaps such as repeated concepts without dedicated pages or areas requiring external search.

Also check source tracking, privacy and security risks, evidence labels, conceptual consistency, knowledge ownership boundaries, overlapping concepts, stale overview/synthesis/domain-map/reference-plan/workflow/index/memory entries, and future RAG readiness.

Report findings first, ordered by severity.

Fix only what the user asked to fix unless the user explicitly authorizes fixes.
