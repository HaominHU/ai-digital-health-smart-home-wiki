---
title: AI-Assisted Pre-Clinic Preparation
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [ai, pre-clinic-preparation, spinal-cord-injury, design-pattern]
last_updated: 2026-08-06
---

# AI-Assisted Pre-Clinic Preparation

## Pattern Summary

Use AI to help care recipients organize concerns, generate questions, prepare portal messages, and create structured visit-preparation materials before clinical encounters.

## Source-Backed Rationale

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: In an exploratory SCI pre-clinic preparation evaluation, a source-reported health-focused ChatGPT interface provided more structured support for caregiver tools, portal message drafts, and multi-deliverable outputs than standard ChatGPT when no records were connected.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG supports a technical architecture for grounding generated preparation materials in retrieved source context.
- `2023_yao_react-reasoning-acting-language-models`: ReAct supports a technical architecture for stepwise source lookup, reasoning, and draft preparation through bounded tool use.
- `2026-07-31_richter_llm-physician-patient-communication-review`: Written LLM responses were often rated more empathic in early studies, but perceived empathy is not evidence of accuracy, trust, safety, or clinical benefit.
- `2026-07-24_hong_caregiver-activation-concept-analysis`: Caregiver activation supports attention to communication, collaboration, help seeking, and advocacy readiness while preserving professional responsibility.

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
- Curated retrieval corpus with source traceability.
- Permissioned tool actions for lookup, drafting, and checklist generation.

## Design Constraints

- The AI should support preparation and communication, not diagnose, recommend treatment, or replace clinical judgment.
- Product/model behavior can change over time, so source-reported product details should not be treated as stable facts without re-verification.
- Avoid requiring EHR or wearable linkage unless privacy, consent, security, and trust implications have been reviewed.
- Require human review before portal messages, care-team communication, or clinical questions are sent.
- Keep retrieved sources and action logs available for review.
- Evaluate supportive tone, evidence support, factual accuracy, completeness, and action safety as separate dimensions.

## Evidence

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`.
- `2023_yao_react-reasoning-acting-language-models`.
- `2026-07-31_richter_llm-physician-patient-communication-review`.
- `2026-07-24_hong_caregiver-activation-concept-analysis`.

## Gaps

- Small exploratory evaluation.
- AI judge scoring rather than patient, caregiver, clinician, or outcome-based validation.
- Record-connected use was not evaluated.
- Context contamination was observed as an accuracy issue.

## Related Pages

- `wiki/design_patterns/care_recipient_style_prompting_for_empathy.md`
- `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`
- `wiki/conditions/spinal_cord_injury.md`
- `wiki/technologies/ai_driven_digital_health.md`
