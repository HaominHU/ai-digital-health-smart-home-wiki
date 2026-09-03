---
title: Research Wiki Memory
type: memory
status: draft
privacy: private
last_updated: 2026-09-03
---

# Research Wiki Memory

## Current State

This repo has been initialized as a private Karpathy-style LLM Wiki for AI-driven digital health and smart home technologies in caregiving, chronic conditions, disability, and aging.

The repo is intentionally Markdown-first and Obsidian-compatible. No database, embedding system, or custom retrieval tooling has been added.

## Core Purpose

The wiki should support:

- General knowledge answers grounded in accumulated research context.
- Evidence-aware research writing.
- System design reasoning.
- AI-ready prompts for research, writing, coding, design, or specification work.
- Knowledge support for agent reasoning.

The wiki must not act as a clinical decision-maker, diagnostic system, treatment recommender, or substitute for professional medical, ethical, privacy, security, or IRB review.

## Architecture Decisions

- Raw sources live under `sources/` and are treated as immutable.
- Maintained wiki pages live under `wiki/`.
- Generated previews, briefs, prompts, and reports live under `outputs/`; `outputs/README.md` governs which artifacts remain local and which may become durable tracked records.
- Sensitive scratch notes live under `private_notes/`.
- Citation-memory records live under `wiki/references/items/`.
- Zotero/EndNote-compatible citation exports live under `outputs/citation_exports/` and are regenerable, local-only artifacts by default.
- `AGENTS.md` governs agent behavior.
- `INDEX.md` is the content-oriented map.
- `LOG.md` is the chronological timeline.
- `MEMORY.md` is the compressed current-state digest.

Assistant infrastructure baseline:

- `AGENTS.md` is the canonical Codex project contract. `CLAUDE.md` exists as a Claude-compatible import/pointer to `AGENTS.md`; avoid duplicating parallel guidance.
- Keep always-loaded guidance concise and durable. Put repeatable procedures in `wiki/workflows/` and short triggers in `wiki/commands/`; consider `.agents/skills/` only for stable reusable workflows that need progressive disclosure, scripts, examples, or references.
- Do not treat Codex `.rules` files as a `.claude/rules/` equivalent for path-scoped content instructions; Codex rules are for command approval/sandbox policy. Use nested `AGENTS.md` or `AGENTS.override.md` only when a subtree truly needs stable different guidance.
- Hooks are for deterministic lifecycle enforcement or audit, not semantic research judgment. Subagents are for explicitly requested or bounded noisy exploration, review, log analysis, or summarization.

Knowledge ownership baseline:

- `wiki/evidence/` pages own source-level summaries and limits.
- `wiki/references/items/` pages own citation memory, writing roles, and export readiness.
- `wiki/overview/` pages own cross-wiki maps and living syntheses, not duplicated full source summaries.
- Topic pages own reusable synthesis for their folder-level concept.
- `wiki/design_patterns/` owns design implications and constraints.
- `wiki/research_questions/` owns gaps and study ideas.

After future ingests, check whether `wiki/overview/domain_map.md`, `wiki/overview/caregiver_system_core_sota_synthesis.md`, relevant reference plans, workflow/command files, `INDEX.md`, and `MEMORY.md` need updating. If a living overview or synthesis is affected but not updated, add a short deferral note to `LOG.md`.

## Domain Model

- Conditions are overlays.
- Caregiving challenges are reusable hubs.
- Care recipient needs are tracked separately from caregiver needs.
- Technologies are reusable intervention lenses.
- Aging-related functional decline and age-associated disease development must be distinguished.
- Evidence, interpretation, personal insight, and speculative design direction must remain separate.
- The wiki is the knowledge-level citation memory layer; Zotero and EndNote remain paper-level reference managers for manuscript-specific collections.

Current condition priority order:

1. Spinal cord injury.
2. Dementia.
3. Falls and general aging issues.
4. Multiple chronic conditions in aging.
5. Systemic sclerosis-associated Raynaud phenomenon.
6. Postpartum women.
7. Gynecological cancer.

## Privacy and Security Baseline

The repo is private by default, but identifiable or sensitive healthcare/study data should not be stored unless the user explicitly provides a safe handling policy.

Default behavior:

- Avoid PHI and identifiable participant information.
- De-identify before wiki integration.
- Mark sensitive source material clearly.
- Include privacy, security, consent, ethics, data minimization, and human oversight considerations in healthcare-related prompts and specs.

## Source Storage and Git Baseline

The user manually handles commits and git management.

Commit messages follow the Haomin Hu-style standard:

- Default shape: `[:emoji: ]type(scope): subject`.
- First line is 72 characters or less.
- Subject uses present-tense imperative wording, starts lowercase, and has no final period.
- Use an applicable type such as `docs`, `update`, `fix`, `feat`, `refactor`, `test`, `chore`, `config`, `build`, `deps`, `security`, `performance`, or another listed repo-approved type.
- Documentation-only commits include `[ci skip]` in the title.
- Issue or pull-request references go after the first line.

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The tracked wiki should preserve source-derived knowledge through source IDs, source context, evidence labels, and durable Markdown synthesis.

Commit/publish guardrail for ingest previews:

