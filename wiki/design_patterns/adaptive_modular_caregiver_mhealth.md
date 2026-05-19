---
title: Adaptive Modular Caregiver mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [mhealth, adaptive-design, modular-design, family-caregivers, design-pattern]
last_updated: 2026-05-18
---

# Adaptive Modular Caregiver mHealth

## Pattern Summary

Build caregiver mHealth systems as modular app suites that combine general caregiver support, reusable condition-specific interfaces, and condition-unique content or modules.

## Source-Backed Rationale

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: The dissertation describes an adaptive modular infrastructure with general modules for all family caregivers, general modules with condition-specific content, data interfaces, and condition-specific modules.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: The iMHere 2.0 paper grounds the system infrastructure behind this research line, including adaptive modules, caregiver app, clinician portal, secure synchronization, and scalable architecture that can support future expansion.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Spinal cord injury.
- Gynecological cancer.

## Technology Components

- Configurable modules.
- General caregiver self-care tools.
- Condition-specific educational content.
- Resource libraries.
- Risk assessment.
- Goals and plans.

## Design Constraints

- Keep reusable caregiver challenges separate from condition overlays.
- Do not turn participant-composition conditions into new wiki condition taxonomies unless explicitly prioritized.
- Treat future AI and wearable augmentation as an extension layer unless implemented and evaluated.

## Evidence

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`.

## Gaps

- Needs broader testing across caregiver populations and conditions.
- Needs outcome evidence beyond usability, acceptability, and feasibility.

## Related Pages

- `wiki/design_patterns/one_stop_caregiver_support_app.md`
- `wiki/populations/family_caregivers.md`
