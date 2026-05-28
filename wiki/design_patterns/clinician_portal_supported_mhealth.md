---
title: Clinician Portal-Supported mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [clinician-portal, mhealth, care-team, self-management, design-pattern]
last_updated: 2026-05-27
---

# Clinician Portal-Supported mHealth

## Pattern Summary

Use a clinician-facing portal to configure mHealth modules, review self-management data, adapt intervention regimens, message users, and coordinate care-team support.

## Source-Backed Rationale

- `2019-04-25_setiawan_adaptive-mhealth-self-management`: The iMHere 2.0 clinician portal allowed clinicians to select modules, customize interventions, monitor progress, adjust regimens, message users, and synchronize changes to client and caregiver apps.
- `2016_nasem_families-caring-for-an-aging-america`: Provider systems should identify, assess, engage, train, support, and refer family caregivers; payment and delivery systems often need redesign to support these interactions.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Provider-supported caregiver interventions should specify targeted caregiving activities and caregiver/care-recipient outcomes.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: Portal-supported interventions need evaluation of organizational adoption, implementation consistency, and maintenance in routine care, not just patient-level efficacy.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes a health care provider interface for approving clients with dementia, updating client information, and discussing care plans with caregivers.

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
- Adoption, fidelity, workflow-fit, and maintenance metrics.
- Care-plan discussion tools and provider-facing client management.

## Design Constraints

- Portal support should assist clinician review and coordination, not replace clinical judgment.
- Access control, auditability, secure messaging, and clear escalation boundaries are required.
- Care recipient consent and autonomy must be preserved when caregivers are also connected.
- Portal designs should account for clinic staffing, reimbursement, training, and workflow burden as adoption and maintenance constraints.

## Evidence

- `2019-04-25_setiawan_adaptive-mhealth-self-management`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`.
- `2001_glasgow_re-aim-framework-chronic-illness-management`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.

## Gaps

- Larger trials are needed to assess clinical and implementation outcomes.
- Caregiver-facing portal functions need evaluation of caregiver activity changes, caregiver outcomes, care-recipient outcomes, provider workload, utilization, and cost.

## Related Pages

- `wiki/design_patterns/adaptive_mhealth_self_management_platform.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