- Major-source ingest requires explicit preview review and approval before maintained-wiki integration. A broad request to "ingest" authorizes source storage and preview preparation only; do not treat it as approval to update wiki pages unless the user explicitly approves the specific preview or waives review for that turn.
- Do not stage or push `outputs/ingest_previews/` files by default. The user has corrected this error twice. Ingest previews are local-only working artifacts unless the user explicitly asks to publish or track specific preview files in that turn.
- During caregiver-source ingest commit/push, stage maintained wiki files, evidence pages, citation-memory records, `INDEX.md`, `MEMORY.md`, `LOG.md`, and reference-plan updates, but leave ignored preview artifacts untracked.
- Do not use `git add -f outputs/ingest_previews/...` unless the user explicitly requests it. Before committing, run `git status --short --ignored` and verify preview files appear as ignored (`!!`), not staged.

Selective output durability baseline:

- Do not ignore the entire `outputs/` tree. Durable, privacy-safe Markdown evidence briefs, prompts, query answers, and meaningful lint reports may be tracked when they are deliberately preserved for reuse, audit history, or project handoff.
- Keep `outputs/ingest_previews/`, `outputs/_scratch/`, and generated citation exports under `outputs/citation_exports/` local-only by default. Track a specific normally local-only artifact only after an explicit user request covering that path.
- Routine no-change lint runs do not need a report file. Track a lint report when it preserves meaningful findings, fixes, decisions, or residual risks.
- Add durable outputs to `INDEX.md` when they need navigation and always record created durable outputs in `LOG.md`.

Paper sources now support a purpose-specific layer under `sources/papers/`. New source groups may get their own folders when a stable purpose emerges.

- `sources/papers/cg_system_core/`: Example lane for the ongoing numbered caregiver system-design core citation set. Use `wiki/references/cg_system_core_reference_plan.md` as the live status map for integrated, planned, skipped, future, and background-only sources.
- `sources/papers/monthly_pubmed/`: Example lane for monthly PubMed push storage before triage, selection, preview, or integration. Current provisional topic-lens folders are `adoption_preferences_and_equity/`, `ai_interaction_and_decision_support/`, `caregiving_support_systems/`, `smart_home_and_ambient_care/`, and `wearables_and_remote_monitoring/`. Assign by the paper's primary contribution. Retain screened but withdrawn sources under `deferred_or_out_of_scope/` rather than mixing them into active topic folders or deleting them.
- Top-level `sources/papers/` can still contain legacy, standalone, or not-yet-assigned papers.

Recommended raw source ID and filename pattern:

`YYYY-MM-DD_author-or-org_short-title.ext`

Periodic lint checks should flag locally stored raw sources that may be removable after their contents have been well digested into the wiki. Do not delete raw sources automatically.

Health-check trigger distinction:

- When the user says "health check" without "repo", run the wiki knowledge lint in `wiki/workflows/lint_wiki.md`: contradictions, stale claims, structural gaps, knowledge gaps, source tracking, privacy, citation memory, conceptual consistency, and stale overview/synthesis checks.
- When the user says "repo health check", run `wiki/workflows/repo_health_check.md`: git/worktree status, staged/unstaged/untracked/ignored files, local-only artifact boundaries, branch/upstream state, and publication hygiene. Then ask whether to commit and push; do not commit or push without explicit confirmation.

## Citation Management Baseline

Citation-bearing sources should have Markdown citation-memory records under `wiki/references/items/`.

Citation records should preserve original citation text, source IDs, evidence type, topic links, supported claims, writing roles, and export-readiness status. RIS is the default generated export format because it is compatible with Zotero and EndNote.

Use citation-supported brainstorming when the user is developing a manuscript idea and wants citations for introduction, background, significance, or related writing sections. Default to wiki-first mode: use stored wiki citations first and assess coverage quality rather than relying on a citation-count threshold.

When wiki coverage is weak, narrow, missing foundational sources, missing recent state-of-the-art sources, or missing population/condition/technology anchors, external seed search can supplement bibliography-building. Keep searched citations separate from wiki citations, label them as external candidates until reviewed or ingested, and create separate RIS exports for wiki citations and external candidates when files are requested.

## Current Operating State

The `sources/papers/cg_system_core/` lane uses `wiki/references/cg_system_core_reference_plan.md` as its live source-status map. Do not infer remaining work from old part numbers or older chat summaries.

`wiki/overview/caregiver_system_core_sota_synthesis.md` is now the living owner-facing SoTA synthesis for the current integrated `cg_system_core` evidence. Use it as the first high-level map for family caregiving outcomes, digital health intervention types/mechanisms/modalities, condition-specific dementia/SCI/gynecological cancer distinctions, evidence boundaries, and research directions to keep current after future relevant ingests.

Current lane status:

- The September 2026 monthly PubMed five-paper preview was explicitly approved and integrated on 2026-09-03. Almeida, Chamberlin, Fernandez Cajavilca, Hwang, and Tong now have evidence pages and RIS-ready citation records. Hwang's exact publication date and Almeida's final volume/issue/pages remain unverified optional metadata; do not fabricate them for export.
- AlzCare and Aliviado add dementia caregiver app design, short-session usability, and coproduction evidence, not effectiveness. Preserve implemented-versus-planned functionality and caregiver-versus-care-recipient evaluation distinctions. Aliviado's recommendation explanations and caregiver disagreement are design requirements, not algorithm safety validation.
- Chamberlin adds older-US-veteran caregiver service-access context: similar rural/urban interest does not guarantee equal receipt. Do not infer causes or that a digital referral tool closes the gap.
- Hwang and Tong add older-adult observational inclusion evidence, not caregiver intervention effects. Hwang excluded diagnosed and suspected dementia; Tong measured heterogeneous device ownership, not actual use or integrated smart-home performance.
- `wiki/concepts/digital_inclusion_and_supported_use.md` now owns access/connectivity/skills/assistance/use/outcome distinctions. `wiki/caregiving_challenges/formal_service_access_and_respite.md` owns service-access and respite pathways. Neither is a validated causal model.
- Tong remains under adoption/preferences/equity by primary contribution, with smart-home and wearable cross-links. The user reviewed and accepted this borderline routing; it is not a reason to duplicate the PDF or relabel it as a direct smart-home system evaluation.

