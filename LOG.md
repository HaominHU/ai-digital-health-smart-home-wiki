# LOG.md

Chronological project log for the AI Digital Health and Smart Home Research Wiki.

Use this as the Karpathy-style append-only timeline of meaningful ingests, queries, lint checks, architecture changes, workflow updates, generated outputs, and memory updates.

Entry format:

```text
## [YYYY-MM-DD] type | Short title

- Summary: One or two lines.
- Files touched: `path`, `path`.
- Notes: Optional.
```

Recommended types:

- `ingest`: Source-backed knowledge integrated into the wiki.
- `query`: A meaningful wiki query or synthesis whose result should be preserved.
- `lint`: Wiki health check, privacy check, source-support check, or conceptual consistency check.
- `architecture`: Folder structure, schema, or project design change.
- `workflow`: Workflow file or operating-rule update.
- `output`: Generated artifact such as a preview, brief, prompt, or report.
- `prompt`: AI-ready research, design, or spec prompt generation.
- `memory`: Compressed state update in `MEMORY.md`.

Logging rule: if the work changes wiki source content, generated outputs, architecture, workflow state, or project memory, append a `LOG.md` entry in the same turn.

## [2026-05-18] architecture | Initialized research wiki scaffold

- Summary: Created the initial Karpathy-style research wiki structure for AI-driven digital health and smart home technologies, including raw source, wiki, output, and private note folders.
- Files touched: `AGENTS.md`, `README.md`, `INDEX.md`, `LOG.md`, `MEMORY.md`, `sources/`, `wiki/`, `outputs/`, `private_notes/`.
- Notes: Established privacy-sensitive healthcare handling, clinical decision boundaries, source tracking, and Obsidian-compatible Markdown conventions.

## [2026-05-18] workflow | Defined local raw source storage policy

- Summary: Added local-only raw source storage defaults, gitignore rules, source filename conventions, and lint reminders for source retention review.
- Files touched: `.gitignore`, `sources/README.md`, `private_notes/README.md`, `AGENTS.md`, `README.md`, `MEMORY.md`, `wiki/workflows/ingest_source.md`, `wiki/workflows/lint_wiki.md`, `LOG.md`.
- Notes: User will manually handle commits and git management. Raw sources are ignored by git by default and should not be deleted automatically.

## [2026-05-18] workflow | Simplified README usage instructions

- Summary: Revised `README.md` to match the restaurant wiki's icon-led format and replaced AI-facing reproduction steps with user-facing prompt examples for ingest, quick notes, queries, prompt generation, and linting.
- Files touched: `README.md`, `sources/README.md`, `LOG.md`.
- Notes: Clarified that command files are reusable instruction recipes, not terminal commands, and that Codex can copy local files into `sources/` when asked.
