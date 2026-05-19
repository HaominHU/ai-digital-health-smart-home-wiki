---
title: Research Wiki Memory
type: memory
status: draft
privacy: private
last_updated: 2026-05-18
---

# Research Wiki Memory

## Current State

This repo has been initialized as a private Karpathy-style LLM Wiki for AI-driven digital health and smart home technologies in caregiving, chronic conditions, disability, and aging.

The repo is intentionally Markdown-first and Obsidian-compatible. No database, embedding system, or custom retrieval tooling has been added.

## Core Purpose

The wiki should support:

- General knowledge answers grounded in accumulated research context.
- Evidence-aware research writing.
- System design reasoning.
- AI-ready prompts for research, writing, coding, design, or specification work.
- Knowledge support for agent reasoning.

The wiki must not act as a clinical decision-maker, diagnostic system, treatment recommender, or substitute for professional medical, ethical, privacy, security, or IRB review.

## Architecture Decisions

- Raw sources live under `sources/` and are treated as immutable.
- Maintained wiki pages live under `wiki/`.
- Generated previews, briefs, prompts, and reports live under `outputs/`.
- Sensitive scratch notes live under `private_notes/`.
- `AGENTS.md` governs agent behavior.
- `INDEX.md` is the content-oriented map.
- `LOG.md` is the chronological timeline.
- `MEMORY.md` is the compressed current-state digest.

## Domain Model

- Conditions are overlays.
- Caregiving challenges are reusable hubs.
- Care recipient needs are tracked separately from caregiver needs.
- Technologies are reusable intervention lenses.
- Aging-related functional decline and age-associated disease development must be distinguished.
- Evidence, interpretation, personal insight, and speculative design direction must remain separate.

Current condition priority order:

1. Spinal cord injury.
2. Dementia.
3. Falls and general aging issues.
4. Multiple chronic conditions in aging.
5. Systemic sclerosis-associated Raynaud phenomenon.
6. Postpartum women.
7. Gynecological cancer.

## Privacy and Security Baseline

The repo is private by default, but identifiable or sensitive healthcare/study data should not be stored unless the user explicitly provides a safe handling policy.

Default behavior:

- Avoid PHI and identifiable participant information.
- De-identify before wiki integration.
- Mark sensitive source material clearly.
- Include privacy, security, consent, ethics, data minimization, and human oversight considerations in healthcare-related prompts and specs.

## Source Storage and Git Baseline

The user manually handles commits and git management.

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The tracked wiki should preserve source-derived knowledge through source IDs, source context, evidence labels, and durable Markdown synthesis.

Recommended raw source ID and filename pattern:

`YYYY-MM-DD_author-or-org_short-title.ext`

Periodic lint checks should flag locally stored raw sources that may be removable after their contents have been well digested into the wiki. Do not delete raw sources automatically.

## Next Useful Step

Continue one-by-one source ingest from `sources/abstracts/` and `sources/papers/`.

First integrated source:

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: AMIA abstract on human-centered design recommendations for generative AI in mHealth apps for family caregivers.

New source-backed hubs from the first ingest:

- Caregiver time burden and engagement.
- Information access and health literacy.
- Emotional and social support.
- Adaptive AI layer for caregiver mHealth.
- Trajectory-sensitive caregiver content.

Condition mapping note:

- Broad "neurological conditions" evidence may be mapped cautiously to spinal cord injury when there is no specific non-SCI neurological condition mention, while preserving the source wording and avoiding unsupported SCI-specific claims.

Second integrated source:

- `2026-05-18_hu_raynaud-phenomenon-mhealth-usability`: AMIA abstract on usability evaluation and iterative refinement of a Raynaud mHealth app for people with systemic sclerosis-associated Raynaud phenomenon.

New source-backed hubs from the second ingest:

- Symptom self-reporting and tracking.
- Accessibility-first mHealth symptom reporting.
- Real-world reliability for mHealth data capture.

Condition mapping note:

- Raynaud usability evidence maps directly to systemic sclerosis-associated Raynaud phenomenon. Older-adult relevance is limited to accessibility/usability barriers noted in the source and should not be treated as evidence that SSc-RP is normal aging.

Third integrated source:

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: AMIA abstract comparing source-reported ChatGPT and ChatGPT Health interfaces for spinal cord injury pre-clinic preparation without connected records.

New source-backed hubs from the third ingest:

- Pre-clinic preparation and advocacy.
- AI-assisted pre-clinic preparation.
- Care-recipient-style prompting for empathy.

AI product/model note:

- Product and model details from this abstract are source-reported and may change. Re-verify current product capabilities before making current-state claims about OpenAI products.

Fourth integrated source:

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Hu's 2024 University of Pittsburgh dissertation on developing a multi-component mHealth app for family caregivers of people with chronic conditions and disabilities.

New source-backed hubs from the fourth ingest:

- Care coordination and shared access.
- Caregiver self-care and health tracking.
- Adaptive modular caregiver mHealth.
- One-stop caregiver support app.
- AI and wearable-augmented caregiver support.

Dissertation condition mapping note:

- Map dissertation condition-specific content only to spinal cord injury and gynecological cancer for current wiki purposes. Spina bifida, cerebral palsy, and traumatic brain injury remain source-level study-composition details unless the user later changes the condition priority list.

Fifth integrated source:

- `2019-04-25_setiawan_adaptive-mhealth-self-management`: Setiawan et al. 2019 JMIR Formative Research paper on iMHere 2.0 as adaptive mHealth self-management infrastructure for people with chronic conditions and disabilities.

System foundation note:

- Setiawan 2019 and Hu's dissertation jointly ground the user's caregiver research, system infrastructure, and future system expansion. Setiawan 2019 anchors the adaptive mHealth infrastructure for PwCCD self-management; Hu's dissertation extends the research line toward family caregiver support, caregiver-specific modules, and future AI/wearable/clinical workflow expansion.

New source-backed hubs from the fifth ingest:

- Self-management and secondary complication prevention.
- Adaptive mHealth self-management platform.
- Clinician portal-supported mHealth.
