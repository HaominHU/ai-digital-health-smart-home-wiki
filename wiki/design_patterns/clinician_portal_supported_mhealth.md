---
title: Clinician Portal-Supported mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [clinician-portal, mhealth, care-team, self-management, design-pattern]
last_updated: 2026-05-18
---

# Clinician Portal-Supported mHealth

## Pattern Summary

Use a clinician-facing portal to configure mHealth modules, review self-management data, adapt intervention regimens, message users, and coordinate care-team support.

## Source-Backed Rationale

- `2019-04-25_setiawan_adaptive-mhealth-self-management`: The iMHere 2.0 clinician portal allowed clinicians to select modules, customize interventions, monitor progress, adjust regimens, message users, and synchronize changes to client and caregiver apps.

## Relevant Populations

- People with chronic conditions and disabilities.

## Relevant Conditions

- Spinal cord injury.

## Technology Components

- Triage dashboard.
- Patient-context panel.
- Module management.
- Care-team management.
- Instant messaging.
- Alerts by SMS or email for urgent/severe conditions.

## Design Constraints

- Portal support should assist clinician review and coordination, not replace clinical judgment.
- Access control, auditability, secure messaging, and clear escalation boundaries are required.
- Care recipient consent and autonomy must be preserved when caregivers are also connected.

## Evidence

- `2019-04-25_setiawan_adaptive-mhealth-self-management`.

## Gaps

- Larger trials are needed to assess clinical and implementation outcomes.

## Related Pages

- `wiki/design_patterns/adaptive_mhealth_self_management_platform.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
