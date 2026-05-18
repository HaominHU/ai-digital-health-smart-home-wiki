---
title: Ingest Source Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-05-18
---

# Ingest Source Workflow

## Purpose

Process a source into the research wiki without losing source separation, evidence labeling, privacy boundaries, or conceptual distinctions.

Use this workflow for:

- Papers.
- Abstracts.
- Reports.
- Dissertations.
- Documentation.
- PDFs.
- Word documents.
- Markdown files.
- Conference notes.
- Presentation notes.
- Quick ideas or takeaways from in-person sessions.

## Source Context Required

Before durable integration, identify as much of this context as possible:

- Title.
- Author, speaker, or organization.
- Event or venue.
- Date.
- Source type.
- File path.
- DOI or URL if available.
- Evidence type: published evidence, formal documentation, personal observation, discussion note, conference takeaway, or user research idea.
- Privacy sensitivity.

If important source context is missing, ask the user before updating the wiki unless it is clearly a low-risk quick note.

## Source Storage and Naming

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The wiki should not depend on raw source files being available after cloning.

Use this default source ID and filename convention for raw files and source references:

```text
YYYY-MM-DD_author-or-org_short-title.ext
```

Examples:

```text
2026-05-18_smith_smart-home-caregiving-review.pdf
2026-05-18_nih_ai-digital-health-report.docx
2026-05-18_conference-session_fall-risk-sensing-notes.md
```

If exact publication date is unknown, use the source date available in the citation. If no source date is available, use the ingest date and mark the source date as unknown in the source context.

## Human Review Policy

For major sources such as papers, reports, dissertations, formal documentation, policy documents, or important files:

1. Read the source.
2. Create an ingest preview under `outputs/ingest_previews/`.
3. Summarize proposed wiki updates.
4. Ask for confirmation before updating wiki pages.

For short quick notes or personal takeaways:

1. Source-track the note.
2. Mark evidence type clearly.
3. Automatically update the wiki only when risk is low and the source context is clear.

## Ingest Steps

1. Read `AGENTS.md`, `MEMORY.md`, and `INDEX.md`.
2. Identify source type, evidence type, privacy level, and source context.
3. Save or reference the raw source under `sources/` if a durable source artifact is provided and local storage is appropriate.
4. Treat raw source files as immutable after saving.
5. For major sources, create an ingest preview before wiki updates.
6. Extract source-backed findings, methods, populations, technologies, contexts, limitations, and open questions.
7. Separate evidence from interpretation, personal insight, and speculative design direction.
8. Identify relevant wiki targets.
9. Update pages under `wiki/` only after preview confirmation when required.
10. Update `INDEX.md` if pages or summaries changed.
11. Update `MEMORY.md` after major milestones.
12. Append a concise `ingest` entry to `LOG.md`.

## Common Wiki Targets

- Population implications -> `wiki/populations/`
- Condition overlay implications -> `wiki/conditions/`
- Caregiver needs -> `wiki/caregiving_challenges/`
- Care recipient needs -> `wiki/care_recipient_needs/`
- Technology implications -> `wiki/technologies/`
- Home or care setting context -> `wiki/environments/`
- Conceptual distinctions -> `wiki/concepts/`
- Evidence summaries -> `wiki/evidence/`
- Design implications -> `wiki/design_patterns/`
- Gaps and study ideas -> `wiki/research_questions/`

## Required Separations

- Caregiver needs vs care recipient needs.
- Disease, disability, aging-related decline, and age-associated prevalence.
- Published evidence vs personal observation.
- Evidence-backed finding vs interpretation.
- Current evidence vs speculative design direction.
- Research support vs clinical decision-making.

## Privacy and Security Check

Before saving or integrating content, check whether it contains:

- PHI.
- Identifiable participant information.
- Clinical records.
- Direct quotes that may identify a person.
- Sensitive study data.
- Contact information.
- Location or timing details that could enable re-identification.

If yes, pause and ask the user how to handle it unless a safe handling policy is already provided.

## Required LOG.md Update

Every completed ingest must append a `LOG.md` entry in the same turn.

Use this format:

```text
## [YYYY-MM-DD] ingest | Source title or note topic

- Summary: Integrated or previewed [source/note] for [topic].
- Files touched: `sources/[file]` if applicable, `outputs/ingest_previews/[file]` if applicable, `wiki/[page].md`, `INDEX.md` if changed, `LOG.md`.
- Notes: Mention source type, evidence type, privacy level, review status, and unresolved gaps.
```
