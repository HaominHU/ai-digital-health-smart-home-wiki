---
title: Real-World Reliability for mHealth Data Capture
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [mhealth, reliability, data-capture, cache, design-pattern]
last_updated: 2026-05-18
---

# Real-World Reliability for mHealth Data Capture

## Pattern Summary

Design mHealth data-capture systems to remain reliable during everyday context changes such as indoor-outdoor transitions, unstable networks, stale cache states, and interrupted use.

## Source-Backed Rationale

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`: A Raynaud app usability abstract reported that network instability and cache staleness contributed to incomplete data collection during indoor-outdoor environmental transitions and occasional app crashes. An automated cache-refresh mechanism was introduced in response.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: iMHere 2.0 supports temporary local storage and secure transmission when network connection returns for most modules, while personal health record data require network access for security. The feasibility study also identified older Android device compatibility and app-freezing issues.

## Relevant Populations

- People with chronic conditions and disabilities who use mobile tools for symptom reporting.

## Relevant Conditions

- Systemic sclerosis-associated Raynaud phenomenon.

## Technology Components

- Cache-refresh strategies.
- Offline or unstable-network handling.
- Data-completeness safeguards.
- Real-world feedback loops after lab usability testing.

## Design Constraints

- Lab usability findings should be validated against real-world use when possible.
- Reliability failures can become evidence-quality failures when the system is used for research data capture.

## Evidence

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`.

## Gaps

- The abstract describes trial feedback as naturalistic validation of usability themes, not as a second formal usability evaluation.
- Larger real-world studies are still needed.

## Related Pages

- `wiki/care_recipient_needs/symptom_self_reporting_and_tracking.md`
- `wiki/conditions/systemic_sclerosis_associated_raynaud_phenomenon.md`
