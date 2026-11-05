---
title: November 2026 Knowledge and Repository Health Check
type: lint_report
status: ready
privacy: private
last_updated: 2026-11-05
---

# November 2026 Knowledge and Repository Health Check

## Outcome and Scope

No blocking maintained-wiki or publication issue remains after the fixes below. Source reporting limitations and open research questions remain labeled; they are not unresolved errors in the compiled wiki.

The structural/citation scan covers all 209 wiki pages, including 65 evidence pages and 63 citation records. Semantic review focuses on the six approved November sources, the affected topic/design/research owners, both living overviews, adjacent caregiver intervention and digital-inclusion evidence, and targeted contradiction/staleness/gap scans across the compiled wiki. This is not an independent reanalysis of study datasets, a full re-reading of every older source, or a new external literature search.

## Findings and Fixes

- Replaced two stale "To be further source-backed" care-recipient connection placeholders in the emotional-support and information-literacy hubs. The new links preserve caregiver versus care-recipient outcomes and do not claim downstream benefit from needs studies.
- Updated current source-category lists in the source documentation, ingest workflow, domain map, and memory after the approved self-management/psychosocial-support extension. Kept breast-cancer patient evidence separate from caregiver evidence and gynecological cancer.
- Refreshed current citation/page totals and both living overviews; retained explicitly dated historical totals as history. The staged caregiver core reference plan remains unchanged.
- Source-specific numerical/measurement cautions stay on evidence pages, with concise constraints at reuse points. No inconsistent Kano ranking was promoted into a fixed design requirement.

## Contradictions and Stale Claims

- Wang's structured review and earlier qualitative studies provide a needs/technology mapping, not a validated assessment tool or pooled comparative effectiveness result. Its broad technology discussion does not supersede outcome-specific caregiver trial evidence or establish caregiver AI benefit.
- Silva's selected qualitative caregiver sample adds information practices and appraisal difficulties, not prevalence or educational effectiveness. Reported dementia-as-normal-aging beliefs remain misconceptions, not wiki assertions.
- Nyamathi evaluates fictional composite design artifacts and stakeholder perceptions. The 36 evaluations come from 15 people; only two were family caregivers and no persons with dementia participated. Neither design ratings nor adapted PPS scores establish clinical benefit or AI/robot performance.
- Svendsen's patient-only stress-management trial found no statistically significant overall intervention advantage at 18 months. This does not contradict beneficial caregiver interventions in other populations/designs, prove equivalence, or negate all psychosocial interventions. Exploratory subgroups are not a replacement for the primary result.
- Vandelli's proxy-inferred trust/adoption classes are separate from validated trust measurement, observed ability, and actual sustained use. Cross-sectional class/regression findings cannot establish a causal adoption pathway.
- Xianheng's sensitivity formula/values, category counts, and age bins are inconsistent. The source is retained for bounded exploratory requirement elicitation; quantitative ranks, uncertain subgroup tests, unmeasured willingness to pay, and retrospective case alignment are not treated as firm priorities or effectiveness evidence.
- The new shared synthesis separates caregiver needs, care-recipient design context, older-adult preferences/attitudes, and patient outcomes. Disease, disability, and aging-related changes remain distinct.

## Structure, Citation Memory, and Privacy

- YAML parsing and duplicate-key checks passed across maintained wiki pages and checked navigation/durable outputs.
- Required frontmatter, source IDs, DOI uniqueness, evidence/reference matching, reciprocal links, documented current paths, Markdown targets, index routing, and approved topic backlinks passed.
- All 63 citation-bearing evidence sources have citation-memory records; 60 are RIS-ready. Three AMIA submissions remain intentionally incomplete. Fridriksson and Koroshetz remain the two presentation-takeaway exceptions.
- No orphan wiki page or non-template index-only entry was found. Five index-only templates are intentional entry points; other templates have additional incoming links.
- Bibliographic readiness is separate from evidence strength. Article numbers are preserved as identifiers rather than PDF page ranges. Publisher/NCBI author indexing for Xianheng is explicitly documented; missing optional fields remain omitted.
- Pattern scans and targeted review found no obvious participant email, DOB, medical-record identifier, pseudonymous individual story, or actual care profile introduced into maintained knowledge. Such scans do not guarantee detection of every identifier. Public citation author names are bibliographic metadata.
- Source methods/results remain on evidence pages; citation fields/writing roles remain in reference records; topic/design pages and overviews contain concise synthesis and labeled hypotheses.

## Knowledge Gaps and Follow-Up

These gaps do not block publication of bounded synthesis:

