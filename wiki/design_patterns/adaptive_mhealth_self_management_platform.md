---
title: Adaptive mHealth Self-Management Platform
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [adaptive-mhealth, self-management, platform, chronic-conditions, design-pattern]
last_updated: 2026-11-05
---

# Adaptive mHealth Self-Management Platform

## Pattern Summary

Use a configurable mHealth platform with modular self-management supports, caregiver support, clinician oversight, secure synchronization, and accessibility personalization.

## Source-Backed Rationale

- `2019-04-25_setiawan_adaptive-mhealth-self-management`: iMHere 2.0 was designed to address diverse needs across people with chronic conditions and disabilities, changing needs over time, and long-term engagement challenges.

## Relevant Populations

- People with chronic conditions and disabilities.

## Relevant Conditions

- Spinal cord injury.

## Technology Components

- Client app.
- Caregiver app.
- Web-based clinician portal.
- Secure two-way communication protocol.
- Back-end server.
- Adaptive modules.
- Persuasive and personalization features.
- Accessibility customization.

## Design Constraints

- Keep self-management support separate from autonomous clinical decision-making.
- Make caregiver and clinician access role-bound and consent-aware.
- Design for changing needs, long-term use, and device/platform differences.

## Evidence

- `2019-04-25_setiawan_adaptive-mhealth-self-management`.

## Long Access Does Not Establish Benefit

Svendsen provides an **adjacent patient-trial evaluation caution**: ten-module stress-management programs with 18-month access and early telephone support did not show a statistically significant overall advantage over usual care. Measure active use and outcomes separately; subgroup tailoring remains a hypothesis. The trial does not evaluate iMHere, caregiver systems, or complication prevention. See `wiki/evidence/svendsen_2026_digital_stress_management_breast_cancer.md`.

## Gaps

- Large-scale and long-term effectiveness remains to be established.

## Related Pages

- `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`
- `wiki/design_patterns/clinician_portal_supported_mhealth.md`
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`
