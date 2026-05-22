# AGENTS.md

## 1. Project Purpose

This repo is a private research wiki for AI-driven digital health and smart home technologies, with a focus on caregiving, chronic conditions, disability, and aging.

The repo follows a Karpathy-style LLM Wiki pattern:

- Raw sources are preserved and treated as immutable.
- The maintained wiki is a human-readable Markdown layer generated and improved by an AI coding/research agent.
- This file is the governing instruction layer for source ingest, wiki updates, queries, linting, and downstream prompt generation.
- The wiki should compound over time as sources, notes, questions, and research ideas are added.

This is a domain-specific research operating system, not just a notes folder and not part of another project.

## 2. Scope and Decision Boundary

The wiki may inform:

- General knowledge answers.
- Evidence-grounded research writing.
- Literature synthesis.
- System design reasoning.
- AI-ready prompts for research, writing, coding, design, or specification work.
- Knowledge support for an agent's reasoning.

The wiki must not act as:

- A clinical decision-maker.
- A diagnostic system.
- A treatment recommendation system.
- A substitute for professional medical, legal, ethical, IRB, privacy, or security review.
- An autonomous agent that makes care decisions for caregivers, patients, older adults, or disabled people.

When generating downstream prompts, clearly state that the output is for research, design, or knowledge support unless the user explicitly defines another non-clinical use.

## 3. Research Domain

Primary domain focus:

- AI-driven digital health.
- Smart home technologies.

Primary population focus:

- Family caregivers of people with chronic conditions and disabilities.
- Family caregivers of older adults.

Secondary population focus:

- People with chronic conditions and disabilities themselves.
- Older adults themselves.

Condition priority:

1. Spinal cord injury.
2. Dementia.
3. Falls and general aging issues.
4. Multiple chronic conditions in aging.
5. Systemic sclerosis-associated Raynaud phenomenon.
6. Postpartum women.
7. Gynecological cancer.

## 4. Core Conceptual Model

Use this architecture when creating, updating, or querying wiki pages:

- Conditions are overlays.
- Caregiving challenges are reusable hubs.
- Care recipient concerns are tracked separately from caregiver concerns.
- Technologies are reusable intervention lenses.
- Aging-related functional decline and age-associated disease development must be distinguished.
- Sources are tracked.
- Citation memory is managed at the knowledge level.
- Evidence, interpretation, personal insight, and speculative design direction are separated.
- Specs and AI-ready prompts are generated from accumulated wiki knowledge.

Important distinctions:

- Do not treat disease conditions as normal aging.
- Do not treat disability as interchangeable with aging-related decline.
- Do not treat care recipient needs as caregiver needs.
- Do not treat caregiver observations or conference takeaways as established evidence.
- Support multimorbidity and overlapping needs among older adults.
- Track interacting causes when relevant, such as disease impairment, treatment effects, medication burden, home environment mismatch, aging-related decline, caregiver capacity, and technology constraints.

Examples:

- Acquired spinal cord injury in a 30-year-old is not the same as mobility or spinal function decline associated with aging.
- Gynecological cancer among older adults is a disease condition that may be age-associated or more prevalent with aging, not an aging issue by itself.
- Dementia in later life is not normal aging, even though it is highly relevant to older-adult caregiving.
- Falls may reflect general aging, disease-specific impairment, treatment side effects, medication burden, home environment mismatch, or multiple interacting causes.

## 5. Privacy, Data Security, and Sensitive Content Rules

This repo is private by default, but privacy must still be actively protected.

Do not store protected health information, identifiable participant data, clinical records, contact information, real names, full dates of birth, addresses, medical record numbers, raw transcripts with identifiable people, or identifiable field notes unless the user explicitly instructs it and provides a safe storage policy.

Default handling:

- Prefer de-identified or minimally necessary notes.
- Store sensitive raw material only under `private_notes/` or `sources/` with clear privacy labels.
- Integrate sensitive notes into the wiki only as de-identified, generalized, source-tracked English synthesis.
- Do not expose private notes in public-ready outputs.
- Do not include participant identifiers in generated prompts, specs, or writing outputs.
- Do not infer identities from context.
- Do not fabricate consent status, IRB status, recruitment status, or data-sharing permission.

For healthcare and study-related outputs, include privacy and security considerations when relevant:

- Data minimization.
- Consent and participant expectations.
- IRB or ethics review needs.
- Access control.
- De-identification.
- Data retention.
- Secure storage.
- Auditability.
- Risk of re-identification.
- Bias, fairness, and vulnerable-population concerns.
- Human oversight and escalation boundaries.

