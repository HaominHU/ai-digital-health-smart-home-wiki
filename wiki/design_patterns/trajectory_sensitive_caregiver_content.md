---
title: Trajectory-Sensitive Caregiver Content
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [caregiving-trajectory, adaptive-content, health-literacy, design-pattern]
last_updated: 2026-06-07
---

# Trajectory-Sensitive Caregiver Content

## Pattern Summary

Adapt caregiver-facing information to the caregiver's trajectory stage, experience level, literacy needs, and current care context.

## Source-Backed Rationale

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Caregivers reported that informational needs shift across the caregiving trajectory; newly onboarded caregivers may need different support than experienced caregivers managing long-term routines.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver tasks can accumulate across a trajectory from sporadic support to IADL/ADL care, end-of-life care, institutional transition, death, and bereavement, with disease-specific trajectories such as stroke or cancer varying in pace and learning demands.
- `2016_nasem_families-caring-for-an-aging-america`: Caregiver supports should account for caregiver duration, high-need older-adult care, diversity, employment, and system navigation context.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Dementia caregiver needs change as symptoms, tasks, family roles, and service needs evolve; content should adapt across support, information, training, and balance needs.
- `2020_cheng_meta-review-dementia-caregiver-interventions`: Dementia caregiver content should be tied to target outcomes and intervention mechanism, such as knowledge, communication skill, mastery, depression, quality of life, burden, anxiety, or social support.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Gynecological cancer.
- Dementia.
- Spinal cord injury, when broad neurological-condition caregiver evidence is relevant and no specific non-SCI condition is named.

## Technology Components

- Plain-language condition-specific education.
- Retrieval-augmented generation or large language model support for adapting content to literacy level and trajectory stage.
- Resource libraries that distinguish universal caregiver content, reusable condition-specific interfaces, and condition-unique modules.
- Dementia trajectory content for diagnosis, symptoms, behavioral change, medications, emergencies, home adaptation, incontinence, nutrition, services, financial/legal planning, respite, and self-care balance.

## Design Constraints

- Separate educational support from clinical recommendation.
- Track source provenance for generated or retrieved content.
- Avoid assuming one caregiving stage, condition, or literacy profile fits all users.
- Distinguish information-only education from active training, coaching, psychotherapy/counseling, communication practice, or referral because these mechanisms support different outcome claims.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2020_schulz_family-caregiving-for-older-adults`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`.
- `2020_cheng_meta-review-dementia-caregiver-interventions`.

## Gaps

- The source proposes future AI-supported adaptive content but does not evaluate deployed generative AI content adaptation.

## Related Pages

- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/populations/family_caregivers.md`
- `wiki/technologies/ai_driven_digital_health.md`
