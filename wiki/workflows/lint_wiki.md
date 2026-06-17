---
title: Lint Wiki Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-06-17
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
- Topic pages duplicating full source summaries instead of linking to evidence pages.
- Stale overview, synthesis, domain-map, reference-plan, workflow, command, index, or memory pages after later ingests.
- `wiki/overview/domain_map.md` missing major later evidence anchors or trying to serve as a complete evidence synthesis.
- `wiki/overview/caregiver_system_core_sota_synthesis.md` not reflecting later relevant caregiver-system ingests.
- Inconsistent YAML frontmatter.
- Generated outputs that should be digested back into the wiki.
- Missing citation-memory records for citation-bearing evidence sources.
- Reference records missing original citation text, source IDs, evidence type, or export-readiness status.
- RIS exports that appear to contain invented or incomplete metadata.
- Future RAG readiness problems such as missing tags, source IDs, dates, or summaries.
- Locally stored raw sources that may no longer need to be retained after successful wiki digestion.

## Lint Steps

1. Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and `LOG.md`.
2. Scan files and frontmatter.
3. Check source and evidence labels.
4. Check privacy and healthcare decision boundaries.
5. Check conceptual distinctions.
6. Check citation-memory records under `wiki/references/items/` against citation-bearing evidence pages.
7. Check overview and synthesis freshness against `LOG.md`, `INDEX.md`, and recent evidence pages.
8. Check knowledge ownership boundaries: evidence pages vs citation records vs overview/synthesis pages vs topic pages vs design patterns vs research questions.
9. Check cross-links and orphan pages.
10. Check whether raw sources under `sources/` should be retained, moved, or removed after successful digestion.
11. Report findings first, ordered by severity.
12. Fix only the issues the user asked to fix, unless the lint task explicitly authorizes fixes.
13. Do not delete raw sources automatically; flag them for user review.
14. Append a `lint` entry to `LOG.md` when the lint pass changes files or creates a durable report.

## Suggested Commands

```sh
rg --files
rg -n "TODO|TBD|unknown|missing|gap|needs source|source needed" .
rg -n "diagnose|treatment|recommend|PHI|participant|patient|clinical" .
rg -n "normal aging|aging issue|caregiver|care recipient|evidence type" wiki
rg -n "citation_status|export_ready|Original Citation|RIS Export" wiki/references wiki/templates
rg -n "last_updated:|domain_map|synthesis|reference_plan|Part [0-9]|next planned|living" AGENTS.md INDEX.md MEMORY.md LOG.md wiki
```

## Required LOG.md Update

If the lint pass changes files or saves a durable lint report, append a `LOG.md` entry in the same turn.
