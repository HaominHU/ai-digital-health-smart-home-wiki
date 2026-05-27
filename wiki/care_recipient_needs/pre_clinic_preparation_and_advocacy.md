---
title: Pre-Clinic Preparation and Advocacy
type: care_recipient_need
status: draft
privacy: private
evidence_status: has_sources
tags: [pre-clinic-preparation, self-advocacy, care-recipient, spinal-cord-injury]
last_updated: 2026-05-27
---

# Pre-Clinic Preparation and Advocacy

## Need Summary

Care recipients may need help preparing questions, organizing concerns, drafting messages, and advocating for themselves during brief clinical encounters.

## Relevant Populations

- People with chronic conditions and disabilities.
- People with spinal cord injury.

## Relevant Conditions

- Spinal cord injury.

## Evidence

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: The abstract describes pre-clinic preparation as a critical but underserved need for individuals with spinal cord injury, who may face complex, multi-system health challenges and need to advocate for their needs during brief clinical encounters.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG can inform technical architecture for grounding preparation outputs in retrieved source context, but is not health-context effectiveness evidence.
- `2023_yao_react-reasoning-acting-language-models`: ReAct can inform stepwise source lookup and draft preparation patterns, but should not be used for autonomous clinical decision-making.

## Technology Support Lens

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AI tools were explored for pre-clinic preparation without connected EHR or wearable data. Structured outputs included support for portal message drafts, caregiver tools, and multi-deliverable preparation materials.
- Source-grounded generation and bounded reasoning-action workflows may support draft preparation when sources, actions, and communications remain reviewable by the care recipient.

## Design Implications

- Keep preparation support separate from diagnosis or treatment recommendation.
- Support self-advocacy while preserving care-recipient autonomy, privacy, and control over what information is shared.
- Treat prompts written in care-recipient style as a human-centered design variable, not just a technical formatting detail.
- Require care-recipient review and consent before sharing AI-generated questions, summaries, or portal-message drafts.
- Keep retrieved sources and proposed actions visible enough for review without exposing private scratch reasoning.

## Gaps

- The source is exploratory and does not evaluate clinical outcomes.
- Record-connected AI support remains an unresolved privacy, safety, and acceptability question.

## Related Pages

- `wiki/conditions/spinal_cord_injury.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/design_patterns/ai_assisted_pre_clinic_preparation.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`