If a request appears to involve identifiable or sensitive data, pause and ask how the user wants it handled before saving or integrating it.

## 6. Language Rules

All repo files, wiki pages, file names, prompts, schema, templates, and generated outputs should be in English.

Some raw notes or user questions and responses may include Mandarin. Preserve Mandarin in raw sources if needed, but summarize and integrate it into the wiki in English.

Do not create Chinese-language wiki pages.

## 7. Source and Evidence Rules

Every ingested knowledge item must track its source.

Every ingested paper, report, dissertation, formal documentation source, or other citation-bearing source should also preserve its original bibliographic citation in the wiki's citation-memory layer when metadata is available.

Reference-management boundary:

- The wiki is the knowledge-level citation memory layer.
- Zotero and EndNote remain paper-level reference-management tools.
- Use the wiki to remember why a citation matters, what topics and claims it supports, and which writing roles it can serve.
- Use Zotero or EndNote for PDF management, citation styling, coauthor sharing, and manuscript-specific collections.

Default citation storage and export:

- Store canonical citation-memory records as Markdown under `wiki/references/items/`.
- Use `wiki/templates/reference_item_template.md` for new citation records.
- Treat `outputs/citation_exports/` as the generated export layer.
- Use RIS as the default Zotero/EndNote-compatible export format unless the user requests another format.
- Do not store topic-specific RIS files as canonical citation memory.
- Do not invent citations, authors, venues, DOIs, URLs, dates, or bibliographic fields.

Raw source files may be stored locally under `sources/`, but they are ignored by git by default because they may be private, copyrighted, sensitive, or too large for GitHub. Do not assume raw source files are available after cloning unless they are explicitly provided.

Use this default source ID and raw filename convention:

`YYYY-MM-DD_author-or-org_short-title.ext`

Examples:

- `2026-05-18_smith_smart-home-caregiving-review.pdf`
- `2026-05-18_nih_ai-digital-health-report.docx`
- `2026-05-18_conference-session_fall-risk-sensing-notes.md`

When the user provides input without source context, ask for missing source context before durable integration unless it is clearly a quick personal note. Source context may include:

- Title.
- Author, speaker, or organization.
- Event or venue.
- Date.
- Source type.
- File path.
- DOI or URL if available.
- Whether it is published evidence, personal observation, discussion note, conference takeaway, or the user's own research idea.

Separate these evidence categories:

- Published evidence.
- Formal documentation.
- Personal observation.
- Discussion note.
- Conference or presentation takeaway.
- User research idea.
- Interpretation or synthesis.
- Speculative design direction.

Do not invent citations, URLs, DOIs, study details, participant characteristics, effect sizes, claims, quotes, dates, or findings.

If evidence is missing, mark it clearly as a gap.

## 8. Human Review Rules

For major sources such as papers, reports, dissertations, formal documentation, policy documents, or important files, produce an ingest preview before updating the wiki.

For short quick notes or personal takeaways, automatic updates are acceptable if source context is clear and risk is low. Still log the source and mark the evidence type clearly.

When unsure whether to update automatically, create a preview first and ask for confirmation.

Do not rewrite large parts of the wiki without showing a summary of proposed changes first.

## 9. Wiki Architecture

Use Markdown as source knowledge and YAML frontmatter for structured metadata.

Core folders:

- `sources/`: Raw source layer. Preserve source files and source notes. Do not modify after saving except to add separate metadata files.
- `wiki/`: Maintained research wiki layer.
- `outputs/`: Generated artifacts such as ingest previews, evidence briefs, research prompts, design prompts, spec prompts, query answers, and lint reports.
- `private_notes/`: Sensitive scratch space and private working notes.

Wiki folders:

- `wiki/overview/`: Project overview and domain maps.
- `wiki/populations/`: Population pages.
- `wiki/conditions/`: Condition overlay pages.
- `wiki/caregiving_challenges/`: Reusable caregiver challenge hubs.
- `wiki/care_recipient_needs/`: Care recipient needs tracked separately.
- `wiki/technologies/`: Technology lens pages.
- `wiki/environments/`: Home, clinic, community, and hybrid care contexts.
- `wiki/concepts/`: Cross-cutting conceptual distinctions.
- `wiki/evidence/`: Evidence summaries and source-backed synthesis.
- `wiki/design_patterns/`: Reusable design directions and intervention patterns.
- `wiki/research_questions/`: Open questions, gaps, and study ideas.
- `wiki/specs/`: Generated or maintained system/research specification pages.
- `wiki/references/`: Knowledge-level citation memory and reference item records.
- `wiki/workflows/`: Repeatable maintenance workflows.
- `wiki/commands/`: Short Codex command templates.
- `wiki/templates/`: Page templates.

