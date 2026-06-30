---
title: Repo Health Check Command
type: command
status: ready
privacy: private
last_updated: 2026-06-30
---

# Repo Health Check

Use when the user says:

- "Repo health check"
- "Check repo health"
- "Check git health"
- "Health check then confirm commit and push" when the wording clearly refers to repository publication readiness

Do not use this command for the default phrase "health check"; use `wiki/commands/lint_wiki.md` for that wiki knowledge lint.

## Command

Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, `LOG.md`, and `wiki/workflows/repo_health_check.md`.

Check repository/worktree status, staged and unstaged changes, untracked files, ignored local-only artifacts, branch/upstream state, and publication safety.

Verify `outputs/ingest_previews/`, raw `sources/`, and sensitive `private_notes/` artifacts are not staged unless the user explicitly requested publishing those exact paths.

Report blocking issues first. If no blocking issue remains, ask the user whether to commit and push. Do not commit or push without explicit confirmation.
