---
title: AI-Driven Digital Health
type: technology
status: draft
privacy: private
evidence_status: has_sources
tags: [ai, digital-health, technology-lens]
last_updated: 2026-07-02
---

# AI-Driven Digital Health

## Scope

Primary technology focus for the wiki.

## Intended Support Role

AI-driven digital health should be analyzed as research, design, and knowledge support unless a source or user request explicitly defines another scope.

## Non-Use Boundary

Do not frame wiki outputs as autonomous diagnosis, treatment recommendation, or clinical decision-making.

## Privacy, Security, and Safety Concerns

Track data minimization, consent, access control, auditability, bias, human oversight, and escalation boundaries.

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: The source explicitly raises that care recipients may be reluctant to link sensitive EHR or wearable data to a commercial AI platform. Record-connected AI support should therefore be treated as a separate privacy, consent, trust, and security question.

## Design Implications

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Generative AI for caregiver mHealth may be most appropriate as an adaptive support layer rather than a standalone chatbot.
- The source identifies three possible AI layers for family caregiver apps: agentic interaction for proactive engagement, adaptive content for personalized education, and emotional/social support for check-ins, peer connection, and resource navigation.
- Named implementation directions include context-sensitive prompts, retrieval-augmented generation, large language models, multimodal AI, peer matching, and dynamic resource directories.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: In an exploratory SCI pre-clinic preparation evaluation, a source-reported health-focused ChatGPT interface provided more structured support for caregiver tools, portal message drafts, and multi-deliverable outputs than standard ChatGPT, while care-recipient-style prompts scored higher on empathetic tone than concise clinical prompts.
- Prompt format should be treated as a design variable that can affect perceived empathy, usability, and actionability.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Future-work directions include GenAI agents for customized suggestions, prompts, automations, RAG-supported chatbot support, and adaptive reminders. These should be treated as design directions from dissertation synthesis, not implemented effectiveness evidence.
- `2016_nasem_families-caring-for-an-aging-america`: The report identifies telehealth, remote monitoring, sensing, assistive technologies, and linked care coordination tools as innovation targets for caregiver support. Treat these as policy/design rationale, not direct AI effectiveness evidence.
- `2020_schulz_family-caregiving-for-older-adults`: Technology-based caregiver interventions can deliver knowledge, social support, therapeutic strategies, monitoring, training, and performance support, but sustained use, accessibility, cost-effectiveness, system design, and care integration remain unresolved.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: AI or digital health interventions should make explicit whether they target caregiving activities, caregiver outcomes, care-recipient outcomes, utilization, or economic outcomes.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: AI and digital health interventions should be evaluated for reach, efficacy/effectiveness, adoption, implementation, and maintenance rather than technical performance or efficacy alone.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`: Telehealth RCT evidence supports remote caregiver intervention delivery through telephone, web, and combined modalities, but should not be treated as AI-specific evidence.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: Digital health caregiver interventions can support psychological health, self-efficacy, caregiving skills, quality of life, social support, and coping; HCD, accessibility, and cultural/linguistic tailoring remain major design needs.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: Retrieval-augmented generation is a technical method for grounding generated outputs in retrieved source passages and updating knowledge through an external index.
- `2023_yao_react-reasoning-acting-language-models`: ReAct is a technical method for interleaving reasoning traces and tool/environment actions, relevant to bounded AI agents but not evidence of healthcare safety or effectiveness.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes a source-reported GPT-4/GPT-3.5 RAG chatbot with confidence-based retrieval, internal Q&A content, external sources, urgent/sensitive-case helpline routing, and privacy/security controls.
- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: A CareBuddy abstract describes a multi-agent conversational AI architecture with specialized agents and central orchestration for Alzheimer's care and assistance.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`: Tele-Savvy supports online synchronous/asynchronous caregiver psychoeducation as broad digital health intervention evidence, but it is not AI-agent evidence.
- `2017_nichols_reach-dementia-caregiver-healthcare-costs`, `2010_gitlin_cope-dementia-home-based-intervention`, `2003_hepburn_savvy-caregiver-transportable-program`, and `2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis`: These are useful caregiver intervention and evaluation anchors for future digital systems, not direct AI or smart-home effectiveness evidence.
- `2020_cheng_meta-review-dementia-caregiver-interventions`: Use this as outcome-matching logic for future AI-enabled dementia caregiver interventions; it is not AI or chatbot evidence.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Use this as a dementia caregiver needs taxonomy for adaptive content, triage, and service-navigation design; it is not digital intervention effectiveness evidence.
- `2021_ruggiano_chatbots-dementia-caregivers`: Use this as direct dementia chatbot design and evaluation evidence. It supports privacy, safety, evidence-provenance, accessibility, and end-user evaluation requirements, but not chatbot effectiveness or current-market claims.
- `2026-06-03_fridriksson_brain-health-aphasia-recovery`: Neurorehabilitation analytics should treat brain-health markers, systemic-health measures, sensory status, network metrics, lesion characteristics, and longitudinal outcomes as distinct data layers. AI support may help stratify trials or map trajectories, but prediction, causal inference, and clinical decision-making must remain separate.
- `2026_kingsada_preferences-digital-health-technologies`: Patient-facing digital health design should account for patient preferences around cost, privacy, convenience, ease of use, data security, personalization, clinician connection, and hybrid digital/in-person support. This is adoption and preference evidence, not AI safety or effectiveness evidence.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: Use as telehealth delivery evidence for remote SCI caregiver coaching, not as AI-agent or smart-home evidence.
- `2026-06-16_chen_generative-ai-meaning-centered-care-later-life`: Use as conceptual rationale for GenAI as bounded, human-supervised interactional infrastructure for meaning-centered care in later life. It supports design attention to dignity, life review, narrative fidelity, user-controlled sharing, escalation, and governance, not effectiveness claims.
- `2026-06-16_mahmood_telehealth-informal-caregivers`: Use as caregiver telehealth utilization evidence and caregiver-inclusive digital health access rationale, not as AI-specific evidence.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: AMIA abstract deriving future generative AI design recommendations from iterative human-centered design and evaluation of the iMHere Family Caregiver App. Generative AI was proposed, not implemented or evaluated in the current app.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AMIA abstract comparing source-reported ChatGPT and ChatGPT Health interfaces for SCI pre-clinic preparation without connected health records. Product/model details are source-reported and may change over time.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Dissertation evidence supports AI/GenAI as future work for caregiver mHealth, especially intelligent reminders and personalized support. It does not evaluate deployed GenAI features.
- `2016_nasem_families-caring-for-an-aging-america`: Formal report supporting technology innovation for caregiver support and care coordination in older-adult care.
- `2020_schulz_family-caregiving-for-older-adults`: Review evidence supporting technology-based caregiver intervention rationale and cautions.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Evaluation framework for caregiver intervention targets and outcomes.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: RE-AIM evaluation framework for chronic illness intervention impact, implementation, and maintenance.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`: Telehealth caregiver intervention systematic review; use for digital delivery and outcome-domain rationale, not AI effectiveness.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: Digital health caregiver intervention systematic review; use for HCD/usability/accessibility and caregiver outcome rationale, not autonomous AI evidence.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: Technical RAG method source; use for architecture rationale only.
- `2023_yao_react-reasoning-acting-language-models`: Technical ReAct method source; use for bounded tool-use and oversight rationale only.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: Published usability/acceptability evidence for AI-supported dementia caregiver mHealth; not effectiveness evidence.
- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: Conference abstract evidence for multi-agent conversational AI in Alzheimer's care; abstract-level only.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`: Online dementia caregiver psychoeducation RCT; use as digital delivery evidence, not AI evidence.
- `2020_cheng_meta-review-dementia-caregiver-interventions`: Meta-review evidence for dementia caregiver intervention outcome matching; use as a future AI-system evaluation anchor, not AI evidence.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Mixed-method review evidence for dementia caregiver needs; use for adaptive content and triage design rationale, not effectiveness evidence.
- `2021_ruggiano_chatbots-dementia-caregivers`: Systematic review of commercially available dementia chatbots; use for chatbot function/quality and evidence-gap framing, not clinical or caregiver outcome effectiveness.
- `2026-06-03_fridriksson_brain-health-aphasia-recovery`: Lecture-note evidence for biomarker-aware neurorehabilitation framing; use for design and trial-stratification rationale, not AI effectiveness or clinical decision support evidence.
- `2026_kingsada_preferences-digital-health-technologies`: Scoping-review evidence on patient preferences for eHealth, telehealth, telemedicine, and mHealth; use for preference-sensitive adoption and HTA rationale, not clinical effectiveness or caregiver outcome evidence.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: SCI caregiver videoconferencing RCT; use as remote delivery and evaluation-boundary evidence, not AI evidence.
- `2026-06-16_chen_generative-ai-meaning-centered-care-later-life`: Perspective article proposing a Sensing-Narrating-Connecting-Governing framework for GenAI-supported meaning-centered care in later life; use as conceptual AI interaction and governance evidence.
- `2026-06-16_mahmood_telehealth-informal-caregivers`: HINTS6 telehealth utilization study among U.S. adults aged 50+; use for caregiver digital health access and multi-participant telehealth rationale, not AI effectiveness.
