---
title: Retrieval-Grounded Health AI Support
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [rag, source-grounding, ai, digital-health, design-pattern]
last_updated: 2026-06-07
---

# Retrieval-Grounded Health AI Support

## Pattern Summary

Use retrieval-augmented generation to ground AI support in a curated source base, preserving source traceability while adapting outputs to a caregiver, care recipient, researcher, or clinician-facing task.

## Source-Backed Rationale

- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG combines a parametric generator with non-parametric retrieved documents and can update knowledge through the external index.
- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Future caregiver mHealth AI directions include retrieval-augmented generation for condition-specific content and trajectory-sensitive support.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AI-assisted pre-clinic preparation should distinguish record-free support from record-connected systems with stronger privacy, consent, and trust implications.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy uses a RAG-supported chatbot with internal Q&A content, external sources, confidence thresholds, empathetic context generation, and urgent/sensitive-case routing to helpline resources.
- `2021_ruggiano_chatbots-dementia-caregivers`: Dementia chatbot reviews show why source provenance, content vetting, privacy statements, safe disclaimers, dialog failure handling, and end-user evaluation are necessary before treating conversational support as reliable health knowledge support.

## Relevant Uses

- Caregiver education and resource navigation.
- Pre-clinic question preparation and portal-message drafting.
- Condition-specific content adaptation.
- Research literature synthesis and prompt generation.
- Wiki-grounded knowledge support.
- Dementia caregiver symptom-management and resource-navigation support.
- Dementia chatbot education, self-assessment, reminiscence, and resource linking when sources, scope limits, and escalation pathways are explicit.

## Design Constraints

- Use curated and versioned source corpora for health-related outputs.
- Show or retain source provenance for generated claims.
- Keep generated content in research, design, preparation, or knowledge-support scope unless separately validated.
- Do not treat retrieval as proof of correctness; source quality, retrieval quality, and generation quality must be evaluated separately.
- Protect sensitive user data before retrieval, indexing, or logging.
- Define confidence thresholds, out-of-scope behavior, and escalation pathways for urgent or sensitive queries.
- Do not treat retrieval-grounding, chatbot availability, or scripted dialog as evidence of caregiver or clinical outcome effectiveness.

## Evidence

- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`.
- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.
- `2021_ruggiano_chatbots-dementia-caregivers`.

## Gaps

- Needs health-domain validation with target users and expert review.
- Needs evaluation of privacy, fairness, literacy adaptation, citation faithfulness, and failure modes.

## Related Pages

- `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/design_patterns/ai_assisted_pre_clinic_preparation.md`
