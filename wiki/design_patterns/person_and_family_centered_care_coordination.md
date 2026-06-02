---
title: Person and Family-Centered Care Coordination
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [family-centered-care, care-coordination, shared-access, design-pattern]
last_updated: 2026-06-02
---

# Person and Family-Centered Care Coordination

## Pattern Summary

Design care coordination workflows that recognize family caregivers as care partners while preserving the care recipient's autonomy, privacy, preferences, and consent.

## Source-Backed Rationale

- `2016_nasem_families-caring-for-an-aging-america`: The report calls for person-centered care to evolve toward person- and family-centered care because caregivers are often expected to implement care plans while being excluded from decisions or training.
- `2020_schulz_family-caregiving-for-older-adults`: Caregivers commonly coordinate care, communicate with providers, advocate, and serve as surrogates across a cumulative care trajectory.
- `2017_nichols_reach-dementia-caregiver-healthcare-costs`: REACH VA suggests that structured dementia caregiver role support may fit integrated care-system coordination and cost evaluation.
- `2010_gitlin_cope-dementia-home-based-intervention`: COPE supports person- and family-centered home intervention through patient capability assessment, caregiver-identified concerns, health review, physician follow-up, and tailored action plans.
- `2003_hepburn_savvy-caregiver-transportable-program`: Savvy supports training caregivers for a dementia caregiving role while requiring facilitator fidelity and organizational support.

## Technology Components

- Role-aware shared access.
- Consent and proxy workflows.
- Provider-caregiver communication.
- Care transition support.
- Task lists and training materials.
- Audit logs and revocable permissions.

## Design Constraints

- Family-centered care is not permission to bypass care-recipient autonomy.
- Shared access requires clear privacy, consent, and auditability rules.
- Provider-facing systems should avoid assuming caregiver capacity without assessment.

## Related Pages

- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/design_patterns/caregiver_assessment_and_triage.md`
- `wiki/evidence/nichols_2017_reach_dementia_caregiver_healthcare_costs.md`
- `wiki/evidence/gitlin_2010_cope_dementia_home_based_intervention.md`
- `wiki/evidence/hepburn_2003_savvy_caregiver_transportable_program.md`
