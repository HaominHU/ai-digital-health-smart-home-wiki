---
title: Output Durability and Publication Policy
type: output_index
status: ready
privacy: private
last_updated: 2026-07-14
---

# Output Durability and Publication Policy

## Purpose

The `outputs/` tree contains generated artifacts with different lifecycles. Do not ignore the entire tree: selected Markdown outputs are part of the wiki's reusable research record and audit history. At the same time, review artifacts, temporary work, and regenerable exports should not create repository noise or accidental publication risk.

## Default Policy

| Path | Default Git status | Track when |
| --- | --- | --- |
| `outputs/ingest_previews/` | Local-only and ignored | Only when the user explicitly requests publishing exact preview files after considering source, copyright, and privacy constraints |
| `outputs/_scratch/` | Local-only and ignored | Never as scratch; move a reviewed artifact to its durable output folder first |
| `outputs/citation_exports/` | Generated exports are local-only and ignored; README and `.gitkeep` remain tracked | Only when the user explicitly requests preserving or publishing exact export files |
| `outputs/evidence_briefs/` | Selectively trackable | The brief is intentionally durable, privacy-safe, and useful for later research or handoff |
| `outputs/research_prompts/` | Selectively trackable | The prompt is intentionally durable and reusable |
| `outputs/design_prompts/` | Selectively trackable | The prompt is intentionally durable and reusable |
| `outputs/spec_prompts/` | Selectively trackable | The prompt is intentionally durable and reusable |
| `outputs/query_answers/` | Selectively trackable | The answer contains durable synthesis worth preserving outside chat |
| `outputs/lint_reports/` | Selectively trackable | The report records meaningful findings, fixes, decisions, or residual risks |

Routine no-change checks, one-off drafts, intermediate transformations, and disposable experiments should remain in chat or use `outputs/_scratch/`. Do not save a lint report merely to record that a routine check ran without meaningful findings.

## Durability Test

Before tracking a generated output, confirm all of the following:

1. It is useful beyond the current chat or run.
2. It has a clear research, audit, handoff, or reuse role.
3. It does not duplicate maintained wiki knowledge that should instead be integrated into the owning wiki page.
4. Its evidence, interpretation, and speculative content are labeled appropriately.
5. It contains no PHI, identifiable participant data, private raw notes, restricted source content, or other material that should remain local.
6. It is written in English and follows repo naming and metadata conventions.

## Navigation and Logging

- Add a durable output to `INDEX.md` when future readers need a stable route to it.
- Append the appropriate `output`, `prompt`, `query`, or `lint` entry to `LOG.md` whenever a durable output file is created or materially updated.
- If a generated output contains knowledge that belongs in the maintained wiki, integrate it into the correct owner page or record a short deferral in `LOG.md`.

## Publication Boundary

Normally local-only artifacts may be tracked only after an explicit user request naming the files or clearly covering that artifact class for the current turn. Before staging them, verify privacy, source/copyright, and evidence-status implications. Never use the private repo setting as a substitute for those checks.
