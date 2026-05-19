---
title: AI-Assisted Pre-Clinic Preparation
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [ai, pre-clinic-preparation, spinal-cord-injury, design-pattern]
last_updated: 2026-05-18
---

# AI-Assisted Pre-Clinic Preparation

## Pattern Summary

Use AI to help care recipients organize concerns, generate questions, prepare portal messages, and create structured visit-preparation materials before clinical encounters.

## Source-Backed Rationale

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: In an exploratory SCI pre-clinic preparation evaluation, a source-reported health-focused ChatGPT interface provided more structured support for caregiver tools, portal message drafts, and multi-deliverable outputs than standard ChatGPT when no records were connected.

## Relevant Populations

- People with spinal cord injury.
- People with chronic conditions and disabilities.

## Relevant Conditions

- Spinal cord injury.

## Technology Components

- LLM-based question preparation.
- Portal message drafting.
- Multi-deliverable visit preparation.
- Scenario-based prompts.
- Care-recipient-style prompts.

## Design Constraints

- The AI should support preparation and communication, not diagnose, recommend treatment, or replace clinical judgment.
- Product/model behavior can change over time, so source-reported product details should not be treated as stable facts without re-verification.
- Avoid requiring EHR or wearable linkage unless privacy, consent, security, and trust implications have been reviewed.

## Evidence

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`.

## Gaps

- Small exploratory evaluation.
- AI judge scoring rather than patient, caregiver, clinician, or outcome-based validation.
- Record-connected use was not evaluated.
- Context contamination was observed as an accuracy issue.

## Related Pages

- `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`
- `wiki/conditions/spinal_cord_injury.md`
- `wiki/technologies/ai_driven_digital_health.md`
