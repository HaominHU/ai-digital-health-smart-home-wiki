---
title: Trajectory-Sensitive Caregiver Content
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [caregiving-trajectory, adaptive-content, health-literacy, design-pattern]
last_updated: 2026-05-26
---

# Trajectory-Sensitive Caregiver Content

## Pattern Summary

Adapt caregiver-facing information to the caregiver's trajectory stage, experience level, literacy needs, and current care context.

## Source-Backed Rationale

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Caregivers reported that informational needs shift across the caregiving trajectory; newly onboarded caregivers may need different support than experienced caregivers managing long-term routines.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver tasks can accumulate across a trajectory from sporadic support to IADL/ADL care, end-of-life care, institutional transition, death, and bereavement, with disease-specific trajectories such as stroke or cancer varying in pace and learning demands.
- `2016_nasem_families-caring-for-an-aging-america`: Caregiver supports should account for caregiver duration, high-need older-adult care, diversity, employment, and system navigation context.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Gynecological cancer.
- Spinal cord injury, when broad neurological-condition caregiver evidence is relevant and no specific non-SCI condition is named.

## Technology Components

- Plain-language condition-specific education.
- Retrieval-augmented generation or large language model support for adapting content to literacy level and trajectory stage.
- Resource libraries that distinguish universal caregiver content, reusable condition-specific interfaces, and condition-unique modules.

## Design Constraints

- Separate educational support from clinical recommendation.
- Track source provenance for generated or retrieved content.
- Avoid assuming one caregiving stage, condition, or literacy profile fits all users.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2020_schulz_family-caregiving-for-older-adults`.
- `2016_nasem_families-caring-for-an-aging-america`.

## Gaps

- The source proposes future AI-supported adaptive content but does not evaluate deployed generative AI content adaptation.

## Related Pages

- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/populations/family_caregivers.md`
- `wiki/technologies/ai_driven_digital_health.md`
