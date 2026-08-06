# AI Digital Health and Smart Home Research Wiki

> A private research Wiki for building structured, source-tracked knowledge about AI-driven digital health and smart home technologies for caregiving, chronic conditions, disability, and aging. This project treats Markdown Wiki files as a human-editable knowledge middleware layer: rigorous enough for research synthesis and future retrieval systems, but readable and correctable by humans.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**🎯 Research Focus:** AI-Driven Digital Health, Smart Home Technologies, Family Caregiving, Chronic Conditions, Disability, Aging

**🧠 Knowledge Architecture:** Markdown + YAML, Source Tracking, Evidence Labeling, Knowledge-Level Citation Memory, Research Prompt Generation, Design/Spec Prompt Generation, Future RAG Preparation

**📊 Status:** WIP / Private Research Wiki

---

## 🧭 Project Overview

This repo is currently private. It is designed for rigorous research knowledge management, not for public note-taking and not as part of an AI learning series.

The working repo supports source-backed synthesis, concept mapping, literature-informed system design, and AI-ready research/design/spec prompts. A sanitized public subset or reusable template may later be extracted, but the working wiki should preserve the full research context needed for serious domain work.

The wiki can inform general knowledge answers, research writing, system design, and knowledge support for agent reasoning. It must not act as a clinical decision-maker, diagnostic system, treatment recommender, or substitute for professional medical, ethical, privacy, security, or IRB review.

## 🏗️ Architecture

```text
Markdown Wiki + YAML Metadata
        ↓
Ingest: papers + reports + notes + documents
        ↓
Persistent Wiki synthesis
        ↓
Query: evidence-aware answers + concept maps
        ↓
Prompt generation: research + design + specs
        ↓
Outputs: briefs, prompts, and durable query answers
        ↓
Health check: contradictions + stale claims + structural gaps + knowledge gaps
```

This project explores how a domain-specific research Wiki can support ongoing scholarship and design reasoning without turning raw notes, study observations, or early ideas into unsupported evidence.

The structure follows the Karpathy-style LLM Wiki pattern in a research-specific way:

- `sources/` is the immutable raw source layer.
- `sources/papers/` can contain purpose-specific paper lanes as source groups emerge.
- `sources/papers/cg_system_core/` is an example lane for the ongoing numbered core citation set for caregiver system-design ingest.
- `sources/papers/monthly_pubmed/` is a storage lane for monthly PubMed pushes before triage and integration, currently organized by provisional topic-lens subfolders: adoption/preferences/equity, AI interaction and decision support, caregiving support systems, smart home/ambient care, and wearables/remote monitoring. Screened papers withdrawn from ingest are retained separately under `deferred_or_out_of_scope/`.
- `wiki/` is the maintained Markdown knowledge layer.
- `wiki/references/` is the knowledge-level citation-memory layer.
- `AGENTS.md` is the schema/control layer for Codex behavior.
- `INDEX.md` is content-oriented navigation.
- `LOG.md` is chronological logging.
- `MEMORY.md` is a compressed current-state digest.

Core operations:

- **Ingest:** integrate papers, abstracts, reports, documentation, conference notes, presentation notes, and quick research ideas into durable Wiki pages.
- **Query:** read the index and relevant Wiki pages to generate source-aware answers, comparisons, concept maps, evidence briefs, or research gaps.
- **Health check:** periodically run the Karpathy-style wiki knowledge lint for contradictions, stale claims, structural gaps, knowledge gaps, source tracking, weak evidence labels, privacy risks, conceptual conflation, stale paths, and future RAG readiness.
- **Repo health check:** check repository/worktree/git hygiene and publication safety, then ask whether to commit and push.
- **Generate prompts:** produce AI-ready research, writing, design, coding-plan, or specification prompts grounded in accumulated Wiki knowledge.
- **Citation-supported brainstorming:** use wiki citation memory to suggest citations for a manuscript idea, assess coverage quality, optionally supplement with searched external candidate citations, generate an AI feed prompt, and prepare separate Zotero/EndNote-compatible RIS content.

## 🧩 Research Model

- Conditions are overlays.
- Caregiving challenges are reusable hubs.
- Care recipient needs are tracked separately from caregiver needs.
- Technologies are reusable intervention lenses.
- Aging-related functional decline and age-associated disease development are distinguished.
- Evidence, interpretation, personal insight, and speculative design direction are separated.
- Source tracking is required for every ingested knowledge item.
- The wiki stores knowledge-level citation memory, while Zotero/EndNote remain paper-level reference managers for manuscript-specific collections.

