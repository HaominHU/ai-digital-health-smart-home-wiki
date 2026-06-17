---
title: Wiki Structure, Knowledge, Logic, and Workflow Check
type: lint_report
status: complete
privacy: private
last_updated: 2026-06-17
---

# Wiki Structure, Knowledge, Logic, and Workflow Check

## Scope

This check reviewed the maintained wiki structure, knowledge design, logic boundaries, and workflow guardrails, with special attention to stale overview/domain-map evidence and growing overlap after repeated ingests.

Files checked included `AGENTS.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`, `wiki/overview/domain_map.md`, `wiki/overview/caregiver_system_core_sota_synthesis.md`, `wiki/workflows/`, `wiki/commands/`, and the `cg_system_core` reference plan.

## Findings

1. `wiki/overview/domain_map.md` was stale.
   - It still had `last_updated: 2026-06-01`.
   - Its evidence section listed only two early stress-process/caregiver health anchors even though later caregiver-system, dementia, SCI, cancer, implementation, and AI architecture sources had been integrated.
   - Fix applied: converted the section into an evidence map with routing anchors and major evidence families rather than a partial source list.

2. The workflow layer did not require overview/synthesis maintenance after ingest.
   - `wiki/workflows/ingest_source.md` required `INDEX.md`, `MEMORY.md`, and `LOG.md` updates but did not explicitly require checking affected overview or synthesis pages.
   - Fix applied: added a living overview/synthesis maintenance step and a deferral-note rule.

3. Knowledge ownership boundaries were implicit.
   - Evidence pages, topic pages, overview pages, reference plans, design patterns, and research questions all existed, but the governing files did not clearly say which layer owns which type of knowledge.
   - This increased the risk of duplicated summaries and overlapping pages.
   - Fix applied: added a knowledge ownership rule to `AGENTS.md`, `domain_map.md`, and `ingest_source.md`.

4. The lint workflow did not explicitly check stale living maps.
   - `wiki/workflows/lint_wiki.md` covered stale index entries and duplicate concepts but not stale domain maps, living syntheses, reference plans, workflow files, command files, or memory.
   - Fix applied: expanded lint checks to include those files and added commands for finding stale part-number or synthesis language.

5. Some workflow/source-lane text was outdated.
   - `AGENTS.md`, `INDEX.md`, `MEMORY.md`, and `wiki/workflows/ingest_source.md` still contained older `cg_system_core` part-status language in places.
   - Fix applied where it governed future behavior: future agents are directed to use `wiki/references/cg_system_core_reference_plan.md` as the live status map instead of relying on old part numbers.

## Current Logic Boundaries

- Evidence pages should carry source-level detail and limits.
- Reference item pages should carry citation memory and export readiness.
- Overview pages should carry routing and high-level synthesis, not full source duplication.
- Topic pages should carry concise reusable implications by population, condition, challenge, need, technology, environment, or concept.
- Design pattern pages should carry design implications and constraints, clearly separating evidence-backed logic from speculative design direction.
- Research question pages should carry gaps and future study ideas.

## Residual Risks

- A full semantic duplicate-page review was not completed for all 146 wiki Markdown files. The added workflow rules should reduce future overlap, but a later dedicated pass could still consolidate older repeated summaries.
- This cleanup removed stale part-based planning language and duplicate domain-map/index pointers from the main guidance layer. Some older topic pages may still contain more source-level detail than ideal. They were not rewritten in this pass to avoid broad uncontrolled refactoring.
- `outputs/ingest_previews/` remains local-only and ignored as expected; this check did not publish or stage preview files.

## Files Updated

- `AGENTS.md`
- `wiki/overview/domain_map.md`
- `wiki/workflows/ingest_source.md`
- `wiki/workflows/lint_wiki.md`
- `wiki/workflows/query_wiki.md`
- `wiki/commands/ingest_source.md`
- `wiki/commands/lint_wiki.md`
- `wiki/commands/README.md`
- `wiki/references/cg_system_core_reference_plan.md`
- `INDEX.md`
- `MEMORY.md`
- `LOG.md`
- `outputs/lint_reports/2026-06-17_wiki_structure_knowledge_workflow_check.md`
