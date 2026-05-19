---
title: Accessibility-First mHealth Symptom Reporting
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [accessibility, mhealth, symptom-reporting, dexterity, design-pattern]
last_updated: 2026-05-18
---

# Accessibility-First mHealth Symptom Reporting

## Pattern Summary

Design mHealth symptom-reporting tools around accessibility constraints from the start, especially dexterity limitations, visual readability, and technology-literacy barriers.

## Source-Backed Rationale

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`: In a Raynaud app usability evaluation, participants reported difficulty with complex gestures, older adults flagged small font sizes and low contrast, and vague prompts caused hesitation among users with lower technology literacy.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: iMHere 2.0 includes customization for font size, font style, button size, line/button spacing, and hand preference to support people with fine motor and visual impairments.

## Relevant Populations

- People with chronic conditions and disabilities.
- Older adults, when accessibility barriers such as font size and contrast are relevant.

## Relevant Conditions

- Systemic sclerosis-associated Raynaud phenomenon.

## Technology Components

- Larger font sizes.
- High-contrast color themes.
- Single-tap interactions instead of swipe or complex gestures.
- Enlarged tap targets.
- Clear prompts that reduce fear of making mistakes.

## Design Constraints

- Do not treat accessibility as a cosmetic refinement after core functionality.
- Do not conflate condition-specific dexterity limitations with normal aging.
- Preserve care recipient autonomy and avoid unnecessary caregiver mediation when self-reporting is feasible.

## Evidence

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`.

## Gaps

- The source does not establish clinical effectiveness or long-term adherence outcomes.

## Related Pages

- `wiki/care_recipient_needs/symptom_self_reporting_and_tracking.md`
- `wiki/populations/people_with_chronic_conditions_and_disabilities.md`
- `wiki/populations/older_adults.md`
