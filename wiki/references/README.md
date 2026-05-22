---
title: Reference and Citation Memory
type: reference_index
status: draft
privacy: private
last_updated: 2026-05-22
---

# Reference and Citation Memory

## Purpose

This folder stores the wiki's knowledge-level citation memory.

The guiding principle is:

> Use the wiki as knowledge-level citation memory; use Zotero or EndNote as paper-level reference management, where each manuscript or project can remain its own collection root.

The wiki should remember why a source matters, which topics and claims it can support, and which writing roles it can serve. Zotero and EndNote remain the tools for PDF management, citation styling, coauthor sharing, and manuscript-specific reference collections.

## Folder Structure

- `wiki/references/items/`: One Markdown citation-memory record per source.
- `wiki/templates/reference_item_template.md`: Template for new citation-memory records.
- `outputs/citation_exports/`: Generated Zotero/EndNote-compatible export files, usually RIS.

## Canonical Storage Rule

Citation records are stored as Markdown with YAML frontmatter. Export files are generated artifacts.

Do not use topic-specific RIS files as canonical storage. A single source may support multiple topics, claims, conditions, populations, technologies, and writing roles.

## Citation Record Responsibilities

Each citation-memory record should track:

- `source_id`.
- Original citation text.
- DOI, URL, publication venue, year, authors, and source file when available.
- Evidence type and privacy level.
- Related topics, populations, conditions, technologies, caregiving challenges, and care recipient needs.
- Claims or knowledge roles the source can support.
- Writing roles such as introduction, background, significance, theory, methods, design rationale, limitations, or gap framing.
- Export readiness and missing bibliographic fields.

## Export Rule

Use RIS as the primary Zotero/EndNote-compatible export format unless the user asks for BibTeX or another format.

Generated export files should be saved under `outputs/citation_exports/` and named with the date plus topic, for example:

```text
2026-05-22_dementia-caregiving-smart-home_wiki-citations.ris
2026-05-22_dementia-caregiving-smart-home_external-candidates.ris
```

Keep wiki citations and searched external candidate citations in separate export files. External candidates are bibliography-building leads and should not be treated as established wiki evidence until reviewed or ingested.

## Current Status

The existing wiki already stores source IDs and some original citation text in evidence pages, but it did not previously have a dedicated reference-management layer or RIS export workflow. Existing source citations should be backfilled into `wiki/references/items/` as sources are revisited or when a citation-supported brainstorming output needs them.
