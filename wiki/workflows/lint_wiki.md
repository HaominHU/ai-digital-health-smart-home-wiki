---
title: Lint Wiki Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-05-18
---

# Lint Wiki Workflow

## Purpose

Health-check the research wiki so it stays accurate, source-tracked, privacy-aware, conceptually disciplined, and useful as it grows.

## Lint Checklist

- Missing source tracking.
- Unsupported claims.
- Evidence type missing or unclear.
- Published evidence mixed with personal observation.
- Personal ideas presented as established evidence.
- Caregiver needs mixed with care recipient needs.
- Disease, disability, aging-related decline, and age-associated prevalence conflated.
- Dementia treated as normal aging.
- Cancer treated as an aging issue rather than disease.
- Falls reduced to a single cause without noting interacting causes.
- PHI or identifiable participant data present outside an approved safe handling policy.
- Public-ready outputs containing private or sensitive notes.
- Missing privacy/security/ethics boundaries in healthcare-related prompts.
- Stale `INDEX.md` entries.
- Missing `LOG.md` entries for meaningful changes.
- Orphan pages under `wiki/`.
- Duplicate pages or overlapping concepts.
- Inconsistent YAML frontmatter.
- Generated outputs that should be digested back into the wiki.
- Future RAG readiness problems such as missing tags, source IDs, dates, or summaries.
- Locally stored raw sources that may no longer need to be retained after successful wiki digestion.

## Lint Steps

1. Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and `LOG.md`.
2. Scan files and frontmatter.
3. Check source and evidence labels.
4. Check privacy and healthcare decision boundaries.
5. Check conceptual distinctions.
6. Check cross-links and orphan pages.
7. Check whether raw sources under `sources/` should be retained, moved, or removed after successful digestion.
8. Report findings first, ordered by severity.
9. Fix only the issues the user asked to fix, unless the lint task explicitly authorizes fixes.
10. Do not delete raw sources automatically; flag them for user review.
11. Append a `lint` entry to `LOG.md` when the lint pass changes files or creates a durable report.

## Suggested Commands

```sh
rg --files
rg -n "TODO|TBD|unknown|missing|gap|needs source|source needed" .
rg -n "diagnose|treatment|recommend|PHI|participant|patient|clinical" .
rg -n "normal aging|aging issue|caregiver|care recipient|evidence type" wiki
```

## Required LOG.md Update

If the lint pass changes files or saves a durable lint report, append a `LOG.md` entry in the same turn.