Primary focus:

- AI-driven digital health
- Smart home technologies

Primary population focus:

- Family caregivers of people with chronic conditions and disabilities
- Family caregivers of older adults

Secondary population focus:

- People with chronic conditions and disabilities themselves
- Older adults themselves

Condition priority:

1. Spinal cord injury
2. Dementia
3. Falls and general aging issues
4. Multiple chronic conditions in aging
5. Systemic sclerosis-associated Raynaud phenomenon
6. Postpartum women
7. Gynecological cancer

## 🪜 How to Use This Wiki

This repo is meant to be maintained by prompting Codex directly. The files in `wiki/commands/` are reusable instruction recipes, not terminal commands. You can copy/paste the command text when needed, but usually a short plain-English trigger is enough.

Start a new Codex session in this repo and say one of these:

```text
Ingest this PDF paper into the wiki: /path/to/paper.pdf
```

```text
Quick note: [your note]

Source context: my own research idea from [meeting/event/date].
Please integrate if low-risk and mark it as a research idea, not evidence.
```

```text
Ask wiki: What does the wiki currently know about smart home monitoring for family caregivers of people with dementia?
```

```text
Generate a research prompt about [topic] using the wiki.
```

```text
Brainstorm citations for a paper about [topic]. Give me an AI feed prompt and a Zotero/EndNote RIS list.
```

```text
Generate a design/spec prompt for [system idea] using the wiki.
```

```text
Health check
```

```text
Repo health check
```

For a paper, report, dissertation, formal document, or other major source, Codex should create an ingest preview first under `outputs/ingest_previews/`, then wait for explicit review approval before updating the wiki. A broad request to "ingest" means prepare the source and preview, not integrate into maintained wiki pages, unless preview approval is explicit.

For a short low-risk note, Codex may integrate it directly if source context is clear.

Useful command recipe files:

- `wiki/commands/ingest_source.md`
- `wiki/commands/quick_note.md`
- `wiki/commands/ask_wiki.md`
- `wiki/commands/lint_wiki.md`
- `wiki/commands/repo_health_check.md`
- `wiki/commands/generate_research_prompt.md`
- `wiki/commands/generate_design_spec_prompt.md`

## 📥 Source Handling

You have three simple options:

1. Put the raw file in `sources/` yourself, then ask Codex to ingest it.
2. Give Codex a local file path and ask it to copy/store the file under `sources/` before ingesting.
3. Give Codex a DOI, URL, or external file path and ask it to reference the source without storing a local copy.

Recommended prompt for a PDF:

```text
Ingest this PDF paper into the wiki.

File: /path/to/paper.pdf
Source type: published paper
Evidence type: published evidence
Title: [paper title]
Authors: [authors]
Year/date: [year]
DOI/URL: [doi or url if available]

Please copy/store it under sources/ using the repo filename convention, then create an ingest preview before updating wiki pages.
```

Raw source storage rules:

- Raw files may be stored locally under `sources/`, but raw source contents are ignored by git by default.
- Use source IDs and filenames like `YYYY-MM-DD_author-or-org_short-title.ext`.
- If you provide only a DOI or URL, Codex should record the source reference. It should download or store a copy only if you ask and access is available.
- If you provide an external local file path, Codex can copy it into `sources/` when you ask it to store the source.
- Citation-bearing sources should get a Markdown citation-memory record under `wiki/references/items/`, preserving the original citation and export-readiness status.
- Generated Zotero/EndNote-compatible exports should go under `outputs/citation_exports/`; RIS is the default export format.
- Periodic lint checks should flag locally stored raw sources that may be removable after successful wiki digestion.
- Do not delete raw source files automatically.

Output durability rules:

- See `outputs/README.md` for the full output policy.
- Keep ingest previews, `outputs/_scratch/`, and generated citation exports local-only by default.
- Track briefs, prompts, query answers, and lint reports only when they are intentionally durable, privacy-safe, and useful beyond the current chat or run.
- Save meaningful lint reports that document findings, fixes, decisions, or residual risks; routine no-change checks do not need a report file.
- Do not ignore the entire `outputs/` tree because selected generated Markdown files are part of the wiki's reusable research and audit history.

Release-safe public subset rule:

