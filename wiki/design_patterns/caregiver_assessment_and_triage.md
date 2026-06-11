---
title: Caregiver Assessment and Triage
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [caregiver-assessment, triage, care-coordination, design-pattern]
last_updated: 2026-06-11
---

# Caregiver Assessment and Triage

## Pattern Summary

Identify caregivers, assess their risks, needs, strengths, preferences, capacity, and willingness, then route them to appropriate training, support, referrals, or escalation pathways.

## Source-Backed Rationale

- `2015_aneshensel-avison_stress-process-appreciation-pearlin`: Caregiver assessment can use Pearlin-style stress-process domains: primary stressors, secondary strains, stressor meaning, coping, social support, mastery, and outcomes.
- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`: Assessment should include care-recipient impairment and behavior, care intensity, vigilance, caregiver health, health behaviors, socioeconomic vulnerability, social support, and positive caregiving meanings.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: Digital caregiver support should include caregiver psychosocial assessment and capacity assessment across physical condition, mental concerns, and self-efficacy.
- `2016_nasem_families-caring-for-an-aging-america`: The National Academies report recommends routine caregiver identification and assessment in health care and LTSS, including caregiver health, stress, skills, employment, willingness, and support needs.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver risk varies by intensity, duration, care recipient suffering, behavioral symptoms, caregiver health, support availability, perceived choice, and home environment.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregiver assessment should include preparedness, physical burden, sleep disruption, financial strain, social support, coping strategies, and need for training or counselling.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: SCI caregiver assessment can use personally salient problem identification and should include retention risk, technology access, caregiver depression, and possible care-recipient social-functioning effects.
- `2009_elliott_brief-problem-solving-training-sci-caregivers`: Recent-onset SCI caregiver triage can include card-sort problem identification, dysfunctional problem-solving style, education needs, and readiness for brief follow-up contacts.
- `2016_smith_caregiving-services-sci-systematic-review`: SCI caregiver/service assessment should include care hours, formal/informal care mix, caregiver backup availability, training history, functional independence, IADL capacity, and secondary-condition knowledge needs.
- `2019_conti_secondary-conditions-caregiver-burden-sci`: SCI caregiver assessment should include care-recipient secondary physical conditions, functional independence, bladder dysfunction, UTIs, pressure injuries, chronic pain, caregiving hours, years of caregiving, and multidimensional caregiver burden.
- `2022_espino_coping-social-support-caregiver-wellbeing-sci`: SCI caregiver triage can assess coping and problem-solving orientation, social support satisfaction, respite gaps, system-navigation needs, caregiver health red flags, isolation, unmet needs, and shared future care planning.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: Advanced ovarian cancer caregiver assessment can use CRA-informed domains such as disrupted schedules, financial problems, lack of family support, health problems, and caregiver self-esteem.
- `2010_gitlin_cope-dementia-home-based-intervention`: Dementia caregiver assessment can include caregiver-identified concerns, patient capabilities, home environment, communication, and caregiver confidence using activities.
- `2003_hepburn_savvy-caregiver-transportable-program`: Dementia caregiver triage can include role-training needs, realistic care-goal formation, care-recipient capability estimation, and problem-solving support.
- `2022_hepburn_telesavvy-online-dementia-caregiver-program`: Online caregiver interventions should assess schedule fit, technology access, and readiness for synchronous/asynchronous participation.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Dementia caregiver assessment should cover support, tailored information, training/education needs, balance, respite, financial/legal support, medical/mental-health help, and changing needs across the disease trajectory.
- `2020_cheng_meta-review-dementia-caregiver-interventions`: Dementia caregiver triage should map assessed needs to specific intervention mechanisms and outcome targets rather than assuming all support should reduce burden.
- `2021_ruggiano_chatbots-dementia-caregivers`: Chatbot triage requires scope limits, privacy review, safe disclaimers, evidence provenance, failure handling, and referral/escalation pathways.

## Technology Components

- Caregiver identification fields.
- Risk screening.
- Needs assessment.
- Stress-process assessment fields.
- Physical and mental health outcome screening.
- Health behavior and self-care screening.
- Digital access, literacy, usability, and accessibility screening.
- Training and referral recommendations.
- Role and consent management.
- Monitoring for capacity mismatch or need for additional support.
- SCI-specific ADL/IADL and bowel/bladder care training needs.
- SCI-specific problem identification, problem-solving style, discharge-transition support, and remote or brief follow-up fit.
- SCI-specific formal/informal care mix, care hours, backup-care availability, care quality, and secondary-condition training needs.
- SCI-specific secondary-condition burden fields for bladder dysfunction, UTIs, pressure injuries, chronic pain, functional independence, and burden dimensions.
- SCI-specific coping, social support, respite, mental/physical health red flags, and future-planning fields.
- Financial and practical resource navigation.
- Caregiver Reaction Assessment-style burden domains.
- Dementia caregiver fields for behavior-response confidence, mastery, active training needs, schedule fit, technology access, and capacity for home-based or synchronous intervention participation.
- Dementia trajectory fields for caregiver support, information, training, balance, legal/financial planning, respite, and acceptance of help.
- Chatbot readiness fields for digital access, voice/text interaction fit, privacy expectations, urgency/safety risk, and need for human support.

## Design Constraints

- Assessment should support care planning and caregiver support; it should not become autonomous clinical decision-making.
- Assessment should distinguish stressors, resources, and outcomes rather than collapsing them into a single burden label.
- Care-recipient consent, autonomy, and privacy must shape what caregiver data are collected and shared.
- Escalation pathways require human review and clear responsibility boundaries.
- Match triage recommendations to evidence-supported mechanisms and label chatbot support as information or navigation support unless outcome evidence is available.

## Related Pages

- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`
- `wiki/evidence/gitlin_2010_cope_dementia_home_based_intervention.md`
- `wiki/evidence/hepburn_2003_savvy_caregiver_transportable_program.md`
- `wiki/evidence/hepburn_2022_telesavvy_online_dementia_caregiver_program.md`
- `wiki/evidence/bressan_2020_dementia_caregiver_needs_mixed_method_review.md`
- `wiki/evidence/cheng_2020_meta_review_dementia_caregiver_interventions.md`
- `wiki/evidence/ruggiano_2021_chatbots_dementia_caregivers.md`
- `wiki/evidence/elliott_2008_problem_solving_videoconferencing_sci_caregivers.md`
- `wiki/evidence/elliott_2009_brief_problem_solving_training_sci_caregivers.md`
- `wiki/evidence/smith_2016_caregiving_services_sci_systematic_review.md`
- `wiki/evidence/conti_2019_secondary_conditions_caregiver_burden_sci.md`
- `wiki/evidence/espino_2022_coping_social_support_caregiver_wellbeing_sci.md`