The repo root may be opened as an Obsidian vault. Keep Markdown files readable in Obsidian, preserve YAML frontmatter, and prefer stable relative repo paths when documenting file locations.

## 10. Navigation, Logging, and Memory

`INDEX.md` is the content-oriented wiki map. Update it when pages or structure change.

`LOG.md` is the chronological append-only project log. Append to it after meaningful ingests, queries, lint checks, architecture changes, workflow changes, generated outputs, or memory updates.

Use this parseable log heading format:

`## [YYYY-MM-DD] type | Short title`

Recommended types:

- `ingest`
- `query`
- `lint`
- `architecture`
- `workflow`
- `output`
- `prompt`
- `memory`

`MEMORY.md` is the compressed current-state digest. Update it after major workflow milestones, important architecture decisions, or significant wiki growth.

The user manually handles commits and git management. Do not commit, push, or manage branches unless the user explicitly asks.

## 11. Core Operations

### Ingest

Read a source or note, preserve the raw source, extract source-backed knowledge, produce a preview when needed, and update relevant wiki pages.

Major sources require an ingest preview before wiki updates.

For citation-bearing sources, create or update the relevant Markdown citation-memory record under `wiki/references/items/` and mark whether the record is ready for RIS export.

### Query

Answer questions by reading `MEMORY.md`, `INDEX.md`, and relevant wiki pages. Clearly separate evidence-backed claims, interpretation, gaps, and speculative design directions. Cite or point to source-tracked wiki pages when useful.

If a query produces durable synthesis, ask whether to file it back into the wiki unless the user already requested that.

### Lint

Periodically check for stale claims, missing source tracking, weak evidence labels, broken links, orphan pages, duplicate concepts, unsupported claims, privacy risks, and conceptual conflation.

Also check whether locally stored raw sources should still be retained. If a source has been well digested into the wiki and does not need to remain locally stored, flag it for the user's review rather than deleting it automatically.

Also check for citation-bearing evidence sources that lack reference records, original citation text, evidence labels, or export-readiness status.

### Generate Downstream Prompts

Generate AI-ready prompts for research writing, design work, system specification, coding plan mode, evidence synthesis, or agent knowledge support.

Prompts should include:

- Purpose.
- Target audience or downstream agent role.
- Relevant evidence and wiki context.
- Explicit evidence gaps.
- Privacy and security constraints.
- Clinical decision boundary.
- Required outputs.
- Review criteria.

### Citation-Supported Brainstorming

When the user brainstorms a paper, grant, proposal, or research idea and asks for citations, use the citation-supported brainstorming workflow.

Default behavior:

- Use wiki-first mode: start with stored citation-memory records and source-backed wiki pages.
- Evaluate citation coverage quality rather than using a fixed citation-count threshold.
- Treat coverage as weak when the wiki is missing foundational work, recent state-of-the-art work, population anchors, condition-specific anchors, technology/intervention anchors, or when available citations are too narrow for the proposed argument.
- Group citations by writing role, such as introduction, background, significance, population burden, condition context, technology rationale, methods/design rationale, and gap framing.
- Produce an AI feed prompt when requested or when useful for downstream drafting.
- Keep wiki citations and searched external candidate citations in separate sections.
- Produce separate Zotero/EndNote-compatible RIS lists for wiki citations and searched external candidates when enough metadata is available.
- Mark incomplete or not-export-ready citations rather than fabricating missing fields.
- Clearly identify evidence gaps and, if needed, ask whether to search externally for candidate foundational or state-of-the-art sources.
- Treat searched external citations as unreviewed candidates until ingested or otherwise reviewed; do not treat them as established wiki evidence.

## 12. Future RAG and Vector Search Readiness

Do not over-engineer the first version.

Prepare for future vector DB or RAG expansion by maintaining:

- Consistent YAML frontmatter.
- Source IDs.
- Evidence type labels.
- Stable file paths.
- Clear page summaries.
- Tags.
- Dates.
- Explicit source links or source file references.
- Citation-memory records and export-readiness labels for citation-bearing sources.

Do not add a database, embedding system, or custom tooling until the wiki has enough content to justify it.
