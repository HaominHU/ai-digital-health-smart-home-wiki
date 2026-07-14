---
title: Citation Export Outputs
type: output_index
status: ready
privacy: private
last_updated: 2026-07-14
---

# Citation Export Outputs

This folder stores generated citation export files for Zotero or EndNote, usually in RIS format.

These files are outputs, not canonical citation memory. The canonical citation-memory records live under `wiki/references/items/`.

Generated export files are regenerable and local-only by default. Keep this README and `.gitkeep` tracked, but track a specific RIS or other export only when the user explicitly asks to preserve or publish that exact file. Before tracking an export, confirm that its metadata is complete, its evidence status is clear, and it contains no sensitive or private material that should remain local.

Use filenames like:

```text
YYYY-MM-DD_topic_wiki-citations.ris
YYYY-MM-DD_topic_external-candidates.ris
```

Keep wiki citations and searched external candidate citations in separate RIS files. Both may be imported into Zotero or EndNote, but they have different evidence status inside the wiki.

Do not add citations to an export file unless the source metadata is known. Mark incomplete citations in the associated Markdown brainstorming output instead of inventing missing RIS fields.

External candidate citations are bibliography-building leads. They should not be treated as established wiki evidence until reviewed or ingested.