- Current monthly PubMed source organization uses provisional topic-lens subfolders rather than a flat folder.
- The August 2026 monthly PubMed batch has completed the preview-approval-integration workflow. Ding, Fritz, Hong, Kolakowski, Pemberton, and Richter are integrated with evidence pages and RIS-ready citation-memory records. Talotta remains preserved under `deferred_or_out_of_scope/` without maintained-wiki evidence or citation-memory representation because it is rheumatoid-arthritis-specific and contains no Raynaud evidence.
- `2026-07-31_ding_wearable-healthcare-bibliometric-analysis`: Use as a large wearable-healthcare field map with preserved scale, cluster, burst, and internal-consistency details; do not use bibliometric prominence as clinical effectiveness evidence.
- `2026-07-23_fritz_community-in-the-loop-smart-home-monitoring`: Use as feasibility and implementation evidence for ambient sensing plus a tiered human response network in low-income, multilingual settings. The source introduces digital distress and does not establish diagnostic accuracy or effectiveness.
- `2026-07-24_hong_caregiver-activation-concept-analysis`: Caregiver activation is now a cross-wiki assessment and tailoring concept spanning care capabilities, autonomy, resilience, self-efficacy, and communication. Low activation must not be framed as blame or permission to shift professional responsibility.
- `2026-07-28_kolakowski_digital-health-intrinsic-capacity-feasibility`: Use as short-term healthy-aging platform feasibility and usability evidence with country variation, device burden, connectivity, and training limits; it does not validate AI performance or health benefit.
- `2026-07-15_pemberton_smart-home-connected-care-adoption`: Use as shared, caregiver-mediated smart-home adoption evidence with relational value, permissions, reliability, and setup implications; not effectiveness evidence.
- `2026-07-31_richter_llm-physician-patient-communication-review`: Use as narrow early evidence on perceived empathy in written LLM communication while keeping accuracy, safety, trust, authentic empathy, relationship quality, and clinical outcomes separate.
- `2026_kingsada_preferences-digital-health-technologies`: Kingsada et al. 2026 Health Economics Review scoping review on patient preferences toward digital health technologies has been previewed and integrated from the monthly PubMed lane.
- `2026-06-16_chen_generative-ai-meaning-centered-care-later-life`: Chen and Jin 2026 Frontiers in Psychiatry perspective on GenAI as interactional infrastructure for meaning-centered care in later life has been integrated from the monthly PubMed lane. Use as conceptual AI interaction, dignity, life-review, and governance rationale, not as effectiveness evidence.
- `2026-06-24_zhai_smart-home-technologies-ageing-in-place`: Zhai et al. 2026 Australasian Journal on Ageing systematic review on smart home technologies for ageing in place has been integrated from the monthly PubMed lane. Use as direct smart-home evidence with heterogeneity and implementation limits.
- `2026-06-16_mahmood_telehealth-informal-caregivers`: Mahmood et al. 2026 Frontiers in Public Health HINTS6 study on telehealth utilization among middle-aged and older informal caregivers has been integrated from the monthly PubMed lane. Use as caregiver telehealth utilization evidence, not intervention-effectiveness evidence.
- SCI caregiver sources 16-18 and 20-21 and gynecologic/cancer caregiver sources 23-25 and 28 have already been integrated; do not describe them as future ingest targets without rechecking the live reference plan.
- Sources 22 and 27 are background-only web sources, not local PDF ingest targets.

Monthly PubMed preference-method anchor:

- `2026_kingsada_preferences-digital-health-technologies`: Broad patient-preference scoping review for digital health technologies, including eHealth, telehealth, telemedicine, and mHealth. Use as patient-preference, adoption, HTA/reimbursement, preference-methods, older-adult digital health preference, and privacy/security design rationale. Do not use as caregiver-specific evidence, intervention-effectiveness evidence, AI-agent evidence, or smart-home effectiveness evidence.

A useful next step is the next genuinely unintegrated `cg_system_core` branch from the reference plan or a later lint/source-status pass checking citation export readiness, orphan pages, stale overviews/syntheses, evidence limits, and whether ignored preview/source artifacts should be retained locally.

September 2026 health-check state:

- The maintained wiki has 185 pages, 53 evidence summaries, and 51 citation records (48 RIS-ready). The two lecture-note exceptions and three incomplete AMIA records remain intentional.
- Chamberlin's receipt comparisons apply to 226 searchers, not all 511 respondents; more rural respite searching does not establish a respite-receipt difference.
- Hwang's table/narrative and confidence-limit reporting discrepancies are preserved as source limitations; verify before precision-dependent quantitative reuse. Only one of nine moderated-mediation contrasts was significant. These issues do not establish or negate a causal effect because the design is observational.
- `outputs/lint_reports/2026-09-03_knowledge-and-repo-health-check.md` records the semantic scope, structural validation, source caveats, residual evidence needs, and publication boundaries. Raw sources remain retained and local-only.

2026-06-17 structure/workflow check:

- `wiki/overview/domain_map.md` had become stale after later ingests because its evidence section still listed only two early anchors. It is now a routing and governance page, not a partial evidence synthesis.
- Future ingest and lint work must check stale living overview/synthesis pages and knowledge ownership boundaries, especially evidence pages vs topic pages vs overview pages vs reference plans vs design patterns.
- `outputs/lint_reports/2026-06-17_wiki_structure_knowledge_workflow_check.md` records the structure, knowledge, logic, and workflow findings.

