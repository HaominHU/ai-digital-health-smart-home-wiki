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

## Paper Discovery Lanes and Topic Categories

- `papers/cg_system_core/`: the planned caregiver system-design citation set; use `wiki/references/cg_system_core_reference_plan.md` for status.
- `papers/monthly_pubmed/`: papers received through monthly PubMed pushes.
- `papers/alacarte/`: papers encountered through posts, LinkedIn, links, or other ad hoc discovery. This lane begins with the October 2026 ingest.

Keep monthly PubMed and a la carte provenance separate, while reusing the same topic-lens folder names where appropriate: `adoption_preferences_and_equity/`, `ai_interaction_and_decision_support/`, `caregiving_support_systems/`, `smart_home_and_ambient_care/`, and `wearables_and_remote_monitoring/`. Create a category only when needed and assign each paper by its primary contribution. Keep screened but withdrawn items under the lane's `deferred_or_out_of_scope/` when needed; do not duplicate a PDF across lanes or topic folders.

The maintained wiki synthesizes across all source lanes through shared topic pages, with one canonical evidence page and citation-memory record per paper. Discovery channel does not determine evidence quality. The article supplies research evidence; a post that led to it is discovery context unless separately reviewed. Do not invent an exact post, URL, or discovery date.

## Source IDs and Dates

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

If exact publication date is unknown, use the available source date under the ingest workflow, or the ingest date when no usable source date is available, and record the date basis. For article-in-press papers, do not substitute acceptance or PDF-creation dates for publication dates. Keep ingest month separate from publication date and leave unknown bibliographic fields empty.
