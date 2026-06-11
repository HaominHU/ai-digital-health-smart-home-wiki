---
title: Adaptive Modular Caregiver mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [mhealth, adaptive-design, modular-design, family-caregivers, design-pattern]
last_updated: 2026-06-11
---

# Adaptive Modular Caregiver mHealth

## Pattern Summary

Build caregiver mHealth systems as modular app suites that combine general caregiver support, reusable condition-specific interfaces, and condition-unique content or modules.

## Source-Backed Rationale

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: The dissertation describes an adaptive modular infrastructure with general modules for all family caregivers, general modules with condition-specific content, data interfaces, and condition-specific modules.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: The iMHere 2.0 paper grounds the system infrastructure behind this research line, including adaptive modules, caregiver app, clinician portal, secure synchronization, and scalable architecture that can support future expansion.
- `2015_aneshensel-avison_stress-process-appreciation-pearlin`: Pearlin-style stress-process architecture supports tailoring modules by stressor type, secondary strains, coping resources, social support, mastery, and outcome risk.
- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`: Modular caregiver systems should account for care intensity, vigilance, caregiver physical and psychological health, health behaviors, and positive caregiving meaning.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`: Telehealth caregiver interventions commonly combine skills training, psychoeducation/resources, self-monitoring/tracking, reminders, counseling, and support applications across telephone, web, and combined modalities.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: Modern digital health caregiver interventions should use HCD, accessibility, usability, cultural/linguistic tailoring, and theory-informed intervention components.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver supports are more plausible when they address both practical care demands and emotional toll and are tailored to caregiver risk, disease/treatment trajectory, and care context.
- `2016_nasem_families-caring-for-an-aging-america`: Caregiver support should start from assessment of caregiver risks, needs, strengths, preferences, capacity, and willingness.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Modules should be classifiable by whether they target clinical knowledge, psychological skills, support seeking, quantity/quality of care, caregiver outcomes, or care-recipient outcomes.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregiver modules should consider onboarding for sudden caregiving entry, ADL/IADL support, physical burden, financial/resource navigation, social support, coping, and training/counselling referral.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: SCI caregiver modules can include remotely delivered, problem-tailored coaching, but should track attrition, fidelity, and dyadic outcomes.
- `2009_elliott_brief-problem-solving-training-sci-caregivers`: SCI caregiver modules can include brief PST, education, caregiver-requested boosters, and first-year transition support while separating problem-solving style from depression outcomes.
- `2016_smith_caregiving-services-sci-systematic-review`: SCI caregiver modules can include care-hour tracking, caregiver/attendant training, secondary-condition knowledge, formal/informal care mix, backup-care planning, and long-term changing needs.
- `2019_conti_secondary-conditions-caregiver-burden-sci`: SCI caregiver modules can include secondary-condition monitoring prompts, bladder/UTI and pressure-injury routine support, functional-independence context, and burden-dimension tracking, while recognizing the source is correlational.
- `2022_espino_coping-social-support-caregiver-wellbeing-sci`: SCI caregiver modules can include problem-solving skill support, social-support routing, respite/resource navigation, caregiver health red-flag screening, and shared future-care planning.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: Advanced ovarian cancer caregiver modules should consider schedule disruption, financial/resource navigation, symptom-management education, respite prompts, self-care support, and interdisciplinary referral pathways.
- `2019_ugalde_cancer-caregiver-interventions-implementation-potential`: Cancer caregiver modules should include implementation-readiness checks for caregiver co-design, acceptability, high-need targeting, adoption partner, fidelity, staff time, training, resources, and cost. Use as implementation evidence, not mHealth effectiveness evidence.
- `2023_becque_supportive-interventions-family-caregivers-advanced-cancer`: Advanced cancer caregiver modules can be organized around caregiver self-care, patient-caregiving support, and family-care support, with format choices for individual, dyadic/family, or peer/group support. Use as intervention-taxonomy evidence, not mHealth effectiveness evidence.
- `2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs`: Gynecologic cancer mHealth modules can include curated information, symptom-urgency guidance, trajectory-tailored recommendations, moderated expert/peer support, private spaces, and granular information-sharing controls. Use as formative design evidence, not effectiveness evidence.
- `2024_dave_cancer-caregiver-needs-patient-advocacy-groups`: Broad cancer caregiver modules can include advocacy-resource navigation, financial/legal/employment support, counseling and peer-support links, and plain-language education. Use as ecosystem framing, not app effectiveness evidence.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: Modular systems should be evaluated for reach, efficacy, adoption, implementation, and maintenance, not only module usability or participant satisfaction.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy provides a dementia-specific example of a modular mobile care ecosystem with assessment, tailored symptom support, RAG chatbot, GPS monitoring, care planning, telemedicine links, helpline, self-care, reminders, and peer support.
- `2010_gitlin_cope-dementia-home-based-intervention`: COPE supports modular dementia caregiver intervention logic around assessment, environmental/task tailoring, caregiver training, medical review, activity engagement, and stress reduction.
- `2003_hepburn_savvy-caregiver-transportable-program`: Savvy Caregiver supports manualized curriculum modules, facilitator preparation, homework, and fidelity-preserving transportability.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`: Tele-Savvy supports synchronous/asynchronous digital delivery of caregiver role training and mastery-building modules.
- `2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis`: Modular caregiver systems should prioritize active training when outcomes beyond knowledge are desired and should match components to target outcomes.
- `2026_kingsada_preferences-digital-health-technologies`: Patient preference evidence supports modular digital health design that can expose choices around cost, privacy, personalization, clinician connection, self-management, and hybrid support. Use this as indirect preference-sensitive design rationale, not caregiver-specific evidence.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Spinal cord injury.
- Gynecological cancer.

## Technology Components

- Configurable modules.
- General caregiver self-care tools.
- Condition-specific educational content.
- Resource libraries.
- Risk assessment.
- Goals and plans.
- Caregiver assessment and triage.
- Stress-process-tailored support pathways.
- Caregiver health behavior and self-care modules.
- Telehealth and digital health delivery modes.
- HCD-informed accessibility and usability modules.
- Evaluation instrumentation for activities, outcomes, utilization, and cost.
- SCI-specific caregiver onboarding and task training.
- SCI-specific problem-solving coaching, brief booster support, and discharge-to-community transition modules.
- SCI-specific caregiving service modules for care hours, care quality, secondary-condition knowledge, attendant training, and formal/informal care coordination.
- SCI-specific secondary-condition and burden modules for bladder/UTI routines, pressure-injury vigilance, chronic pain context, functional independence, and burden dimensions.
- SCI-specific caregiver well-being modules for coping orientation, social support, respite, system navigation, red flags, and future planning.
- Financial strain and social support navigation.
- Advanced cancer symptom-management education and referral pathways.
- Cancer caregiver implementation-readiness checks for adoption partner, staff role, training burden, fidelity, caregiver time, resource requirements, and cost.
- Advanced cancer caregiver support modules for psycho-emotional, daily-functioning, social/family, spiritual, physical, and quality-of-life targets.
- Gynecologic cancer dyadic modules for self-triage guidance, curated expert information, private caregiver/patient spaces, and controlled family sharing.
- Advocacy-resource navigation modules for financial assistance, legal/employment rights, counseling, peer support, genetic-risk resources, and cancer-specific nonprofit support.
- Reach, adoption, implementation, and maintenance instrumentation.
- Dementia-specific modules for behavioral/physical symptoms, wandering, caregiver self-care, peer support, and future planning.
- Active caregiver training modules for dementia-related behavior response, activity engagement, mastery, and environmental/task adaptation.
- Synchronous/asynchronous learning pathways with explicit scheduling, connectivity, and technology-access constraints.
- Preference-elicitation and configuration checks that separately capture caregiver preferences, care-recipient preferences, and shared-access privacy trade-offs.

## Design Constraints

- Keep reusable caregiver challenges separate from condition overlays.
- Do not turn participant-composition conditions into new wiki condition taxonomies unless explicitly prioritized.
- Treat future AI and wearable augmentation as an extension layer unless implemented and evaluated.
- Track whether modular personalization improves reach and sustained use or only adds configuration burden.
- Do not import patient DHT preferences directly as caregiver preferences; elicit caregiver and care-recipient preferences separately when modules affect both.

## Evidence

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`.
- `2015_aneshensel-avison_stress-process-appreciation-pearlin`.
- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`.
- `2023_zhai_digital-health-interventions-support-family-caregivers`.
- `2020_schulz_family-caregiving-for-older-adults`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`.
- `2001_glasgow_re-aim-framework-chronic-illness-management`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.
- `2010_gitlin_cope-dementia-home-based-intervention`.
- `2003_hepburn_savvy-caregiver-transportable-program`.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`.
- `2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis`.
- `2026_kingsada_preferences-digital-health-technologies`.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`.
- `2009_elliott_brief-problem-solving-training-sci-caregivers`.
- `2016_smith_caregiving-services-sci-systematic-review`.
- `2019_conti_secondary-conditions-caregiver-burden-sci`.
- `2022_espino_coping-social-support-caregiver-wellbeing-sci`.
- `2019_ugalde_cancer-caregiver-interventions-implementation-potential`.
- `2023_becque_supportive-interventions-family-caregivers-advanced-cancer`.
- `2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs`.
- `2024_dave_cancer-caregiver-needs-patient-advocacy-groups`.

## Gaps

- Needs broader testing across caregiver populations and conditions.
- Needs outcome evidence beyond usability, acceptability, and feasibility.
- Needs evaluation designs that distinguish module targets, caregiver outcomes, care-recipient outcomes, utilization, and cost.
- Needs RE-AIM-style evaluation of representativeness, organizational adoption, fidelity, and sustained use.
- Needs SCI-specific testing of whether secondary-condition, respite, coping, and social-support modules improve meaningful outcomes beyond perceived relevance or usability.
- Needs cancer caregiver digital adaptations that evaluate implementation readiness, not only usability or caregiver satisfaction.
- Needs advanced-cancer-specific testing of whether modular digital delivery preserves the benefits of supportive interventions without increasing caregiver workload or losing face-to-face relational support.
- Needs gynecologic cancer mHealth testing with more diverse, rural, lower-resource, and lower-digital-literacy samples.
- Needs evaluation of whether advocacy-resource navigation produces completed referrals, reduced burden, financial relief, or better caregiver outcomes.

## Related Pages

- `wiki/design_patterns/one_stop_caregiver_support_app.md`
- `wiki/populations/family_caregivers.md`
