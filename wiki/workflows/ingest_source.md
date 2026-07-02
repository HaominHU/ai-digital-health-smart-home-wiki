---
title: Ingest Source Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-07-02
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
- Original citation text or enough metadata to reconstruct a citation, when the source is citation-bearing.

If important source context is missing, ask the user before updating the wiki unless it is clearly a low-risk quick note.

## Source Storage and Naming

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The wiki should not depend on raw source files being available after cloning.

For paper sources, preserve the purpose-specific lane when assigning or updating source paths. New purpose-specific folders may be created under `sources/papers/` when a stable new source group emerges.

- Use `sources/papers/cg_system_core/` for the ongoing numbered caregiver system-design core citation ingest. Check `wiki/references/cg_system_core_reference_plan.md` for the live staged-ingest status, integrated sources, future sources, and background-only source markers.
- Use `sources/papers/monthly_pubmed/` for monthly PubMed push papers before triage, prioritization, preview, or integration. Use the current provisional topic-lens subfolders when storing selected papers: `adoption_preferences_and_equity/`, `ai_interaction_and_decision_support/`, `caregiving_support_systems/`, and `smart_home_and_ambient_care/`. Assign by the paper's primary contribution, not every secondary theme; revise the taxonomy when future monthly papers create repeated conflicts.
- Use top-level `sources/papers/` only for legacy papers, standalone papers, or papers not yet assigned to a purpose-specific lane.

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

Do not infer confirmation from broad wording such as "ingest this paper", "start ingesting", or a task list that includes ingest as a later step. Treat those requests as authorization to store or reference the source and prepare a preview, not as authorization to integrate the source into maintained wiki pages. Only skip the approval pause when the user explicitly says they have reviewed and approved the specific preview, or explicitly waives preview review for that turn.

For short quick notes or personal takeaways:

1. Source-track the note.
2. Mark evidence type clearly.
3. Automatically update the wiki only when risk is low and the source context is clear.

## Ingest Steps

1. Read `AGENTS.md`, `MEMORY.md`, and `INDEX.md`.
2. Identify source type, evidence type, privacy level, and source context.
3. Save or reference the raw source under `sources/` if a durable source artifact is provided and local storage is appropriate.
4. Treat raw source files as immutable after saving.
5. For major sources, create an ingest preview and wait for explicit user approval before wiki updates.
6. Extract source-backed findings, methods, populations, technologies, contexts, limitations, and open questions.
7. Separate evidence from interpretation, personal insight, and speculative design direction.
8. Identify relevant wiki targets and the knowledge owner for each target.
9. For citation-bearing sources, create or update a citation-memory record under `wiki/references/items/` using `wiki/templates/reference_item_template.md`.
10. Preserve the original citation text and mark whether the record is RIS export-ready.
11. Update pages under `wiki/` only after preview confirmation when required.
12. Check affected overview and synthesis pages, especially `wiki/overview/domain_map.md`, `wiki/overview/caregiver_system_core_sota_synthesis.md`, and any relevant reference plan. Update them when the source changes high-level knowledge, or record a short deferral reason in `LOG.md`.
13. Update `INDEX.md` if pages or summaries changed.
14. Update `MEMORY.md` after major milestones, workflow decisions, or significant wiki growth.
15. Append a concise `ingest` entry to `LOG.md`.

## Knowledge Ownership Check

Before editing multiple pages, assign each extracted item to its primary owner:

- Source-level findings and evidence limits -> `wiki/evidence/`.
- Bibliographic metadata, citation text, writing roles, and export readiness -> `wiki/references/items/`.
- Staged source status, source numbers, and background-only source markers -> relevant reference plans such as `wiki/references/cg_system_core_reference_plan.md`.
- Cross-wiki state, high-level synthesis, and routing -> `wiki/overview/`.
- Reusable topic synthesis -> populations, conditions, caregiving challenges, care-recipient needs, technologies, environments, and concepts.
- Design implications and constraints -> `wiki/design_patterns/`.
- Gaps and study ideas -> `wiki/research_questions/`.

Do not copy a full source summary into every mapped page. Topic pages should keep concise source-backed implications and links; evidence pages should carry the detailed source picture.

## Source-Type Extraction Depth

Match the extraction depth to the source type. Do not let review papers collapse into generic summaries, and do not let single studies lose the full study picture.

For systematic reviews, scoping reviews, meta-analyses, and evidence syntheses, capture:

- Review question and inclusion logic.
- Search date range, databases, study designs, and screening scope when available.
- Included population and condition scope, including whether the review directly supports a priority wiki condition or only broad caregiver/digital health context.
- Technology or intervention taxonomy, including concrete delivery modes, intervention components, and whether the source is AI-specific, smart-home-specific, broader digital health, telehealth, or non-technology intervention evidence.
- Outcome taxonomy, including caregiver outcomes, care-recipient outcomes, usability/acceptability outcomes, implementation outcomes, and evidence-quality ratings when available.
- Equity, access, cultural, linguistic, accessibility, and human-centered design details, especially when the source mentions marginalized or underserved caregivers.
- Review-level takeaway: what the review adds beyond repeating included studies.
- What the review does not answer, including unsupported condition-specific, clinical-effectiveness, AI-agent, smart-home, or implementation claims.

For single empirical studies, capture a compact full-study picture:

- Problem or gap addressed.
- Population, care-recipient condition, setting, and relationship context.
- Intervention, system, exposure, or phenomenon studied.
- Key innovation or distinguishing contribution.
- Study design, methods, sample, and measures.
- Main results and primary takeaway.
- Evidence limits, including whether the source supports feasibility, usability, acceptability, mechanism, association, or effectiveness.
- Direct wiki mapping across caregiver needs, care-recipient needs, condition overlays, technology lenses, design patterns, and evaluation logic.

## Common Wiki Targets

- Population implications -> `wiki/populations/`
- Condition overlay implications -> `wiki/conditions/`
- Caregiver needs -> `wiki/caregiving_challenges/`
- Care recipient needs -> `wiki/care_recipient_needs/`
- Technology implications -> `wiki/technologies/`
- Home or care setting context -> `wiki/environments/`
- Conceptual distinctions -> `wiki/concepts/`
- Evidence summaries -> `wiki/evidence/`
- Citation memory -> `wiki/references/items/`
- Design implications -> `wiki/design_patterns/`
- Gaps and study ideas -> `wiki/research_questions/`

## Required Separations

- Caregiver needs vs care recipient needs.
- Disease, disability, aging-related decline, and age-associated prevalence.
- Published evidence vs personal observation.
- Evidence-backed finding vs interpretation.
- Current evidence vs speculative design direction.
- Research support vs clinical decision-making.

## Citation Memory Check

For papers, dissertations, reports, formal documentation, conference abstracts, proceedings, and other citation-bearing sources:

- Preserve the original citation in `wiki/references/items/`.
- Store one canonical Markdown citation-memory record per source.
- Link the citation record to relevant evidence and topic pages.
- Record writing roles such as introduction, background, significance, design rationale, methods rationale, limitation, or gap framing.
- Mark `export_ready: true` only when the minimum RIS fields are known.
- Use `outputs/citation_exports/` only for generated export files, not canonical storage.
- Do not invent missing bibliographic metadata.

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
- Notes: Mention source type, evidence type, privacy level, citation-memory status, review status, and unresolved gaps.
```