2026-07-14 output-policy and wiki health check:

- `outputs/README.md` now owns the selective output durability policy. Ingest previews, scratch work, and generated citation exports remain local-only by default; privacy-safe briefs, prompts, query answers, and meaningful lint reports may be tracked deliberately.
- The validation found no direct maintained-wiki knowledge conflicts, broken citation-record targets, missing indexed reference items, or obvious PHI/identifier exposure.
- Low-cost structural fixes added five missing evidence-type labels, restored the Setiawan evidence-to-reference backlink, indexed all templates, and added incoming links to two weakly connected design patterns.
- Citation-memory backfill for the three 2026-05-18 AMIA submission abstracts and the caregiver mHealth dissertation was completed during the 2026-08-06 health check. The dissertation record is RIS-ready. The three abstract records remain explicitly incomplete and not export-ready until acceptance or publication status, final venue, date, pages, DOI, and URL are verified.
- `outputs/lint_reports/2026-07-14_output-policy-knowledge-structure-health-check.md` records scope, fixes, limits, and residual risks.

Background-only source boundary:

- Do not look for or create a source 22 PDF in `sources/papers/cg_system_core/`. Source 22 is the NINDS spinal cord injury knowledge website (`https://www.ninds.nih.gov/health-information/disorders/spinal-cord-injury`) and should be checked only when disease-background knowledge is needed. It should not be treated as caregiver-specific, intervention-effectiveness, digital health, AI, or smart-home evidence.
- Do not look for or create a source 27 PDF in `sources/papers/cg_system_core/`. Source 27 is the NCI PDQ family caregiver professional page (`https://www.cancer.gov/about-cancer/coping/family-friends/family-caregivers-hp-pdq?utm_source=chatgpt.com`) and should be checked only when cancer caregiver background, framework, or clinical-context knowledge is needed. It should not be treated as local PDF evidence, intervention-effectiveness evidence, AI, digital health, or smart-home evidence unless a later reviewed source directly supports those claims.

Completed dementia caregiver sources after the updated core-list trim:

- `2020_cheng_meta-review-dementia-caregiver-interventions`: Cheng and Zhang 2020 comprehensive meta-review of dementia caregiver intervention reviews.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Bressan, Visintini, and Palese 2020 mixed-method systematic review of dementia caregiver needs.
- `2021_ruggiano_chatbots-dementia-caregivers`: Ruggiano et al. 2021 systematic review of chatbot functions and quality for people with dementia and caregivers.

Reference planning file:

- `wiki/references/cg_system_core_reference_plan.md`: Planning-only map for the full caregiver system core reference backbone, including current integrated coverage, future sources, background-only source markers, and writing roles. This file is not canonical citation memory and should not be treated as evidence until individual sources are previewed and integrated.

Source-gap notes:

- AHRQ 2020 is intentionally skipped for now because it is very long, over 500 pages, and not practical for this staged ingest batch.
- Previously integrated but deprioritized material is retained in the wiki and moved to the 30+ source-number range when applicable, rather than being deleted.

First integrated source:

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: AMIA abstract on human-centered design recommendations for generative AI in mHealth apps for family caregivers.

New source-backed hubs from the first ingest:

- Caregiver time burden and engagement.
- Information access and health literacy.
- Emotional and social support.
- Adaptive AI layer for caregiver mHealth.
- Trajectory-sensitive caregiver content.

Condition mapping note:

- Broad "neurological conditions" evidence may be mapped cautiously to spinal cord injury when there is no specific non-SCI neurological condition mention, while preserving the source wording and avoiding unsupported SCI-specific claims.

