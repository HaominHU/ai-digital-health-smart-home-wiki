---
title: Deep Overview and Knowledge Conflict Compliance Check
type: lint_report
status: complete
privacy: private
last_updated: 2026-06-17
---

# Deep Overview and Knowledge Conflict Compliance Check

## Scope

This check focused on files that could contaminate future wiki behavior after the old staged-ingest workflow:

- `wiki/overview/domain_map.md`
- `wiki/overview/caregiver_system_core_sota_synthesis.md`
- `wiki/references/cg_system_core_reference_plan.md`
- `AGENTS.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`
- `wiki/workflows/` and `wiki/commands/`
- Topic pages under `wiki/conditions/`, `wiki/populations/`, `wiki/technologies/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/`, `wiki/design_patterns/`, `wiki/research_questions/`, and `wiki/concepts/`
- Source-level pages under `wiki/evidence/`

## Checks Run

- Searched for old staged-ingest residue such as `Part 5`, `Part 6`, `Part 7`, `pre-ingest`, `next planned`, and `not yet ingested`.
- Checked overview pages for source-by-source evidence synthesis that should live in evidence pages, reference items, topic pages, or SoTA synthesis.
- Checked source 22 and source 27 boundaries for conflicts with the background-only rule.
- Checked conceptual boundaries around dementia vs normal aging, gynecological cancer vs aging, SCI vs aging-related decline, AI method evidence vs caregiver evidence, smart-home claims, mHealth effectiveness claims, and intervention-effectiveness claims.
- Checked evidence frontmatter for blank source IDs.

## Findings and Fixes

1. `wiki/overview/domain_map.md` was still too close to an evidence synthesis.
   - It listed top-level evidence anchors by source family.
   - This could recreate the original failure mode where the domain map becomes stale after a few ingests.
   - Fix applied: changed the page to a routing/governance map and removed source-by-source evidence-anchor bullets.

2. Some current-state files still used one-time batch wording.
   - `INDEX.md`, `MEMORY.md`, and `wiki/overview/caregiver_system_core_sota_synthesis.md` described the synthesis as the completed `cg_system_core` Tier 1 ingest.
   - Fix applied: changed this to current integrated `cg_system_core` evidence.

3. `MEMORY.md` retained one old `Part 2 integrated sources` heading.
   - Fix applied: changed it to `Current CareBuddy integrated sources`.

4. `wiki/evidence/bressan_2020_dementia_caregiver_needs_mixed_method_review.md` still called Bressan 2020 the `part 5` dementia-needs anchor.
   - Fix applied: changed it to the current dementia-needs anchor.

5. Source ID frontmatter check found apparent blank `source_ids:` lines for two presentation-note evidence pages.
   - Manual inspection showed both use valid multiline YAML lists and have source files:
     - `wiki/evidence/koroshetz_2026_neuroscience_takeaways_sci_translation.md`
     - `wiki/evidence/fridriksson_2026_brain_health_aphasia_recovery.md`
   - No fix needed.

6. Redundant source 22/source 27 boundary language in the reference-plan tables was tightened.
   - Fix applied: added a `background_only` status and moved the detailed restriction text to one source-specific boundary section.

7. No direct knowledge conflicts were found in the checked topic/evidence pages for:
   - Dementia as normal aging.
   - Gynecological cancer as an aging issue.
   - SCI as aging-related decline.
   - AI architecture papers as caregiver outcome evidence.
   - Smart-home-adjacent sources as smart-home effectiveness evidence.
   - Formative mHealth evidence as mHealth effectiveness evidence.
   - Source 22 or source 27 as PDF ingest targets.

## Residual Risk

Historical `LOG.md` entries still mention older part numbers and old workflow states. That is acceptable because `LOG.md` is append-only chronology. Future agents should use `MEMORY.md`, `INDEX.md`, current workflows, and the live reference plan for current state, not old log entries.

The remaining source-family details in `wiki/overview/caregiver_system_core_sota_synthesis.md` are appropriate because that page is explicitly the living synthesis owner. They should not be copied into `domain_map.md`.
