---
title: Reasoning-Action Health AI Agent
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [react, agentic-ai, tool-use, human-oversight, design-pattern]
last_updated: 2026-05-27
---

# Reasoning-Action Health AI Agent

## Pattern Summary

Use a tightly bounded reasoning-plus-action architecture when an AI system needs to perform multi-step knowledge-support work through tools, source lookup, drafting, task tracking, or resource navigation.

## Source-Backed Rationale

- `2023_yao_react-reasoning-acting-language-models`: ReAct interleaves reasoning traces and task-specific actions, allowing models to gather external information and produce inspectable trajectories.
- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Future caregiver mHealth directions include agentic interaction for proactive engagement and context-sensitive prompts.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AI-assisted preparation can support question generation, portal-message drafts, and structured visit-preparation outputs without autonomous clinical decision-making.

## Relevant Uses

- Stepwise pre-clinic preparation.
- Source lookup and evidence-grounded drafting.
- Care coordination draft support.
- Resource-navigation support.
- Research/design prompt generation.
- Smart-home task support only when actions are permissioned and non-dangerous.

## Design Constraints

- Do not allow autonomous diagnosis, treatment recommendation, care escalation, medication changes, or unsafe home automation.
- Keep action spaces permissioned, logged, auditable, and reversible where possible.
- Require human confirmation before external communication, care-plan changes, purchases, data sharing, or device actuation.
- Do not expose sensitive chain-of-thought or private scratch reasoning to users; provide concise rationale, sources, and action logs instead.
- Evaluate failure modes including hallucinated actions, privacy leakage, overconfident plans, context-length failures, and caregiver workload transfer.

## Evidence

- `2023_yao_react-reasoning-acting-language-models`.
- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`.

## Gaps

- Needs health-domain validation, safety testing, and governance before use in real caregiving or clinical workflows.
- Needs evaluation against RE-AIM dimensions, privacy/security requirements, and caregiver/care-recipient outcomes.

## Related Pages

- `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
