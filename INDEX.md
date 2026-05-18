---
title: AI Digital Health and Smart Home Wiki Index
type: index
status: draft
privacy: private
last_updated: 2026-05-18
---

# AI Digital Health and Smart Home Wiki Index

## Project Overview

This repo is a private research wiki for AI-driven digital health and smart home technologies in caregiving, chronic conditions, disability, and aging.

The wiki is designed as a Markdown knowledge middleware layer: readable by humans, maintainable by AI agents, compatible with Obsidian, and structured enough for future vector DB or RAG use.

## Root-Level Control Files

- `AGENTS.md`: Agent operating rules, privacy boundaries, source rules, and wiki conventions.
- `CLAUDE.md`: Claude-compatible pointer to `AGENTS.md`.
- `README.md`: Project overview and usage summary.
- `INDEX.md`: Content-oriented wiki map.
- `LOG.md`: Chronological append-only project log.
- `MEMORY.md`: Compressed current-state digest.

## Raw Source Layer

- `sources/papers/`: Published papers and paper notes.
- `sources/reports/`: Reports, dissertations, white papers, and formal documents.
- `sources/abstracts/`: Abstracts and short publication records.
- `sources/conference_notes/`: Conference notes and session takeaways.
- `sources/presentation_notes/`: Notes from talks, seminars, and presentations.
- `sources/documentation/`: Technical, policy, or product documentation.
- `sources/personal_notes/`: User-provided quick notes and research ideas.
- `sources/attachments/`: Attachments associated with source records.

Raw sources should be treated as immutable.

## Wiki Layer

- `wiki/overview/`: Project overview and domain maps.
- `wiki/populations/`: Population pages.
- `wiki/conditions/`: Condition overlay pages.
- `wiki/caregiving_challenges/`: Reusable caregiver challenge hubs.
- `wiki/care_recipient_needs/`: Care recipient needs tracked separately from caregiver needs.
- `wiki/technologies/`: Technology lens pages.
- `wiki/environments/`: Home, clinic, community, and hybrid care contexts.
- `wiki/concepts/`: Cross-cutting conceptual distinctions.
- `wiki/evidence/`: Evidence summaries and source-backed synthesis.
- `wiki/design_patterns/`: Reusable intervention and system design patterns.
- `wiki/research_questions/`: Research gaps, open questions, and study ideas.
- `wiki/specs/`: Research, design, and system specification pages.
- `wiki/workflows/`: Repeatable maintenance workflows.
- `wiki/commands/`: Short command templates for Codex.
- `wiki/templates/`: Reusable page templates.

## Outputs

- `outputs/ingest_previews/`: Human-review previews before major source integration.
- `outputs/evidence_briefs/`: Evidence summaries generated from the wiki.
- `outputs/research_prompts/`: AI-ready research and writing prompts.
- `outputs/design_prompts/`: AI-ready design prompts.
- `outputs/spec_prompts/`: AI-ready system or study specification prompts.
- `outputs/query_answers/`: Durable answers worth preserving outside chat.
- `outputs/lint_reports/`: Wiki health-check reports.

## Privacy-Sensitive Space

- `private_notes/`: Sensitive scratch space and private working notes.

Do not store identifiable participant data, PHI, clinical records, or raw sensitive study material unless the user explicitly provides a safe handling policy.

## Initial Conceptual Pages

- `wiki/overview/domain_map.md`: Overall research domain map.
- `wiki/concepts/aging_vs_disease.md`: Distinguishes aging-related decline from disease and disability.
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`: Separates caregiver needs from care recipient needs.
- `wiki/concepts/multimorbidity_and_overlapping_needs.md`: Tracks overlapping needs and interacting causes.

## Initial Population Pages

- `wiki/populations/family_caregivers.md`
- `wiki/populations/older_adults.md`
- `wiki/populations/people_with_chronic_conditions_and_disabilities.md`

## Initial Condition Pages

- `wiki/conditions/spinal_cord_injury.md`
- `wiki/conditions/dementia.md`
- `wiki/conditions/falls_and_aging.md`
- `wiki/conditions/multiple_chronic_conditions_in_aging.md`
- `wiki/conditions/gynecological_cancer.md`

## Initial Technology Pages

- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/technologies/smart_home_technologies.md`

## Workflows

- `wiki/workflows/ingest_source.md`
- `wiki/workflows/query_wiki.md`
- `wiki/workflows/lint_wiki.md`
- `wiki/workflows/generate_research_prompt.md`
- `wiki/workflows/generate_design_spec_prompt.md`

## Command Templates

- `wiki/commands/README.md`
- `wiki/commands/ingest_source.md`
- `wiki/commands/quick_note.md`
- `wiki/commands/ask_wiki.md`
- `wiki/commands/lint_wiki.md`
- `wiki/commands/generate_research_prompt.md`
- `wiki/commands/generate_design_spec_prompt.md`
