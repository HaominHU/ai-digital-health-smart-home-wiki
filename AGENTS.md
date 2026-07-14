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

Knowledge ownership rule:

- `wiki/evidence/` pages own source-level summaries and limits.
- `wiki/references/items/` pages own citation memory, writing roles, and export readiness.
- `wiki/overview/` pages own cross-wiki maps and living syntheses; they should not become duplicate source summaries.
- `wiki/conditions/`, `wiki/populations/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/`, `wiki/technologies/`, and `wiki/environments/` own reusable topic-level synthesis.
- `wiki/design_patterns/` owns design implications and constraints, clearly labeled as evidence-backed or speculative.
- `wiki/research_questions/` owns gaps, study ideas, and future research directions.

When new evidence touches a living overview or synthesis page, update that page in the same turn or add a short explicit deferral note to `LOG.md` explaining why it was not updated.

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
- Treat `outputs/citation_exports/` as a regenerable, local-only-by-default export layer. Track a specific export only when the user explicitly asks to preserve or publish it.
- Use RIS as the default Zotero/EndNote-compatible export format unless the user requests another format.
- Do not store topic-specific RIS files as canonical citation memory.
- Do not invent citations, authors, venues, DOIs, URLs, dates, or bibliographic fields.

Raw source files may be stored locally under `sources/`, but they are ignored by git by default because they may be private, copyrighted, sensitive, or too large for GitHub. Do not assume raw source files are available after cloning unless they are explicitly provided.

Paper source organization:

- `sources/papers/`: Published paper source layer. Purpose-specific paper lanes may be added under this folder as new source groups emerge.
- `sources/papers/cg_system_core/`: Example purpose-specific lane for the ongoing key citation set for caregiver system-design evidence ingest. This is the current lane for numbered caregiver-system core papers and related background-only source markers. Use `wiki/references/cg_system_core_reference_plan.md` as the live status map instead of relying on old part numbers in chat context.
- `sources/papers/monthly_pubmed/`: Example purpose-specific lane for monthly PubMed push papers before they are selected, prioritized, or integrated. Use provisional topic-lens subfolders: `adoption_preferences_and_equity/`, `ai_interaction_and_decision_support/`, `caregiving_support_systems/`, and `smart_home_and_ambient_care/`. Assign by the paper's primary contribution, not every theme it touches; revisit the taxonomy when future papers conflict with these categories.
- Papers that remain directly under `sources/papers/` are legacy, standalone, or not yet assigned to one of the purpose-specific lanes.

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

For major sources such as papers, reports, dissertations, formal documentation, policy documents, or important files, produce an ingest preview and wait for explicit user approval of that preview before updating the wiki.

Do not infer preview approval from broad wording such as "ingest this paper", "start ingesting", or a task list that includes ingest as a later step. Treat those requests as authorization to store or reference the source and prepare a preview, not as authorization to integrate the source into maintained wiki pages. Only skip the approval pause when the user explicitly says they have reviewed and approved the specific preview, or explicitly waives preview review for that turn.

For short quick notes or personal takeaways, automatic updates are acceptable if source context is clear and risk is low. Still log the source and mark the evidence type clearly.

When unsure whether to update automatically, create a preview first and ask for confirmation.

Do not rewrite large parts of the wiki without showing a summary of proposed changes first.

## 9. Wiki Architecture

Use Markdown as source knowledge and YAML frontmatter for structured metadata.

Core folders:

- `sources/`: Raw source layer. Preserve source files and source notes. Do not modify after saving except to add separate metadata files.
- `sources/papers/cg_system_core/`: Example purpose-specific lane for numbered caregiver system-design core citation papers in the ongoing staged ingest.
- `sources/papers/monthly_pubmed/`: Example purpose-specific lane for monthly PubMed push paper storage before triage or ingest, organized by provisional topic-lens subfolders when papers accumulate.
- `wiki/`: Maintained research wiki layer.
- `outputs/`: Generated artifacts such as ingest previews, evidence briefs, research prompts, design prompts, spec prompts, query answers, and lint reports.
- `private_notes/`: Sensitive scratch space and private working notes.

Output durability rule:

- Do not ignore all of `outputs/`; some generated Markdown artifacts are durable research records.
- Keep `outputs/ingest_previews/`, `outputs/_scratch/`, and generated files under `outputs/citation_exports/` local-only by default.
- Track evidence briefs, research/design/spec prompts, query answers, and lint reports only when they are intentionally durable, privacy-safe, and useful beyond the current chat or run.
- A lint report is worth tracking when it records meaningful findings, fixes, decisions, or residual risks. Routine no-change checks can remain in chat and need no report file.
- When a durable output is tracked, route it from `INDEX.md` when useful and record its creation in `LOG.md`.
- Use `outputs/README.md` as the detailed output-storage and publication policy.

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