Second integrated source:

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`: AMIA abstract on usability evaluation and iterative refinement of a Raynaud mHealth app for people with systemic sclerosis-associated Raynaud phenomenon.

New source-backed hubs from the second ingest:

- Symptom self-reporting and tracking.
- Accessibility-first mHealth symptom reporting.
- Real-world reliability for mHealth data capture.

Condition mapping note:

- Raynaud usability evidence maps directly to systemic sclerosis-associated Raynaud phenomenon. Older-adult relevance is limited to accessibility/usability barriers noted in the source and should not be treated as evidence that SSc-RP is normal aging.

Third integrated source:

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AMIA abstract comparing source-reported ChatGPT and ChatGPT Health interfaces for spinal cord injury pre-clinic preparation without connected records.

New source-backed hubs from the third ingest:

- Pre-clinic preparation and advocacy.
- AI-assisted pre-clinic preparation.
- Care-recipient-style prompting for empathy.

AI product/model note:

- Product and model details from this abstract are source-reported and may change. Re-verify current product capabilities before making current-state claims about OpenAI products.

Fourth integrated source:

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Hu's 2024 University of Pittsburgh dissertation on developing a multi-component mHealth app for family caregivers of people with chronic conditions and disabilities.

New source-backed hubs from the fourth ingest:

- Care coordination and shared access.
- Caregiver self-care and health tracking.
- Adaptive modular caregiver mHealth.
- One-stop caregiver support app.
- AI and wearable-augmented caregiver support.

Dissertation condition mapping note:

- Map dissertation condition-specific content only to spinal cord injury and gynecological cancer for current wiki purposes. Spina bifida, cerebral palsy, and traumatic brain injury remain source-level study-composition details unless the user later changes the condition priority list.

Fifth integrated source:

- `2019-04-25_setiawan_adaptive-mhealth-self-management`: Setiawan et al. 2019 JMIR Formative Research paper on iMHere 2.0 as adaptive mHealth self-management infrastructure for people with chronic conditions and disabilities.

System foundation note:

- Setiawan 2019 and Hu's dissertation jointly ground the user's caregiver research, system infrastructure, and future system expansion. Setiawan 2019 anchors the adaptive mHealth infrastructure for PwCCD self-management; Hu's dissertation extends the research line toward family caregiver support, caregiver-specific modules, and future AI/wearable/clinical workflow expansion.

New source-backed hubs from the fifth ingest:

- Self-management and secondary complication prevention.
- Adaptive mHealth self-management platform.
- Clinician portal-supported mHealth.

Sixth integrated batch:

- `2020_schulz_family-caregiving-for-older-adults`: Annual Review of Psychology review on family caregiving for older adults, caregiver role complexity, chronic stress exposure, caregiver impacts, risk factors, intervention evidence, and technology-based intervention cautions.
- `2016_nasem_families-caring-for-an-aging-america`: National Academies consensus report on U.S. family caregiving for older adults, caregiver definitions, prevalence, policy, caregiver assessment, person- and family-centered care, LTSS/health-system integration, economic support, and technology innovation.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: BMC Geriatrics article providing a framework for caregiver intervention activities, caregiver outcomes, care-recipient outcomes, utilization, and economic evaluation.

New source-backed hubs from the sixth integrated batch:

- Caregiving as chronic stress exposure.
- Caregiving activities vs outcomes.
- Caregiver assessment and triage.
- Caregiver intervention evaluation core outcomes.
- Person and family-centered care coordination.
- Caregiver intervention implementation and evaluation.

Systematic ingest rule:

- For future caregiver or digital health sources, classify population scope, condition scope, caregiver challenge, care-recipient need, technology lens, environment, intervention target/mechanism, evaluation outcomes, and evidence limits. A single citation can and often should appear across multiple wiki fields with different writing roles.
- For systematic reviews, scoping reviews, meta-analyses, and evidence syntheses, do not stop at generic findings. Capture review question/inclusion logic, included population and condition scope, technology/intervention taxonomy, outcome taxonomy, evidence quality and heterogeneity, equity/HCD/accessibility details, review-level takeaway, and what the review does not answer.
- For single empirical studies, preserve a compact full-study picture: problem or gap, population/condition/setting, intervention or phenomenon, key innovation, methods/sample/measures, main results, primary takeaway, evidence limits, and direct wiki mappings.

Seventh integrated source:

- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: PLOS ONE qualitative study of 10 family caregivers of people with spinal cord injury at Komfo Anokye Teaching Hospital in Ghana.

Source-backed SCI caregiver notes:

- SCI caregivers in this Ghanaian hospital context often entered caregiving suddenly and felt unprepared.
- Caregiver roles included hands-on inpatient care, ADL/IADL support, bowel/bladder-related support, transport, financial management, and household or business task substitution.
- Reported burdens included body pain, sleeplessness, tiredness, physical weakness, sickness, reduced ability to work, and financial strain.
- Coping included acceptance, personal care, hope, religious practices, social support, family financial help, childcare or business help, and encouragement.
- Use this source as condition-specific qualitative evidence and design rationale for SCI caregiver onboarding, assessment, training, counselling/social support, financial/resource navigation, and low-burden self-care support. Do not use it as prevalence or intervention-effectiveness evidence.
- Use Smith 2016 separately for SCI care-service structure, care hours, formal/informal care mix, and caregiver/attendant training gaps; pair it with Mohammed 2023 or other burden/lived-experience sources when making caregiver distress claims.

Eighth integrated source:

- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: Clinical Journal of Oncology Nursing pilot study of 50 primary caregivers of patients with end-stage ovarian cancer at an urban comprehensive cancer center.

Source-backed gynecological cancer caregiver notes:

- End-stage ovarian cancer caregivers in this sample reported disrupted schedules and financial problems as the most burdensome CRA domains.
- Caregiver self-esteem/positive meaning was also high and did not eliminate practical burden.
- Lower income and lower education were associated with greater financial burden in this sample; schedule disruption varied by income and employment status.
- Nursing support recommendations include caregiver preparation, symptom-management education, social work and interdisciplinary referrals, financial and medication assistance, support groups, and respite.
- Use this source as end-stage ovarian cancer caregiver burden evidence and design rationale for schedule support, financial/resource navigation, symptom-management education, self-care support, respite prompts, and referral pathways. Do not generalize to all gynecological cancers, earlier-stage ovarian cancer, or intervention effectiveness.

Ninth integrated source:

- `2001_glasgow_re-aim-framework-chronic-illness-management`: Patient Education and Counseling article applying the RE-AIM framework to chronic illness management intervention modalities.

Source-backed implementation and evaluation notes:

- RE-AIM evaluates Reach, Efficacy, Adoption, Implementation, and Maintenance.
- Reach includes participation rate and representativeness of participants versus non-participants.
- Adoption and implementation operate at the organization or setting level and are central to real-world intervention impact.
- Maintenance applies at both the individual level and organization level.
- Use this source as a methods and implementation-science anchor for digital health, smart-home, caregiver-support, and chronic illness management intervention evaluation.
- Do not treat this source as caregiver-specific evidence, condition-specific evidence, or proof that a particular AI, mHealth, or smart-home intervention is effective.

Tenth integrated batch:

- `2015_aneshensel-avison_stress-process-appreciation-pearlin`: Society and Mental Health article serving as a readable modern overview of Leonard I. Pearlin's stress-process legacy.
- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`: Journal of Social Work Education article on physical and mental health effects of family caregiving.