- Extract only blank templates, generic workflows, sanitized examples, and non-private instructions.
- Do not include identifiable participant data, PHI, raw sensitive notes, private study material, unpublished observations, or personal metadata.
- Keep the private working Wiki and any public template/framework as separate artifacts.

## 🗂️ Structure

```text
AGENTS.md                         Agent operating rules, privacy boundaries, and research schema
CLAUDE.md                         Claude-compatible pointer to AGENTS.md
MEMORY.md                         Compressed project state and decisions
INDEX.md                          Human-readable Wiki map
LOG.md                            Chronological project log

wiki/overview/                    Domain maps and high-level orientation
wiki/populations/                 Population pages
wiki/conditions/                  Condition overlay pages
wiki/caregiving_challenges/       Reusable caregiver challenge hubs
wiki/care_recipient_needs/        Care recipient needs tracked separately
wiki/technologies/                AI, digital health, and smart home technology lenses
wiki/environments/                Home, clinic, community, and hybrid care contexts
wiki/concepts/                    Cross-cutting conceptual distinctions
wiki/evidence/                    Source-backed evidence summaries
wiki/design_patterns/             Reusable intervention and system design patterns
wiki/research_questions/          Research gaps, questions, and study ideas
wiki/specs/                       Research, design, and system specification pages
wiki/references/                  Knowledge-level citation memory and reference records
wiki/workflows/                   Repeatable research Wiki workflows
wiki/commands/                    Reusable short Codex command templates
wiki/templates/                   Reusable page templates

outputs/README.md                 Output durability and publication policy
outputs/ingest_previews/          Local-only human-review previews before major source integration
outputs/_scratch/                 Local-only temporary generated work
outputs/evidence_briefs/          Generated evidence summaries
outputs/research_prompts/         AI-ready research and writing prompts
outputs/design_prompts/           AI-ready design prompts
outputs/spec_prompts/             AI-ready system or study specification prompts
outputs/query_answers/            Durable answers worth preserving outside chat
outputs/lint_reports/             Wiki health-check reports
outputs/citation_exports/         Local-only-by-default Zotero/EndNote exports, usually RIS

sources/papers/                   Published papers and paper notes
sources/reports/                  Reports, dissertations, white papers, and formal documents
sources/abstracts/                Abstracts and short publication records
sources/conference_notes/         Conference notes and session takeaways
sources/presentation_notes/       Notes from talks, seminars, and presentations
sources/documentation/            Technical, policy, or product documentation
sources/personal_notes/           User-provided quick notes and research ideas
sources/attachments/              Attachments associated with source records
private_notes/                    Sensitive scratch space and private working notes
```

This repo can be opened directly as an Obsidian vault. `INDEX.md` is the main map, and `MEMORY.md` is the compressed current-state digest.

## 📌 Existing Wiki Entries

Initial scaffold pages:

- `wiki/overview/domain_map.md`
- `wiki/concepts/aging_vs_disease.md`
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`
- `wiki/concepts/multimorbidity_and_overlapping_needs.md`
- `wiki/populations/family_caregivers.md`
- `wiki/populations/older_adults.md`
- `wiki/populations/people_with_chronic_conditions_and_disabilities.md`
- `wiki/conditions/spinal_cord_injury.md`
- `wiki/conditions/dementia.md`
- `wiki/conditions/falls_and_aging.md`
- `wiki/conditions/multiple_chronic_conditions_in_aging.md`
- `wiki/conditions/systemic_sclerosis_associated_raynaud_phenomenon.md`
- `wiki/conditions/postpartum_women.md`
- `wiki/conditions/gynecological_cancer.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/technologies/smart_home_technologies.md`

These pages are scaffolds, not evidence summaries. Source-backed claims should be added through the ingest workflow.

## 📄 License & Acknowledgments

**License:** MIT. See [LICENSE](LICENSE).

**AI Tools Used:**

- ChatGPT - Architecture brainstorming and research workflow design.
- Claude - Potential research writing and synthesis support.
- Codex CLI/Desktop - Repo setup, Wiki maintenance, source ingest, linting, and structured file updates.

**Acknowledgments:**

- [Karpathy-style LLM Wiki / personal Wiki concepts as architecture inspiration](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f).
- The research-specific structure is customized for AI-driven digital health, smart home technologies, caregiving, chronic conditions, disability, and aging.

---

*Private research Wiki | Last updated: July 2026*
