---
title: Research Wiki Memory
type: memory
status: draft
privacy: private
last_updated: 2026-05-27
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
- Generated previews, briefs, prompts, and reports live under `outputs/`.
- Sensitive scratch notes live under `private_notes/`.
- Citation-memory records live under `wiki/references/items/`.
- Zotero/EndNote-compatible citation exports live under `outputs/citation_exports/`.
- `AGENTS.md` governs agent behavior.
- `INDEX.md` is the content-oriented map.
- `LOG.md` is the chronological timeline.
- `MEMORY.md` is the compressed current-state digest.

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

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The tracked wiki should preserve source-derived knowledge through source IDs, source context, evidence labels, and durable Markdown synthesis.

Recommended raw source ID and filename pattern:

`YYYY-MM-DD_author-or-org_short-title.ext`

Periodic lint checks should flag locally stored raw sources that may be removable after their contents have been well digested into the wiki. Do not delete raw sources automatically.

## Citation Management Baseline

Citation-bearing sources should have Markdown citation-memory records under `wiki/references/items/`.

Citation records should preserve original citation text, source IDs, evidence type, topic links, supported claims, writing roles, and export-readiness status. RIS is the default generated export format because it is compatible with Zotero and EndNote.

Use citation-supported brainstorming when the user is developing a manuscript idea and wants citations for introduction, background, significance, or related writing sections. Default to wiki-first mode: use stored wiki citations first and assess coverage quality rather than relying on a citation-count threshold.

When wiki coverage is weak, narrow, missing foundational sources, missing recent state-of-the-art sources, or missing population/condition/technology anchors, external seed search can supplement bibliography-building. Keep searched citations separate from wiki citations, label them as external candidates until reviewed or ingested, and create separate RIS exports for wiki citations and external candidates when files are requested.

## Next Useful Step

Continue one-by-one source ingest from `sources/abstracts/` and `sources/papers/`.

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

Seventh integrated source:

- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: PLOS ONE qualitative study of 10 family caregivers of people with spinal cord injury at Komfo Anokye Teaching Hospital in Ghana.

Source-backed SCI caregiver notes:

- SCI caregivers in this Ghanaian hospital context often entered caregiving suddenly and felt unprepared.
- Caregiver roles included hands-on inpatient care, ADL/IADL support, bowel/bladder-related support, transport, financial management, and household or business task substitution.
- Reported burdens included body pain, sleeplessness, tiredness, physical weakness, sickness, reduced ability to work, and financial strain.
- Coping included acceptance, personal care, hope, religious practices, social support, family financial help, childcare or business help, and encouragement.
- Use this source as condition-specific qualitative evidence and design rationale for SCI caregiver onboarding, assessment, training, counselling/social support, financial/resource navigation, and low-burden self-care support. Do not use it as prevalence or intervention-effectiveness evidence.

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
- Technology-access assumptions in the paper reflect the 2000-era context and need current evidence before making present-day access claims.

Tenth and eleventh integrated sources:

- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: NeurIPS 2020 technical paper introducing retrieval-augmented generation for knowledge-intensive NLP tasks.
- `2023_yao_react-reasoning-acting-language-models`: ICLR 2023 technical paper introducing ReAct, a reasoning-plus-action prompting paradigm for language models.

Source-backed AI method notes:

- RAG combines a parametric seq2seq generator with a non-parametric retrieval index and supports source-grounded generation, provenance inspection, and knowledge updates through the external index.
- ReAct interleaves reasoning traces and tool/environment actions, supporting stepwise task solving, external information gathering, and inspectable trajectories.
- Use both sources as technical architecture/design rationale for future AI-driven digital health, caregiver-support, pre-clinic preparation, information access, and bounded tool-use systems.
- Do not treat either source as healthcare, caregiving, condition-specific, clinical-safety, usability, equity, or intervention-effectiveness evidence.
- Health-related RAG/ReAct systems need curated source corpora, privacy controls, access control, audit logs, human confirmation, source review, clinical decision boundaries, and RE-AIM-style evaluation before real-world use.