- Direct caregiver outcomes, sustained use, care-recipient safety, human response capacity, and real-world implementation require evidence beyond the new needs, perception, preference, and proxy-measure studies.
- Validate adapted persona measures, involve persons with dementia appropriately, and test contextual personalization prospectively. Validate trust measures and distinguish pre-adoption expectations from experienced trust.
- Clarify or verify Kano reporting before precision-dependent numerical reuse; include nonusers and people with substantial disability in requirements studies. Affordability and willingness-to-pay were not directly measured there.
- Svendsen's subgroup-targeting implications require confirmatory studies and direct caregiver-population evidence before transfer. Main-article supplementary estimates and datasets were not comprehensively retrieved.
- Compassion fatigue, relational strain, and digital trust currently fit existing emotional-support and supported-use owners. Reconsider dedicated concept pages if further sources require a richer synthesis; do not duplicate the source taxonomy prematurely.
- Existing foundational WHO/ICOPE, Pearlin/Lazarus, and implementation-framework source coverage remains incomplete. The postpartum scaffold and some care-recipient/time-burden connections need stronger direct evidence. External primary-source searches would be needed before stronger claims; none is implied by this ingest.
- Previously documented optional bibliographic gaps, including Hwang's exact date, Almeida's final fields, and Tu's final publication fields, remain unverified rather than fabricated.

## Source Retention and Pending Intake

Retain the five new publisher PDFs and Nyamathi's complete PMC JATS XML for audit and later review, especially where reporting/measurement limits matter. All six SHA-256 hashes are unchanged. Nyamathi's XML preserves main text and tables; linked images and supplementary assets are not a complete local archive.

Svendsen moved unchanged into `sources/papers/monthly_pubmed/self_management_and_psychosocial_support/`. The original intake manifest remains immutable; separate integration metadata records the current paths. No raw source was deleted or recommended for deletion in this pass. Historical filenames in append-only logs may refer to earlier source locations; current evidence/reference paths were checked.

PMIDs 42981790, 42981698, and 42949683 still await manual full-text retrieval and later preview. The pediatric procedural-VR paper also needs scope review if supplied. The previously unassigned Nallo smart-home PDF remains pending triage. None is silently treated as ingested evidence.

## Repository and Publication Boundary

- The starting worktree had only the current November task's `LOG.md` edits; no staged or unrelated tracked change was present.
- `main` tracks `origin/main`. A live fetch matched the starting revision before the authorized publication sequence.
- Raw sources, source-side metadata, ingest previews, extraction/rendering scratch, generated exports, private notes, and OS files remain ignored or outside the publication set. The new source folder's `.gitkeep` preserves structure without publishing article contents.
- This meaningful health report is intentionally durable, privacy-safe, indexed, and logged. No generated citation export is included.
- Commit/push is explicitly authorized by the user conditional on no blocking issue. Commit title: `:books: docs(pubmed): ingest November papers and audit wiki [ci skip]`. The final staged-set check verifies the exact publication contents; actual commit/push success is reported in the chat handoff.

## Follow-Up Check After Scratch Cleanup

At the user's subsequent request, repeated the knowledge check before repository checks and publication of the cleanup/workflow changes. Used temporary inline commands without creating a new persistent helper script.

- Rechecked all 209 wiki pages, 65 evidence pages, and 63 citation records (60 RIS-ready): YAML/duplicate keys, metadata, source/reference/DOI uniqueness, reciprocal links, current source paths/hashes, navigation, and targeted privacy checks passed. The two presentation exceptions and three incomplete AMIA records remain intentional.
- Reviewed the November evidence against the emotional-support, supported-use, outcome-evaluation, and living-synthesis owners. Found no new blocking contradiction or overstatement. The patient trial's null overall result, formative persona scope, proxy-trust limits, and Kano reporting cautions remain attached to reuse.
- Corrected stale folder enumerations in `INDEX.md` and `AGENTS.md` to include the already approved self-management/psychosocial-support category. Recorded the completed cleanup and future cleanup step in `MEMORY.md`.
- Residual knowledge gaps remain as documented above, including the postpartum scaffold, stronger direct care-recipient/time-burden evidence, foundational coverage, and three unavailable November sources. No new external search, source ingest, or source deletion occurred.
- Canonical source hashes and unique NCBI provenance remain intact after cleanup. The removed batch scripts and intermediate files are no longer workflow dependencies. Reviewed previews and pending-source handoff remain local-only.
- The follow-up repository check covers the exact pending Markdown publication set, ignored artifacts, tracked-code inventory, branch/upstream state, and staged whitespace/content. It does not add a software build or test suite to this Markdown-only wiki. The user explicitly requested the follow-up commit and push; the chat handoff records its result.
- Follow-up repository result: `main` matched a live-refreshed `origin/main`; no pre-staged or unrelated pending files were present. Only six intended Markdown files changed. Raw sources, previews, and metadata remain ignored; no Python file is tracked, and the removed batch scratch directory is absent. Whitespace checks passed. Follow-up commit title: `:books: docs(workflow): record cleanup and refresh routing [ci skip]`.
