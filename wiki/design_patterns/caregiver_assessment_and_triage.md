---
title: Caregiver Assessment and Triage
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [caregiver-assessment, triage, care-coordination, design-pattern]
last_updated: 2026-05-27
---

# Caregiver Assessment and Triage

## Pattern Summary

Identify caregivers, assess their risks, needs, strengths, preferences, capacity, and willingness, then route them to appropriate training, support, referrals, or escalation pathways.

## Source-Backed Rationale

- `2016_nasem_families-caring-for-an-aging-america`: The National Academies report recommends routine caregiver identification and assessment in health care and LTSS, including caregiver health, stress, skills, employment, willingness, and support needs.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver risk varies by intensity, duration, care recipient suffering, behavioral symptoms, caregiver health, support availability, perceived choice, and home environment.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregiver assessment should include preparedness, physical burden, sleep disruption, financial strain, social support, coping strategies, and need for training or counselling.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: Advanced ovarian cancer caregiver assessment can use CRA-informed domains such as disrupted schedules, financial problems, lack of family support, health problems, and caregiver self-esteem.

## Technology Components

- Caregiver identification fields.
- Risk screening.
- Needs assessment.
- Training and referral recommendations.
- Role and consent management.
- Monitoring for capacity mismatch or need for additional support.
- SCI-specific ADL/IADL and bowel/bladder care training needs.
- Financial and practical resource navigation.
- Caregiver Reaction Assessment-style burden domains.

## Design Constraints

- Assessment should support care planning and caregiver support; it should not become autonomous clinical decision-making.
- Care-recipient consent, autonomy, and privacy must shape what caregiver data are collected and shared.
- Escalation pathways require human review and clear responsibility boundaries.

## Related Pages

- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`
