---
title: Output Policy, Knowledge, and Structure Health Check
type: lint_report
status: complete
privacy: private
last_updated: 2026-07-14
---

# Output Policy, Knowledge, and Structure Health Check

## Scope

This health check validated the new selective-output policy and reviewed the maintained wiki for knowledge and structural consistency. It covered 154 Markdown pages under `wiki/`, including 42 evidence pages and 36 citation-memory items, plus governing files, discovery surfaces, workflows, commands, and durable output routing.

Checks included:

- contradictions, stale claims, and conceptual boundary risks;
- frontmatter and evidence-label consistency;
- source IDs, source-file targets, citation-memory backlinks, and reference-item index coverage;
- index coverage, weak incoming links, duplicate-title intent, and stable repo-path references;
- privacy and identifiable-data markers;
- living overview, synthesis, reference-plan, workflow, command, index, and memory freshness;
- local-only versus selectively trackable output boundaries;
- raw-source retention and citation-memory backfill needs.

## Findings and Fixes

### No critical knowledge conflict found

No direct contradiction was found in the maintained wiki around disease versus normal aging, caregiver versus care-recipient needs, AI or smart-home effectiveness, usability versus clinical outcomes, or autonomous healthcare decision-making. Current pages generally preserve evidence limits and distinguish design rationale from effectiveness evidence.

No obvious PHI, direct participant identifiers, or broken citation-record targets were found in the maintained wiki. All 36 citation-memory items are routed from `INDEX.md` and contain the expected citation-status, export-readiness, and original-citation sections.

### Evidence metadata consistency fixed

Five older evidence pages had source tracking and citation-memory links but lacked an explicit `evidence_type`. Added the matching reviewed evidence category:

- Hartnett 2016: `published evidence`.
- Mohammed 2023: `published qualitative evidence`.
- National Academies 2016: `formal report`.
- Schulz 2020: `published evidence`.
- Van Houtven 2011: `published evidence`.

The Setiawan 2019 evidence page already had a canonical reference item, but its frontmatter lacked the backlink. Added the existing `reference_item` path without changing source claims.

### Navigation and cross-link consistency fixed

Six existing templates were absent from the template section of `INDEX.md`; all template files are now listed.

Two design patterns were reachable from `INDEX.md` but had no clear incoming topic/design links:

- `ai_and_wearable_augmented_caregiver_support.md` is now linked from the caregiver self-care and health-tracking hub.
- `care_recipient_style_prompting_for_empathy.md` is now linked from the AI-assisted pre-clinic preparation pattern.

The duplicate title `Biomarker-Stratified Neurorehabilitation` is intentional rather than a duplicate ownership problem: one page owns the design pattern and the other owns research questions, and the pages link to each other.

### Output policy validated

Ignore behavior now matches the documented policy:

- `outputs/ingest_previews/`, `outputs/_scratch/`, and generated `outputs/citation_exports/` files are ignored by default.
- `outputs/citation_exports/README.md` and `.gitkeep` remain trackable.
- evidence briefs, prompts, query answers, and lint reports remain selectively trackable.

This report is durable because it records policy decisions, fixes, and residual risks. Routine no-change checks should remain in chat rather than accumulating report files.

## Residual Gaps and Limits

### Citation-memory backfill

Four older citation-bearing evidence pages predate the current citation-memory workflow and lack canonical reference items:

- the family caregiver generative-AI HCD AMIA submission abstract;
- the SCI pre-clinic ChatGPT/ChatGPT Health AMIA submission abstract;
- the systemic sclerosis-associated Raynaud mHealth usability AMIA submission abstract;
- the family caregiver mHealth doctoral dissertation.

Their approved previews contain useful author/title/source context, but publication status and canonical original-citation text should be reviewed before records are created. No citation fields were invented during this check. Two presentation-takeaway pages also lack reference items, which is acceptable unless the underlying lectures are later treated as formally citation-bearing sources.

### Concurrent durable outputs

Two output files appeared after the initial clean worktree check and were treated as concurrent work:

- `outputs/evidence_briefs/2026-07-14_agentic-family-caregiver-support_design-evidence-brief.md`;
- `outputs/query_answers/2026-07-14_agentic-cg-support_readme_cross-check.md`.

The concurrent task marked both ready and added a durable `LOG.md` entry. This health check added `INDEX.md` routes, and publication validation added the repo-standard `last_updated: 2026-07-14` field without changing either output's substantive content.

### Raw-source retention

The local source layer currently contains 45 non-placeholder files, and the preview layer contains 47 local preview artifacts. No source was deleted. Many raw files remain useful for claim verification and citation repair, so this check does not recommend blanket cleanup. Any later deletion review should be source-by-source and user-approved.

### Knowledge gaps

The check did not add external evidence. Existing gaps remain around comparative AI-wiki versus vector-RAG performance, caregiver-specific multi-agent effectiveness, long-term digital intervention maintenance, and technology-specific smart-home effectiveness. These remain research questions rather than contradictions in current synthesis.

## Files Updated by the Health Check

- `INDEX.md`
- `MEMORY.md`
- five evidence pages receiving explicit evidence-type labels
- the Setiawan 2019 evidence page
- the caregiver self-care and health-tracking hub
- the AI-assisted pre-clinic preparation design pattern
- this lint report

No living overview or caregiver-system synthesis update was needed because this check changed workflow policy, metadata, and routing without adding or changing domain evidence.