Source-backed stress-process and caregiver health notes:

- Source 01 should be used as a readable gateway into Pearlin's original stress-process architecture, not as a substitute citation for the original 1981 stress-process article or 1990 caregiving-specific stress-process paper.
- Pearlin-style stress-process architecture supports separating primary stressors, secondary role strains, secondary intrapsychic strains, stressor meaning/appraisal, coping, social support, mastery/self-concept, and outcomes.
- Schulz and Sherwood 2008 supports caregiving as chronic stress exposure involving sustained strain, unpredictability, uncontrollability, secondary stress, and vigilance.
- Caregiver health outcomes should include psychological health, physical health, health behaviors, self-care, positive caregiving meanings, and mortality-related outcomes when appropriate.
- Dementia caregiving burden claims from Schulz and Sherwood 2008 are caregiver-context evidence, not dementia treatment evidence and not evidence that dementia is normal aging.

Eleventh integrated batch:

- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`: International Journal of Telemedicine and Applications systematic review of 57 randomized controlled trial articles on telehealth interventions for family caregivers of people with chronic health conditions.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: DIGITAL HEALTH updated systematic review of 40 modern digital health intervention studies for family caregivers, including HCD method assessment.

Source-backed digital caregiver intervention notes:

- Graven 2021 supports telehealth caregiver intervention delivery across telephone, web, and combined modalities; telephone was the dominant RCT delivery mode, skills training was the most common intervention strategy, and psychological functioning was the most frequent improvement domain.
- Graven 2021 should not be treated as AI-agent, smart-home, or care-recipient clinical effectiveness evidence.
- Zhai 2023 supports digital health caregiver intervention design and outcome rationale, including psychological health, self-efficacy, caregiving skills, quality of life, social support, and coping.
- Zhai 2023 maps modern caregiver digital health technologies into web resources, telemedicine, and mHealth; intervention purposes include education, real-time communication, data collection/monitoring, psychotherapy, and connection/support.
- Zhai 2023 adds HCD, usability, accessibility, cultural/linguistic tailoring, marginalized caregiver inclusion, and digital health literacy as recurring design and evaluation concerns.
- Usability, satisfaction, feasibility, and acceptability remain separate from caregiver outcome effectiveness.
- Technology-access assumptions in older telehealth and digital health literature need current evidence before making present-day access claims.

Twelfth integrated batch:

- `2017_nichols_reach-dementia-caregiver-healthcare-costs`: Journal of the American Geriatrics Society article examining REACH II and REACH VA dementia caregiver intervention healthcare costs.
- `2010_gitlin_cope-dementia-home-based-intervention`: JAMA randomized trial of the COPE home-based biobehavioral environmental intervention for community-living dementia dyads.
- `2003_hepburn_savvy-caregiver-transportable-program`: The Gerontologist field-test article on translating the Savvy Caregiver Program into a transportable manualized dementia caregiver training program.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`: The Gerontologist randomized trial of online synchronous/asynchronous Tele-Savvy psychoeducation for dementia family caregivers.
- `2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis`: The Gerontologist updated comprehensive meta-analysis of dementia caregiver intervention effects.

Source-backed dementia caregiver intervention notes:

- REACH II/REACH VA add healthcare cost and integrated-system adoption evidence; use them for economic/implementation evaluation, not dementia treatment evidence.
- COPE supports short-term dyadic outcome evidence for home-based caregiver training, environmental/task tailoring, medical review, activity engagement, caregiver well-being, and caregiver confidence. It did not show sustained standardized effects at 9 months.
- Savvy Caregiver supports role-training, manualized curriculum, facilitator preparation, fidelity, and transportability, but the 2003 field-test article is not RCT-level effectiveness evidence.
- Tele-Savvy supports online synchronous/asynchronous dementia caregiver psychoeducation effects on depression, perceived stress, caregiver reaction to care-recipient behaviors, and mastery, while burden and anxiety effects were not found.
- Walter and Pinquart 2020 supports a dementia caregiver intervention taxonomy and outcome taxonomy. Average effects are generally small-to-moderate, active caregiver participation matters, and heterogeneity/publication-bias cautions should travel with claims.

Boundary note:

- These sources strengthen the dementia caregiver intervention, implementation, delivery, and evaluation layer. They should not be treated as AI-agent evidence, smart-home effectiveness evidence, normal-aging evidence, or direct dementia clinical treatment evidence.

Current dementia caregiver branch notes:

- `2020_cheng_meta-review-dementia-caregiver-interventions`: BMC Geriatrics comprehensive meta-review of systematic reviews and meta-analyses on nonpharmacological interventions for informal dementia caregivers.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Health and Social Care in the Community mixed-method systematic review of needs among family caregivers of people with dementia living at home.
- `2021_ruggiano_chatbots-dementia-caregivers`: Journal of Medical Internet Research systematic review of commercially available chatbot functions and quality for people with dementia and caregivers.

Source-backed dementia caregiver notes:

