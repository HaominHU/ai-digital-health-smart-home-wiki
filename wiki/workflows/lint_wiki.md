---
title: Wiki Health Check Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-07-14
---

# Wiki Health Check Workflow

## Purpose

Health-check the research wiki so it stays accurate, source-tracked, privacy-aware, conceptually disciplined, structurally navigable, and useful as it grows.

When the user says "health check" without the word "repo", this workflow is the default meaning. It is a wiki knowledge lint, not a git, commit, or push workflow.

Use `wiki/workflows/repo_health_check.md` only when the user says "repo health check" or otherwise clearly asks for repository/worktree/git hygiene.

## Karpathy-Style Knowledge Lint

- Contradictions: identify conflicting claims, incompatible interpretations, or opposing data points across compiled wiki pages.
- Stale claims: spot old assertions that have been superseded, narrowed, or disproven by newer ingested sources.
- Structural gaps: find orphan pages, missing incoming links, weak cross-references, stale index entries, and missing backlinks between interrelated concepts.
- Knowledge gaps: highlight important recurring concepts without dedicated article pages, missing source coverage, and areas that require external web or literature search before stronger synthesis can be written.

## Lint Checklist

- Contradictions between source summaries, topic pages, overview pages, design patterns, or research questions.
- Stale claims superseded by later ingests or narrowed by newer evidence limits.
- Structural gaps, including orphan pages, missing backlinks, broken links, and stale `INDEX.md` routing.
- Knowledge gaps, including repeated concepts without dedicated pages or missing external-source coverage.
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
- Generated outputs whose tracked/local-only status conflicts with `outputs/README.md`.
- Tracked lint reports that contain only routine no-change output, or meaningful durable outputs that are missing `INDEX.md` routing or a `LOG.md` entry.
- Missing citation-memory records for citation-bearing evidence sources.
- Reference records missing original citation text, source IDs, evidence type, or export-readiness status.
- RIS exports that appear to contain invented or incomplete metadata.
- Future RAG readiness problems such as missing tags, source IDs, dates, or summaries.
- Locally stored raw sources that may no longer need to be retained after successful wiki digestion.

## Lint Steps

1. Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and `LOG.md`.
2. Scan files and frontmatter.
3. Check contradictions across evidence, topic, overview, design, and research-question pages.
4. Check stale claims against `LOG.md`, `INDEX.md`, recent evidence pages, and living overview/synthesis pages.
5. Check structural gaps: cross-links, backlinks, orphan pages, broken links, stale index entries, and missing routing.
6. Check knowledge gaps: recurring concepts without pages, missing condition/population/technology anchors, and areas that need external search.
7. Check source and evidence labels.
8. Check privacy and healthcare decision boundaries.
9. Check conceptual distinctions.
10. Check citation-memory records under `wiki/references/items/` against citation-bearing evidence pages.
11. Check overview and synthesis freshness against `LOG.md`, `INDEX.md`, and recent evidence pages.
12. Check knowledge ownership boundaries: evidence pages vs citation records vs overview/synthesis pages vs topic pages vs design patterns vs research questions.
13. Check whether raw sources under `sources/` should be retained, moved, or removed after successful digestion.
14. Check generated outputs against `outputs/README.md`: local-only boundaries, intentional durability, privacy safety, index routing, and log coverage.
15. Report findings first, ordered by severity.
16. Fix only the issues the user asked to fix, unless the lint task explicitly authorizes fixes.
17. Do not delete raw sources automatically; flag them for user review.
18. Append a `lint` entry to `LOG.md` when the lint pass changes files or creates a durable report.

## Suggested Commands

```sh
rg --files
rg -n "TODO|TBD|unknown|missing|gap|needs source|source needed" .
rg -n "diagnose|treatment|recommend|PHI|participant|patient|clinical" .
rg -n "normal aging|aging issue|caregiver|care recipient|evidence type" wiki
rg -n "citation_status|export_ready|Original Citation|RIS Export" wiki/references wiki/templates
rg -n "last_updated:|domain_map|synthesis|reference_plan|Part [0-9]|next planned|living" AGENTS.md INDEX.md MEMORY.md LOG.md wiki
rg -n "contradict|conflict|superseded|outdated|stale|orphan|backlink|cross-link|cross link|external search|needs page" wiki INDEX.md MEMORY.md LOG.md
```

## Required LOG.md Update

If the lint pass changes files or saves a durable lint report, append a `LOG.md` entry in the same turn.
