# Sources

Raw source files may be stored here locally, but they are ignored by git by default.

Use this folder for local copies of papers, reports, PDFs, Word documents, abstracts, documentation, conference notes, presentation notes, and other durable source artifacts.

You can either place files here yourself or give Codex a local file path and ask it to copy/store the source here before ingesting. If you provide only a DOI, URL, or external reference, Codex should record the reference and should download/store a local copy only when you ask and access is available.

Default policy:

- Preserve raw sources locally when useful.
- Do not modify raw source files after saving.
- Do not commit raw source contents by default.
- Track source-derived knowledge in `wiki/` with source IDs and evidence labels.
- Use ingest previews under `outputs/ingest_previews/` for major sources before updating the wiki.

Recommended source ID and filename pattern:

```text
YYYY-MM-DD_author-or-org_short-title.ext
```

Examples:

```text
2026-05-18_smith_smart-home-caregiving-review.pdf
2026-05-18_nih_ai-digital-health-report.docx
2026-05-18_conference-session_fall-risk-sensing-notes.md
```
