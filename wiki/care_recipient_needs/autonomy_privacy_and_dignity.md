---
title: Autonomy, Privacy, and Dignity
type: care_recipient_need
status: draft
privacy: private
evidence_status: has_sources
tags: [autonomy, privacy, dignity, care-recipient]
last_updated: 2026-08-06
---

# Autonomy, Privacy, and Dignity

## Need Summary

Care recipient autonomy, privacy, and dignity should be tracked separately from caregiver convenience or monitoring needs.

## Design Tension

Technologies that reduce caregiver uncertainty may increase surveillance, reduce autonomy, or create privacy concerns for the care recipient.

AI systems that offer preparation, messaging, or advocacy support may increase care-recipient agency, but can also pressure users to disclose sensitive health records or accept outputs that appear clinically authoritative.

## Evidence

- `2026-05-18_hu_chatgpt-health-sci-preclinic-preparation`: An SCI pre-clinic preparation abstract notes that care recipients may be reluctant to link sensitive EHR or wearable data to a commercial AI platform. The source evaluates use without connected records and frames AI support around preparation and advocacy rather than autonomous clinical decision-making.
- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: The dissertation identifies balancing security and multiple-user access as a caregiver app design issue. Shared access and monitoring features should preserve care recipient privacy, consent, role boundaries, and autonomy.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: iMHere 2.0 uses caregiver roles, clinician portal support, secure two-way communication, real-time synchronization, temporary local storage for most modules, and network-only personal health record handling to manage self-management support and data access.
- `2016_nasem_families-caring-for-an-aging-america`: Person- and family-centered care should recognize caregivers as partners while still respecting care-recipient autonomy and privacy; HIPAA misunderstanding and individual-coverage models can complicate caregiver engagement.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Caregiver interventions may affect care-recipient outcomes including psychological health, physical health, disease management, utilization, and economic status, so care-recipient effects should be measured separately.
- `2020_schulz_family-caregiving-for-older-adults`: Monitoring, advocacy, surrogacy, and care coordination can support care recipients but can also interact with relationship quality, care-recipient suffering, and safety concerns.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG-style systems require careful control over what user data are indexed, retrieved, logged, and exposed as provenance.
- `2023_yao_react-reasoning-acting-language-models`: ReAct-style systems raise privacy and safety concerns when language models can look up information or take actions in external environments.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes GPS monitoring, chatbot records, provider messaging, shared caregiver access, cloud storage, and source-reported de-identification/delinking/privacy controls, making consent and role boundaries central.
- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: A multi-agent conversational AI intended for both persons with Alzheimer's disease and caregivers should preserve care-recipient autonomy when task support and medical inquiries are included.
- `2010_gitlin_cope-dementia-home-based-intervention`: COPE supports capability-aligned activity engagement and task simplification for people with dementia, but many outcomes relied on caregiver proxy reports and should not be treated as direct care-recipient subjective experience.
- `2003_hepburn_savvy-caregiver-transportable-program`: Savvy Caregiver's dementia-specific role training includes taking control as dementia erodes autonomy; wiki use should pair this with dignity, consent, and decision-capacity cautions.
- `2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis`: Care-recipient symptoms and institutionalization should be measured separately from caregiver outcomes when evaluating caregiver interventions.
- `2021_ruggiano_chatbots-dementia-caregivers`: Dementia chatbots and voice assistants raise privacy, safety, trustworthiness, evidence-source, disclaimer, accessibility, and escalation concerns for people with dementia and caregivers.
- `2020_bressan_dementia-caregiver-needs-mixed-method-review`: Dementia caregiver training and information needs include safety and dignity, but caregiver needs should not be collapsed into care-recipient autonomy or preference.
- `2008_elliott_problem-solving-videoconferencing-sci-caregivers`: Care recipients of SCI caregivers receiving PST reported social-functioning gains, supporting separate measurement of care-recipient outcomes when caregiver interventions are evaluated. This should not be treated as direct evidence of care-recipient preference or autonomy.
- `2022_espino_coping-social-support-caregiver-wellbeing-sci`: SCI dyads discussed care-recipient independence, adaptive coping, and shared future care planning. Use this as dyadic planning evidence, not as justification for caregiver override, surveillance, or collapsing care-recipient autonomy into caregiver support.
- `2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs`: Gynecologic cancer patients and caregivers wanted private spaces and control over what information is shared with the other dyad member and other family members. Dyadic apps should preserve both patient and caregiver autonomy.
- `2026-06-16_chen_generative-ai-meaning-centered-care-later-life`: GenAI-supported life review and meaning-centered care should preserve user agency, distinguish user words from AI-generated text, avoid false memories, support user control over sharing, and keep human review and escalation pathways explicit.
- `2026-06-24_zhai_smart-home-technologies-ageing-in-place`: Smart-home monitoring for aging in place can support safety and independence but raises privacy, surveillance, consent, and household data-governance concerns that should be separated from caregiver reassurance.
- `2026-07-23_fritz_community-in-the-loop-smart-home-monitoring`: Some withdrawals and qualitative findings involved privacy, invasiveness, confusion, and trust, supporting digital-distress assessment and meaningful monitoring choice.
- `2026-07-15_pemberton_smart-home-connected-care-adoption`: Shared adoption and caregiver-mediated use support granular permissions, transparent logs, and role clarity rather than blanket family access.
- `2026-07-31_richter_llm-physician-patient-communication-review`: Perceived empathy should not be used to override informed choice or conceal uncertainty, incorrect content, or unclear authorship.

## Design Implications

- Do not index or retrieve sensitive care-recipient data without explicit consent and a retention policy.
- Keep AI action spaces permissioned and auditable.
- Require human confirmation before sharing information, sending messages, changing access, or acting on behalf of a care recipient.
- Preserve care-recipient control over what is summarized, disclosed, or delegated to caregivers.
- Treat GPS location, chatbot conversation history, care plans, and provider messages as sensitive data with explicit access and retention rules.
- For dementia caregiver interventions, distinguish caregiver confidence or proxy-rated improvement from care-recipient autonomy, preference, and lived experience.
- For dementia chatbots, do not assume that ease of use for a caregiver or successful command completion means the person with dementia understands, consents to, or benefits from the interaction.
- For SCI caregiver systems, support shared future planning and care-recipient independence while preserving separate consent, autonomy, and preference fields.
- For gynecologic cancer dyadic apps, support patient-only, caregiver-only, dyadic, and family-sharing modes with explicit consent, granular permissions, and revocable access.
- For GenAI narrative support, preserve provenance of personal words, allow users to review or delete summaries, and require explicit consent before sharing biographical material with family, caregivers, clinicians, or community workers.
- For smart-home systems, treat passive sensing, location, activity, sleep, and inferred behavior data as sensitive care-recipient and household data, not merely caregiver convenience data.
- Make monitoring purpose, access, retention, revocation, pause controls, non-alert meaning, and response responsibility understandable and revisable.
- Preserve provenance so users can distinguish their own words, clinician communication, caregiver input, and AI-generated text.

## Related Pages

- `wiki/concepts/digital_distress.md`
- `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`
