---
title: Information Access and Health Literacy
type: caregiving_challenge
status: draft
privacy: private
evidence_status: has_sources
tags: [health-literacy, information-access, education, caregiving]
last_updated: 2026-05-28
---

# Information Access and Health Literacy

## Challenge Summary

Reusable caregiving challenge hub for making health, care, and resource information understandable and usable across caregiver literacy levels, experience levels, and care trajectories.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition challenge.
- Gynecological cancer.
- May apply to spinal cord injury when broad neurological-condition caregiver evidence is relevant and no specific non-SCI condition is named.

## Caregiver Need

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Caregivers with lower health literacy found some educational resources inaccessible, and caregivers across stages reported that information needs shift over time.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Dissertation participants needed reliable, concise, condition-specific education and caregiver-facing resources. Resource library content could be useful as a digital archive, but preset PDF resources could feel too professional or reading-intensive for some caregivers.
- `2016_nasem_families-caring-for-an-aging-america`: Family caregivers are often expected to perform medical, personal care, and coordination tasks with little training; provider systems need capacity to assess and support caregiver training needs.
- `2020_schulz_family-caregiving-for-older-adults`: Multicomponent psychosocial interventions often include education about disease, disease progression, resources, communication, and coping.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Clinical skills and knowledge are caregiving activity targets, including disease knowledge, service knowledge, problem solving, adherence to guidelines, and decision-making skills.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregivers in the Ghanaian study often felt unprepared for sudden caregiving responsibilities; the authors recommend training and counselling for family caregivers.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: Oncology nursing recommendations include preparing caregivers for advanced ovarian cancer care and providing symptom-management education before discharge or home care.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: Educational and self-management interventions should be evaluated for reach and representativeness, because referral requirements, scheduling, cost, transportation, and literacy or technology barriers can limit participation.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG provides technical rationale for retrieving source material and generating adapted outputs, but does not establish healthcare or caregiver education effectiveness.
- `2023_yao_react-reasoning-acting-language-models`: ReAct provides technical rationale for stepwise information seeking with external tools, but health use requires source verification and bounded action spaces.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: Dementia caregivers valued curated dementia trajectory, behavioral/physical symptom management, grief, stress, self-care, and service-directory content; early feedback also flagged textual overload, leading to content and navigation refinements.

## Care Recipient Connection

To be further source-backed.

## Technology Support Lens

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`: Retrieval-augmented generation and large language models were proposed as possible ways to generate condition-specific content at the caregiver's literacy level and trajectory stage.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: The dissertation supports adaptive modular delivery of general caregiver content and condition-specific content through reusable interfaces, with future RAG/chatbot directions framed as future work.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: Telephone, interactive computer, mailed, and policy modalities may change reach, adoption, implementation, and maintenance compared with face-to-face education.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: Retrieval-grounded systems can connect generated education to retrieved source passages.
- `2023_yao_react-reasoning-acting-language-models`: Reasoning-action systems can structure search, lookup, and draft-generation workflows.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy uses a RAG-supported chatbot, structured Q&A database, tiered confidence retrieval, and source-reported urgent/sensitive-case routing to helpline resources.

## Evidence

- `2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth`.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2020_schulz_family-caregiving-for-older-adults`.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`.
- `2001_glasgow_re-aim-framework-chronic-illness-management`.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`.
- `2023_yao_react-reasoning-acting-language-models`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.

## Design Implications

- Separate condition-specific information from reusable interface patterns.
- Track caregiver literacy level and caregiving trajectory as design variables.
- Generated education should remain knowledge support and should not become diagnosis, treatment recommendation, or autonomous clinical advice.
- Record whether a design claim targets knowledge, clinical skill, decision support, communication, or provider referral.
- Evaluate whether information interventions reach low-literacy, low-resource, or time-constrained caregivers rather than only motivated participants.
- Use curated sources, citation traceability, and review workflows when adapting health information with AI.
- Reduce text overload through progressive disclosure, visuals, audio options, and navigation aids when caregivers are under cognitive and time burden.

## Gaps

- The abstract does not evaluate RAG or LLM-generated education in deployment.

## Related Pages

- `wiki/populations/family_caregivers.md`
- `wiki/design_patterns/trajectory_sensitive_caregiver_content.md`
- `wiki/technologies/ai_driven_digital_health.md`
