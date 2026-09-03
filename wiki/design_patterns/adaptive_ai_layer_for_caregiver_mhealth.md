---
title: Adaptive AI Layer for Caregiver mHealth
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [generative-ai, mhealth, family-caregivers, adaptive-support, design-pattern]
last_updated: 2026-09-03
---

# Adaptive AI Layer for Caregiver mHealth

## Pattern Summary

Use generative AI as an adaptive support layer within caregiver mHealth rather than as a standalone chatbot or autonomous care decision-maker.

## Source-Backed Rationale

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: An AMIA abstract synthesizing iterative human-centered design of the iMHere Family Caregiver App concluded that future generative AI may be useful for proactive engagement, personalized content delivery, and responsive emotional and social support. Generative AI was not implemented in the evaluated app.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG provides technical rationale for grounding adaptive caregiver content in retrieved sources.
- `2023_yao_react-reasoning-acting-language-models`: ReAct provides technical rationale for bounded agentic interaction, stepwise tool use, and inspectable action traces.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition caregiver support.
- Dementia.
- Gynecological cancer.
- Spinal cord injury, when broad neurological-condition caregiver evidence is relevant and no specific non-SCI condition is named.

## Technology Components

- Agentic interaction layer for context-sensitive prompts.
- Adaptive content layer using retrieval-augmented generation or large language models.
- Emotional and social layer using multimodal AI, emotional check-ins, peer matching, and dynamic resource directories.
- Curated retrieval index with source provenance.
- Permissioned tool/action layer with logs and human confirmation.

## Design Constraints

- Keep the AI role bounded to research, design, and knowledge support unless a separate reviewed scope is defined.
- Preserve human oversight, escalation boundaries, privacy, consent, access control, auditability, and bias monitoring.
- Avoid unsupported claims that AI improves health outcomes until source-backed.
- Do not expose private scratch reasoning or sensitive chain-of-thought; provide user-facing summaries, sources, and action logs.
- Treat RAG and ReAct as technical method sources, not caregiver intervention evidence.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`.
- `2023_yao_react-reasoning-acting-language-models`.

## Gaps

- Needs implementation and evaluation evidence for generative AI features.
- Needs safety, privacy, and escalation validation before use with vulnerable populations.

## Explainable and Contestable Prioritization

Aliviado care partners requested a clear rationale when machine-learning symptom priorities differed from their own, with the option to retain their choice. Apply this as human-centered design rationale for user-facing explanations, uncertainty, disagreement, and reviewable priorities; it is not evidence for generative AI performance. Clinical-risk routing still requires separately reviewed safeguards and human oversight. See `wiki/evidence/fernandez_cajavilca_2026_aliviado_caregiving_app_design.md`.

## Related Pages

- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`
- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/caregiving_challenges/emotional_and_social_support.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`
