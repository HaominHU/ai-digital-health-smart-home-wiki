---
title: Research Wiki Memory
type: memory
status: draft
privacy: private
last_updated: 2026-06-03
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

Current local abstracts and papers through source 42 have been previewed and integrated. A useful next step is a lint/source-status pass before adding new sources, especially to check citation export readiness, orphan pages, evidence limits, and whether ignored preview/source artifacts should be retained locally.

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

Part 2 integrated sources:

- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: Innovation in Aging conference abstract on CareBuddy as a modular multi-agent conversational AI for Alzheimer's care and assistance.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: JMIR Aging development and mixed-methods usability/acceptability study of CareBuddy as a mobile care ecosystem for dementia caregivers.

Source-backed CareBuddy notes:

- Hasan 2025 should be used as abstract-level evidence for multi-agent conversational AI with specialized agents for medical inquiries, appointment scheduling, meal planning, and reminders coordinated by a central orchestrator.
- Malhotra 2025 should be used as direct published evidence for dementia caregiver mHealth development, usability, acceptability, and design rationale, not effectiveness.
- Malhotra 2025 CareBuddy includes personalized assessments, tailored dementia symptom-management strategies, RAG-supported chatbot support, GPS monitoring for wandering, care plans, provider messaging, QR multi-caregiver coordination, telemedicine links, helpline access, financial/legal/future planning, self-care worksheets, calendar reminders, peer forum support, provider/moderator interfaces, usage logs, notifications, chat history management, and source-reported privacy/security controls.
- CareBuddy strengthens the wiki's dementia caregiver system-design layer across AI-driven digital health, smart-home/location monitoring, information access, care coordination, caregiver self-care, emotional/social support, safety monitoring, care-recipient privacy, modular caregiver mHealth, one-stop caregiver support, RAG health AI, clinician-portal support, reliability, and intervention evaluation.
- Do not treat either source as evidence of clinical effectiveness, care-recipient safety outcomes, long-term adoption, or caregiver burden reduction. The planned hybrid type 1 randomized trial in Malhotra 2025 is future work.