## 10.1 Assistant Infrastructure and Context Design

Treat this repo as an agent-readable research operating system. Keep always-loaded instructions durable, concise, and operational; move lower-frequency procedures into workflows, command templates, or skills.

Claude Code and Codex use different names for similar assistant-infrastructure surfaces. For this repo:

- `AGENTS.md` is the canonical Codex project contract. `CLAUDE.md` may import or point to `AGENTS.md` for Claude Code compatibility, but duplicated parallel guidance should be avoided.
- Directory-specific Codex guidance should use nested `AGENTS.md` or `AGENTS.override.md` when a stable subtree truly needs different rules. Do not invent a `.claude/rules/` equivalent for Codex path rules.
- Codex `.rules` files are for command approval and sandbox policy, not for wiki content or path-scoped writing guidance.
- Repeatable workflows belong in `wiki/workflows/` and short user-facing triggers belong in `wiki/commands/`.
- Reusable agent procedures that need progressive disclosure, examples, scripts, or supporting references may become Codex skills under `.agents/skills/` when the workflow is stable enough to justify it.
- MCP or connector tools should be used only when live external data or an external action is required.
- Hooks are for deterministic enforcement or audit at lifecycle points, such as command policy, lightweight validation, or privacy checks. Do not put semantic research judgment or long-running wiki workflows into hooks.
- Subagents are for explicitly requested or clearly bounded noisy work such as broad read-only exploration, parallel review, log analysis, or summarization. Avoid parallel write-heavy wiki edits unless the user explicitly asks for that workflow and conflict handling is clear.

Context hygiene rules:

- Keep `AGENTS.md` focused on rules that should apply in nearly every session.
- Keep command output concise when running checks; prefer targeted `rg`, bounded file reads, and summarized test/lint output.
- For long or multi-phase work, preserve handoff state in the maintained wiki, `LOG.md`, `MEMORY.md`, or an explicit output file rather than relying on chat memory.
- If a recurring correction is repo-governing, update `AGENTS.md`, `MEMORY.md`, or the relevant workflow after user confirmation.
- If a recurring correction is task-specific, update the relevant workflow or command template instead of bloating the root instruction file.

## 11. Core Operations

### Ingest

Read a source or note, preserve the raw source, extract source-backed knowledge, produce a preview when needed, and update relevant wiki pages.

Major sources require an ingest preview and explicit user approval before wiki updates.

For citation-bearing sources, create or update the relevant Markdown citation-memory record under `wiki/references/items/` and mark whether the record is ready for RIS export.

For every ingest, decide whether the source changes any living overview, synthesis, domain map, reference plan, workflow, command, or memory page. If yes, update the affected page. If no, leave a concise `LOG.md` note such as "No overview or synthesis update needed because this source only adds source-level detail already covered by [page]."

### Query

Answer questions by reading `MEMORY.md`, `INDEX.md`, and relevant wiki pages. Clearly separate evidence-backed claims, interpretation, gaps, and speculative design directions. Cite or point to source-tracked wiki pages when useful.

If a query produces durable synthesis, ask whether to file it back into the wiki unless the user already requested that.

### Lint

When the user says "health check" without the word "repo", run the Karpathy-style wiki knowledge lint workflow. This means checking the maintained wiki itself, not preparing a commit or push.

The default health check must include:

- Contradictions: conflicting claims, incompatible evidence interpretations, or opposing data points across compiled pages.
- Stale claims: older assertions superseded, narrowed, or contradicted by newer ingested sources.
- Structural gaps: orphan pages, weak cross-links, missing backlinks, stale index entries, and broken routing between interrelated concepts.
- Knowledge gaps: important recurring concepts that lack dedicated pages, missing source coverage, and areas that may require external search before stronger claims can be made.

Also periodically check for missing source tracking, weak evidence labels, broken links, duplicate concepts, unsupported claims, privacy risks, conceptual conflation, and stale living overviews or synthesis pages after later ingests.

Also check whether locally stored raw sources should still be retained. If a source has been well digested into the wiki and does not need to remain locally stored, flag it for the user's review rather than deleting it automatically.

Also check for citation-bearing evidence sources that lack reference records, original citation text, evidence labels, or export-readiness status.

When the user says "repo health check", run repository/worktree health checks instead of the wiki knowledge lint by default. A repo health check includes git status, staged/unstaged/untracked files, ignored local-only artifacts, branch/remotes, and obvious infrastructure hygiene. After a repo health check, ask the user whether to commit and push; do not commit or push without explicit confirmation.

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
