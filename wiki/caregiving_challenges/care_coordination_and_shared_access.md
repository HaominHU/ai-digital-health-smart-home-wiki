---
title: Care Coordination and Shared Access
type: caregiving_challenge
status: draft
privacy: private
evidence_status: has_sources
tags: [care-coordination, shared-access, caregiving, privacy]
last_updated: 2026-06-02
---

# Care Coordination and Shared Access

## Challenge Summary

Reusable caregiving challenge hub for coordinating care tasks, sharing information across caregivers or providers, and managing role-appropriate access to care information.

## Relevant Populations

- Family caregivers of people with chronic conditions and disabilities.

## Relevant Conditions

- Cross-condition challenge.
- Spinal cord injury.
- Gynecological cancer.

## Caregiver Need

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: Focus group feedback identified care coordination, monitoring data, customized reminders, and balancing security with multiple user access as design criteria for a caregiver app.
- `2016_nasem_families-caring-for-an-aging-america`: Family caregivers often navigate health care and LTSS, communicate with many provider types, provide health-history information, and may be expected to implement care plans while being excluded from planning or training.
- `2020_schulz_family-caregiving-for-older-adults`: Caregiver roles include advocacy, care coordination, provider communication, and surrogacy across cumulative care trajectories.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`: Support-seeking skills include organizational, tactical, recruiting, provider coordination, and resource-navigation skills.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregivers in Ghana reported instrumental roles including transportation, cooking, errands, housekeeping, managing finances, and managing care-recipient business or money.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`: The oncology nursing article recommends interdisciplinary support, including nursing education, social work, financial and medication assistance, community organization referrals, support groups, and respite.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`: Telehealth can provide an avenue for caregivers to discuss support needs between scheduled health care visits.
- `2023_zhai_digital-health-interventions-support-family-caregivers`: Digital health interventions can support interactive communication and caregiver-care recipient relationships, but shared access and communication functions still require privacy and role-boundary design.
- `2023_yao_react-reasoning-acting-language-models`: ReAct provides technical rationale for stepwise tool use and inspectable action traces, but it should only inform speculative coordination support under strict action-space limits.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes care planning, centralized provider messaging, QR code multi-caregiver coordination, telemedicine links, care center transfer workflows, provider interface, and moderator interface for dementia caregiver support.
- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`: The abstract reports specialized agents for appointment scheduling and reminders, coordinated by a central orchestrator.
- `2017_nichols_reach-dementia-caregiver-healthcare-costs`: REACH VA suggests that structured caregiver role support embedded in an integrated care system may be associated with lower care-recipient VA costs.
- `2010_gitlin_cope-dementia-home-based-intervention`: COPE links caregiver training with patient medical review, home assessment, and physician follow-up for undiagnosed conditions.
- `2003_hepburn_savvy-caregiver-transportable-program`: Savvy Caregiver supports community-adoptable caregiver training, but implementation requires facilitator preparation and organizational support.

## Care Recipient Connection

Shared access can help caregivers coordinate support, but it can also create privacy, autonomy, consent, and surveillance concerns for care recipients.

## Technology Support Lens

- Centralized notes, schedules, medication lists, resource libraries, reminders, and role-based access controls.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`: The caregiver app supports monitoring, positive reinforcement, schedule setup, and caregiver role concepts, while the clinician portal supports module selection, regimen adjustment, messaging, and care-team management.
- `2016_nasem_families-caring-for-an-aging-america`: Shared access and caregiver engagement should be designed as person- and family-centered care, preserving care-recipient autonomy, privacy, and consent.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: RAG can support source-grounded resource lookup or coordination drafts when sources are curated.
- `2023_yao_react-reasoning-acting-language-models`: ReAct can support draft task orchestration, but external communication, purchases, care-plan changes, or device actions should require human confirmation.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy is a concrete provider-connected caregiver mHealth example, but the study reports usability/acceptability rather than coordination outcome effectiveness.

## Evidence

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`.
- `2019-04-25_setiawan_adaptive-mhealth-self-management`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2020_schulz_family-caregiving-for-older-adults`.
- `2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions`.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`.
- `2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer`.
- `2021_graven_telehealth-interventions-family-caregivers-chronic-conditions`.
- `2023_zhai_digital-health-interventions-support-family-caregivers`.
- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`.
- `2023_yao_react-reasoning-acting-language-models`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.
- `2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers`.
- `2017_nichols_reach-dementia-caregiver-healthcare-costs`.
- `2010_gitlin_cope-dementia-home-based-intervention`.
- `2003_hepburn_savvy-caregiver-transportable-program`.

## Design Implications

- Define who can view, edit, share, or act on different information.
- Separate caregiver convenience from care recipient consent and dignity.
- Include auditability and revocable access when designing shared caregiver systems.
- Assess caregiver capacity and willingness before assigning coordination tasks.
- For AI-assisted coordination, log retrieved sources, proposed actions, confirmations, and any shared-access changes.
- For multi-caregiver and provider-connected workflows, make role permissions, consent, and revocation explicit.

## Gaps

- The dissertation supports design criteria and pilot usability/acceptability/feasibility, not effectiveness of shared-access models.

## Related Pages

- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/populations/family_caregivers.md`
- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/design_patterns/caregiver_assessment_and_triage.md`