- Cheng 2020 closes the current dementia caregiver intervention synthesis anchor for section 3. It supports outcome-matched intervention logic, with depression more consistently modifiable than burden, anxiety, or social support, and cautions against assuming dyadic, multicomponent, respite, support-group, or technology-delivered approaches are inherently superior.
- Bressan 2020 closes the dementia caregiver needs anchor for section 3. It organizes home-care dementia caregiver needs around being supported, receiving accessible and personalized information, being trained and educated to manage changes, and finding balance.
- Ruggiano 2021 closes the dementia chatbot anchor for section 3. It supports cautious chatbot function/quality, privacy, safety, evidence-provenance, accessibility, escalation, and end-user-evaluation requirements, but not chatbot effectiveness, caregiver burden reduction, clinical safety, RAG/LLM effectiveness, or current app-market claims.
- These sources complete the narrowed dementia/ADRD caregiver Tier 1 branch in the updated core reference plan. AHRQ 2020 remains a future potential reference only and is skipped for now because it is over 500 pages.

Current SCI caregiver integrated sources:

- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: Behaviour Research and Therapy randomized trial of individualized problem-solving training delivered by monthly videoconferencing for SCI caregivers.
- `2009_elliott_brief-problem-solving-training-sci-caregivers`: Journal of Clinical Psychology randomized trial of brief problem-solving training plus education for recent-onset SCI caregivers.
- `2016_smith_caregiving-services-sci-systematic-review`: Spinal Cord systematic review of caregiving services in SCI.
- `2019_conti_secondary-conditions-caregiver-burden-sci`: Topics in Spinal Cord Injury Rehabilitation cross-sectional dyad study on care-recipient secondary conditions and SCI caregiver burden dimensions.
- `2022_espino_coping-social-support-caregiver-wellbeing-sci`: Topics in Spinal Cord Injury Rehabilitation mixed-methods study on coping, social support, unmet needs, and caregiver well-being in SCI dyads.

Source-backed SCI caregiver notes:

- Elliott 2008 supports remote/videoconference caregiver problem-solving support with caregiver depression and care-recipient social-functioning signals, but high attrition and unclear mechanisms limit broad effectiveness claims.
- Elliott and Berry 2009 supports brief PST plus education for dysfunctional problem-solving style in recent-onset SCI caregivers, not caregiver depression effectiveness.
- Smith 2016 supports SCI caregiving service structure, formal/informal care, care hours, functional predictors, caregiver/attendant training, and service-quality gaps. It excluded caregiver burden studies and should not be used as the primary caregiver burden synthesis.
- Conti 2019 supports SCI secondary-condition burden mechanisms, especially bladder dysfunction, UTIs, pressure injuries, chronic pain, functional independence, care hours, and caregiving duration. It is cross-sectional correlational evidence, not causal or intervention-effectiveness evidence.
- Espino 2022 supports SCI caregiver protective-factor and unmet-needs logic around coping/problem-solving orientation, social support, respite, system navigation, caregiver mental/physical health red flags, and shared future planning. Its caregiver profiles are exploratory, not validated triage categories.
- None of these SCI caregiver sources are AI-agent, smart-home, autonomous care, or SCI disease-background evidence. Source 22 remains the NINDS SCI website for disease-background checks only.

Current cancer caregiver integrated sources:

- `2019_ugalde_cancer-caregiver-interventions-implementation-potential`: Psycho-Oncology systematic review appraising cancer caregiver intervention studies for implementation potential using Proctor implementation outcomes. Use as broad cancer caregiver implementation-readiness evidence, especially for acceptability, adoption, appropriateness, feasibility, fidelity, cost, caregiver co-design gaps, high-need targeting, eligible-caregiver enrollment gaps, staff training, delivery-resource reporting, and translation-to-practice limits.
- Do not treat Ugalde 2019 as gynecological-cancer-specific effectiveness evidence, AI-agent evidence, smart-home evidence, mHealth effectiveness evidence, autonomous-care evidence, cancer-treatment evidence, or proof that acceptability or completion equals effectiveness. Its PDF extraction was usable for narrative sections, but long table details should be checked manually before exact included-study claims.
- `2023_becque_supportive-interventions-family-caregivers-advanced-cancer`: Psycho-Oncology systematic review of supportive interventions for family caregivers of patients with advanced cancer. Use as broad advanced cancer caregiver supportive-intervention taxonomy and outcome-domain mapping evidence, especially for individual, dyadic/family, and group support formats; caregiver self-care, patient-caregiving, and family-care components; and physical, psycho-emotional, social, spiritual, daily-functioning, and quality-of-life outcomes.
- Do not treat Becque 2023 as gynecological-cancer-specific effectiveness evidence, AI-agent evidence, smart-home evidence, mHealth effectiveness evidence, autonomous care evidence, or cancer-treatment evidence. Its PDF has a two-column layout; Ghostscript extraction was usable for narrative sections, but table-level details should be checked manually before exact table claims.
- `2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs`: JMIR Cancer focus group study with 41 gynecologic cancer patients and 22 caregivers/support persons. Use as direct gynecologic cancer formative mHealth design evidence for curated trustworthy information, symptom-urgency self-triage needs, trajectory-tailored recommendations, moderated peer/clinical expert support, patient and caregiver private spaces, granular sharing controls, and technology-access cautions.
- Do not treat Campbell 2024 as mHealth effectiveness evidence, AI-agent evidence, smart-home evidence, autonomous triage evidence, or cancer-treatment evidence. Its sample was mostly White and recruited through a trusted gynecologic oncology practice; COVID-19 timing and mixed patient-caregiver focus groups may have shaped responses.
- `2024_dave_cancer-caregiver-needs-patient-advocacy-groups`: Future Oncology narrative review on broad cancer caregiver unmet needs and patient advocacy group roles. Use as advocacy-ecosystem framing across informational, relationship/communication, emotional, and practical/financial needs; caregiver identity recognition; telehealth access cautions; and advocacy-group education, navigation, counseling, peer-support, financial-aid, and policy roles.
- Do not treat Dave 2024 as a systematic review, gynecological-cancer-specific evidence, intervention-effectiveness proof, AI evidence, smart-home evidence, mHealth effectiveness evidence, or cancer-treatment evidence. The article includes Pfizer and advocacy-organization authors and explicitly says the review is not comprehensive.

