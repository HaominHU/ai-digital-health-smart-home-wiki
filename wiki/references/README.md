---
title: Reference and Citation Memory
type: reference_index
status: draft
privacy: private
last_updated: 2026-11-05
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

The citation-memory layer is established. After the November 2026 monthly PubMed ingest, all 63 citation-bearing evidence sources have canonical item records; two additional evidence pages represent user-provided lecture takeaways rather than formal citation-bearing sources. The three AMIA submission records remain incomplete and not export-ready pending final publication or acceptance metadata. The other 60 records are RIS-ready; missing optional metadata is disclosed in each record, including Hwang's exact publication date, Almeida's final volume/issue/pages, and Tu's exact publication date and final bibliographic fields. Generated RIS files remain local-only by default.

The October records preserve original citations and printed publication dates for El-Saboni, Liu, Batchelor, Allheeib, and Long. Export readiness concerns bibliographic completeness; Allheeib remains conceptual and the review and guideline evidence limits remain attached to citation use.

The October a la carte record for Tu preserves the supplied article-in-press version and permanent DOI. Its source ID uses the ingest date, not an asserted publication date. RIS export can use the verified core citation fields with a version note while omitting unverified final fields. Citation memory remains shared across discovery lanes, with no duplicate record for a paper encountered through more than one channel.

## November 2026 Citation Records

Six approved November sources add bibliographic memory with distinct knowledge roles: caregiver needs (Wang/Silva), formative persona evaluation (Nyamathi), patient-only null overall trial results (Svendsen), older-adult adoption context (Vandelli), and requirements with numerical reporting caution (Xianheng). All are RIS-ready; this does not upgrade their evidence strength. Three unavailable PMIDs remain pending without maintained citation/evidence records.

- `wiki/references/items/2026-10-29_wang_mental-health-technology-needs-dementia-caregivers.md`
- `wiki/references/items/2026-10-26_silva_health-literacy-alzheimer-family-caregivers.md`
- `wiki/references/items/2026-10-28_nyamathi_personas-daily-activity-maps-dementia.md`
- `wiki/references/items/2026-11-04_svendsen_digital-stress-management-breast-cancer.md`
- `wiki/references/items/2026-07-30_vandelli_trust-digital-health-remote-older-adults.md`
- `wiki/references/items/2026-10-20_xianheng_smart-home-care-platform-requirements-kano.md`
