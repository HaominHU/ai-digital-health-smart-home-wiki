---
title: Repo Health Check Workflow
type: workflow
status: ready
privacy: private
last_updated: 2026-07-14
---

# Repo Health Check Workflow

## Purpose

Check repository, worktree, and publication hygiene before any commit or push decision.

Use this workflow when the user says "repo health check" or clearly asks for repository/git health. Do not use it for the default "health check"; that phrase means the wiki knowledge lint in `wiki/workflows/lint_wiki.md`.

## Scope

- Git worktree state.
- Staged, unstaged, untracked, and ignored files.
- Local-only artifact boundaries.
- Branch and remote status.
- Obvious infrastructure or workflow problems that could affect commit or push safety.

This workflow does not replace the wiki knowledge health check. If the user asks for both, run the wiki health check first, then the repo health check.

## Required Checks

1. Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and `LOG.md`.
2. Run `git status --short --branch`.
3. Run `git status --short --ignored` before any commit recommendation.
4. Verify raw `sources/`, `outputs/ingest_previews/`, `outputs/_scratch/`, and generated `outputs/citation_exports/` artifacts remain local-only unless the user explicitly asked to publish exact paths in this turn.
5. Check staged changes with `git diff --cached --stat` and `git diff --cached --name-status` when files are staged.
6. Check unstaged changes with `git diff --stat` and targeted diffs when needed.
7. Check untracked files and decide whether they are maintained wiki files, generated outputs, local-only artifacts, or unrelated scratch files.
8. Check branch and upstream status with `git branch --show-current` and `git status --short --branch`.
9. Report issues first, ordered by commit/push risk.
10. If no blocking issue remains, ask the user whether to commit and push. Do not commit or push without explicit confirmation.

## Local-Only Artifact Guardrail

By default, do not stage or publish:

- `outputs/ingest_previews/`
- `outputs/_scratch/`
- generated files under `outputs/citation_exports/`
- raw source files under `sources/`
- sensitive or identifiable material under `private_notes/`
- generated scratch files that are not meant as maintained wiki artifacts

Other generated output folders are selectively trackable. Before recommending them for staging, verify that each file is intentionally durable, privacy-safe, useful beyond the current run, logged in `LOG.md`, and routed from `INDEX.md` when navigation is useful. Meaningful lint reports may be tracked; routine no-change lint output should normally remain in chat.

If the user explicitly asks to publish a normally local-only artifact, confirm the exact file paths and privacy/source rationale before staging.

## Suggested Commands

```sh
git status --short --branch
git status --short --ignored
git diff --stat
git diff --cached --stat
git diff --cached --name-status
git branch --show-current
```

## Output Format

Report:

- Blocking issues.
- Non-blocking warnings.
- Local-only artifacts verified as ignored or unstaged.
- Files that appear ready for commit.
- Whether a separate wiki health check is still needed.
- A direct question asking whether to commit and push if the repo is ready.

## Required LOG.md Update

If the repo health check changes files, creates a durable report, or leads to a commit/push workflow, append the appropriate `lint`, `workflow`, or `output` entry to `LOG.md`.
