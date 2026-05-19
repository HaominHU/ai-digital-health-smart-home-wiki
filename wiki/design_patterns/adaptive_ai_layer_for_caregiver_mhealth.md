---
title: Adaptive AI Layer for Caregiver mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [generative-ai, mhealth, family-caregivers, adaptive-support, design-pattern]
last_updated: 2026-05-18
---

# Adaptive AI Layer for Caregiver mHealth

## Pattern Summary

Use generative AI as an adaptive support layer within caregiver mHealth rather than as a standalone chatbot or autonomous care decision-maker.

## Source-Backed Rationale

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: An AMIA abstract synthesizing iterative human-centered design of the iMHere Family Caregiver App concluded that future generative AI may be useful for proactive engagement, personalized content delivery, and responsive emotional and social support. Generative AI was not implemented in the evaluated app.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Gynecological cancer.
- Spinal cord injury, when broad neurological-condition caregiver evidence is relevant and no specific non-SCI condition is named.

## Technology Components

- Agentic interaction layer for context-sensitive prompts.
- Adaptive content layer using retrieval-augmented generation or large language models.
- Emotional and social layer using multimodal AI, emotional check-ins, peer matching, and dynamic resource directories.

## Design Constraints

- Keep the AI role bounded to research, design, and knowledge support unless a separate reviewed scope is defined.
- Preserve human oversight, escalation boundaries, privacy, consent, access control, auditability, and bias monitoring.
- Avoid unsupported claims that AI improves health outcomes until source-backed.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.

## Gaps

- Needs implementation and evaluation evidence for generative AI features.
- Needs safety, privacy, and escalation validation before use with vulnerable populations.

## Related Pages

- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`
- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/caregiving_challenges/emotional_and_social_support.md`
