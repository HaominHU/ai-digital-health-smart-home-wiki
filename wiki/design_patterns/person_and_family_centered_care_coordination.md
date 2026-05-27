---
title: Person and Family-Centered Care Coordination
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [family-centered-care, care-coordination, shared-access, design-pattern]
last_updated: 2026-05-26
---

# Person and Family-Centered Care Coordination

## Pattern Summary

Design care coordination workflows that recognize family caregivers as care partners while preserving the care recipient's autonomy, privacy, preferences, and consent.

## Source-Backed Rationale

- `2016_nasem_families-caring-for-an-aging-america`: The report calls for person-centered care to evolve toward person- and family-centered care because caregivers are often expected to implement care plans while being excluded from decisions or training.
- `2020_schulz_family-caregiving-for-older-adults`: Caregivers commonly coordinate care, communicate with providers, advocate, and serve as surrogates across a cumulative care trajectory.

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