Standalone event-notes ingest:

- `2026-06-03_koroshetz_neuroscience-take-home-points-sci-translation`: University of Pittsburgh Rehabilitation Research Institute day event morning first lecture notes from Dr. Walter Koroshetz, Immediate past Director of NINDS and Senior Advisor at the Dana Foundation. The user specified that Gemini 3.5 Flash translated original slide points from `image.png` into spinal cord injury specific research, clinical trial, and engineering settings.

Source-backed SCI research framing notes:

- Treat these notes as presentation takeaway plus AI-assisted interpretation, not published evidence and not a verified transcript.
- Keep this record separate from the middle Mac setup talk and separate from the ongoing caregiver system ingest.
- The notes frame SCI research around rapid neuroscience progress with remaining spinal-circuitry gaps, neuroplasticity-focused combination therapies, bionic integration, spatial transcriptomics and single-cell omics, realistic public communication around stem-cell/regenerative timelines, hyper-acute secondary-injury urgency, better trial stratification, the brain-in-body problem, rodent-model translation limits, molecular/systems-neuroscience convergence, and sustained funding for long SCI trials.
- Use this source for SCI research framing, trial-design questions, neuroengineering ideation, and science-communication gaps. Do not use it as proof of clinical effectiveness or as caregiver evidence unless later event notes directly discuss caregivers.

Second standalone event-notes ingest:

- `2026-06-03_fridriksson_brain-health-aphasia-recovery`: University of Pittsburgh Rehabilitation Research Institute day event second lecture notes from Dr. Julius Fridriksson, Professor and Vice President for Research, Department of Communication Sciences and Disorders, Arnold School of Public Health, University of South Carolina.

Source-backed chronic-condition/disability neurorehabilitation framing notes:

- Aphasia is not a focused condition overlay in this wiki; treat it as chronic-condition/disability neurorehabilitation source context unless the user later asks for an aphasia condition page.
- The notes frame aphasia recovery as shaped by upstream drivers such as vascular strain, hypertension, diabetes, glycemic control, and hearing loss; brain-health axes such as Brain Age Gap and white matter hyperintensities; network mechanisms such as structural disconnection and controllability; and the stroke lesion pathway.
- Use this source for biomarker-stratified rehabilitation design, trial-stratification questions, longitudinal imaging/behavior mapping, and AI analytics boundaries. Do not use it as proof of causality, proof of intervention effectiveness, or evidence that brain age can currently be clinically reversed.

AI method integrated sources:

- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: NeurIPS 2020 technical paper introducing retrieval-augmented generation for knowledge-intensive NLP tasks.
- `2023_yao_react-reasoning-acting-language-models`: ICLR 2023 technical paper introducing ReAct, a reasoning-plus-action prompting paradigm for language models.

Source-backed AI method notes:

- RAG combines a parametric seq2seq generator with a non-parametric retrieval index and supports source-grounded generation, provenance inspection, and knowledge updates through the external index.
- ReAct interleaves reasoning traces and tool/environment actions, supporting stepwise task solving, external information gathering, and inspectable trajectories.
- Use both sources as technical architecture/design rationale for future AI-driven digital health, caregiver-support, pre-clinic preparation, information access, and bounded tool-use systems.
- Do not treat either source as healthcare, caregiving, condition-specific, clinical-safety, usability, equity, or intervention-effectiveness evidence.
- Health-related RAG/ReAct systems need curated source corpora, privacy controls, access control, audit logs, human confirmation, source review, clinical decision boundaries, and RE-AIM-style evaluation before real-world use.

Current CareBuddy integrated sources:

- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: Innovation in Aging conference abstract on CareBuddy as a modular multi-agent conversational AI for Alzheimer's care and assistance.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: JMIR Aging development and mixed-methods usability/acceptability study of CareBuddy as a mobile care ecosystem for dementia caregivers.

Source-backed CareBuddy notes:

- Hasan 2025 should be used as abstract-level evidence for multi-agent conversational AI with specialized agents for medical inquiries, appointment scheduling, meal planning, and reminders coordinated by a central orchestrator.
- Malhotra 2025 should be used as direct published evidence for dementia caregiver mHealth development, usability, acceptability, and design rationale, not effectiveness.
- Malhotra 2025 CareBuddy includes personalized assessments, tailored dementia symptom-management strategies, RAG-supported chatbot support, GPS monitoring for wandering, care plans, provider messaging, QR multi-caregiver coordination, telemedicine links, helpline access, financial/legal/future planning, self-care worksheets, calendar reminders, peer forum support, provider/moderator interfaces, usage logs, notifications, chat history management, and source-reported privacy/security controls.
- CareBuddy strengthens the wiki's dementia caregiver system-design layer across AI-driven digital health, smart-home/location monitoring, information access, care coordination, caregiver self-care, emotional/social support, safety monitoring, care-recipient privacy, modular caregiver mHealth, one-stop caregiver support, RAG health AI, clinician-portal support, reliability, and intervention evaluation.
- Do not treat either source as evidence of clinical effectiveness, care-recipient safety outcomes, long-term adoption, or caregiver burden reduction. The planned hybrid type 1 randomized trial in Malhotra 2025 is future work.
