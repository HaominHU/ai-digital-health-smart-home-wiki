---
title: AI Digital Health and Smart Home Wiki Index
type: index
status: draft
privacy: private
last_updated: 2026-05-27
---

# AI Digital Health and Smart Home Wiki Index

## Project Overview

This repo is a private research wiki for AI-driven digital health and smart home technologies in caregiving, chronic conditions, disability, and aging.

The wiki is designed as a Markdown knowledge middleware layer: readable by humans, maintainable by AI agents, compatible with Obsidian, and structured enough for future vector DB or RAG use.

## Root-Level Control Files

- `AGENTS.md`: Agent operating rules, privacy boundaries, source rules, and wiki conventions.
- `CLAUDE.md`: Claude-compatible pointer to `AGENTS.md`.
- `README.md`: Project overview and usage summary.
- `INDEX.md`: Content-oriented wiki map.
- `LOG.md`: Chronological append-only project log.
- `MEMORY.md`: Compressed current-state digest.

## Raw Source Layer

- `sources/papers/`: Published papers and paper notes.
- `sources/reports/`: Reports, dissertations, white papers, and formal documents.
- `sources/abstracts/`: Abstracts and short publication records.
- `sources/conference_notes/`: Conference notes and session takeaways.
- `sources/presentation_notes/`: Notes from talks, seminars, and presentations.
- `sources/documentation/`: Technical, policy, or product documentation.
- `sources/personal_notes/`: User-provided quick notes and research ideas.
- `sources/attachments/`: Attachments associated with source records.

Raw sources should be treated as immutable.

## Wiki Layer

- `wiki/overview/`: Project overview and domain maps.
- `wiki/populations/`: Population pages.
- `wiki/conditions/`: Condition overlay pages.
- `wiki/caregiving_challenges/`: Reusable caregiver challenge hubs.
- `wiki/care_recipient_needs/`: Care recipient needs tracked separately from caregiver needs.
- `wiki/technologies/`: Technology lens pages.
- `wiki/environments/`: Home, clinic, community, and hybrid care contexts.
- `wiki/concepts/`: Cross-cutting conceptual distinctions.
- `wiki/evidence/`: Evidence summaries and source-backed synthesis.
- `wiki/design_patterns/`: Reusable intervention and system design patterns.
- `wiki/research_questions/`: Research gaps, open questions, and study ideas.
- `wiki/specs/`: Research, design, and system specification pages.
- `wiki/references/`: Knowledge-level citation memory and reference item records for Zotero/EndNote-ready export workflows.
- `wiki/workflows/`: Repeatable maintenance workflows.
- `wiki/commands/`: Short command templates for Codex.
- `wiki/templates/`: Reusable page templates.

## Source-Backed Evidence Pages

- `wiki/evidence/hcd_generative_ai_family_caregiver_mhealth.md`
- `wiki/evidence/raynaud_mhealth_usability_systemic_sclerosis.md`
- `wiki/evidence/chatgpt_health_sci_preclinic_preparation.md`
- `wiki/evidence/dissertation_family_caregiver_mhealth_app.md`
- `wiki/evidence/setiawan_2019_adaptive_mhealth_self_management.md`
- `wiki/evidence/schulz_2020_family_caregiving_older_adults.md`
- `wiki/evidence/nasem_2016_families_caring_aging_america.md`
- `wiki/evidence/van_houtven_2011_caregiver_intervention_framework.md`
- `wiki/evidence/mohammed_2023_sci_family_caregiver_experiences_ghana.md`
- `wiki/evidence/hartnett_2016_caregiver_burden_end_stage_ovarian_cancer.md`
- `wiki/evidence/glasgow_2001_reaim_chronic_illness_management.md`
- `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`
- `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`

## Citation Memory

- `wiki/references/README.md`: Citation-memory policy and Zotero/EndNote export boundary.
- `wiki/references/items/2019-04-25_setiawan_adaptive-mhealth-self-management.md`
- `wiki/references/items/2020_schulz_family-caregiving-for-older-adults.md`
- `wiki/references/items/2016_nasem_families-caring-for-an-aging-america.md`
- `wiki/references/items/2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions.md`
- `wiki/references/items/2023-04-21_mohammed_sci-family-caregiver-experiences-ghana.md`
- `wiki/references/items/2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer.md`
- `wiki/references/items/2001_glasgow_re-aim-framework-chronic-illness-management.md`
- `wiki/references/items/2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp.md`
- `wiki/references/items/2023_yao_react-reasoning-acting-language-models.md`

## Templates

- `wiki/templates/reference_item_template.md`
- `wiki/templates/citation_supported_brainstorming_output_template.md`

## Outputs

- `outputs/ingest_previews/`: Human-review previews before major source integration.
- `outputs/evidence_briefs/`: Evidence summaries generated from the wiki.
- `outputs/research_prompts/`: AI-ready research and writing prompts.
- `outputs/design_prompts/`: AI-ready design prompts.
- `outputs/spec_prompts/`: AI-ready system or study specification prompts.
- `outputs/query_answers/`: Durable answers worth preserving outside chat.
- `outputs/lint_reports/`: Wiki health-check reports.
- `outputs/citation_exports/`: Generated Zotero/EndNote-compatible citation exports, usually RIS.

## Privacy-Sensitive Space

- `private_notes/`: Sensitive scratch space and private working notes.

Do not store identifiable participant data, PHI, clinical records, or raw sensitive study material unless the user explicitly provides a safe handling policy.

## Initial Conceptual Pages

- `wiki/overview/domain_map.md`: Overall research domain map.
- `wiki/concepts/aging_vs_disease.md`: Distinguishes aging-related decline from disease and disability.
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`: Separates caregiver needs from care recipient needs.
- `wiki/concepts/multimorbidity_and_overlapping_needs.md`: Tracks overlapping needs and interacting causes.
- `wiki/concepts/caregiving_as_chronic_stress_exposure.md`: Frames caregiving as potential chronic stress exposure while preserving variation and positive caregiving meanings.
- `wiki/concepts/caregiving_activities_vs_outcomes.md`: Separates caregiving activities from caregiver and care-recipient outcomes.
- `wiki/concepts/reach_adoption_implementation_maintenance.md`: Uses RE-AIM to track reach, efficacy, adoption, implementation, and maintenance for intervention evaluation.

## Initial Population Pages

- `wiki/populations/family_caregivers.md`
- `wiki/populations/older_adults.md`
- `wiki/populations/people_with_chronic_conditions_and_disabilities.md`

## Initial Condition Pages

- `wiki/conditions/spinal_cord_injury.md`
- `wiki/conditions/dementia.md`
- `wiki/conditions/falls_and_aging.md`
- `wiki/conditions/multiple_chronic_conditions_in_aging.md`
- `wiki/conditions/systemic_sclerosis_associated_raynaud_phenomenon.md`
- `wiki/conditions/postpartum_women.md`
- `wiki/conditions/gynecological_cancer.md`

## Caregiving Challenge Hubs

- `wiki/caregiving_challenges/monitoring_and_safety_awareness.md`
- `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`
- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/caregiving_challenges/emotional_and_social_support.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`

## Care Recipient Need Pages

- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/care_recipient_needs/symptom_self_reporting_and_tracking.md`
- `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`
- `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`

## Design Pattern Pages

- `wiki/design_patterns/adaptive_ai_layer_for_caregiver_mhealth.md`
- `wiki/design_patterns/trajectory_sensitive_caregiver_content.md`
- `wiki/design_patterns/accessibility_first_mhealth_symptom_reporting.md`
- `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`
- `wiki/design_patterns/ai_assisted_pre_clinic_preparation.md`
- `wiki/design_patterns/care_recipient_style_prompting_for_empathy.md`
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`
- `wiki/design_patterns/one_stop_caregiver_support_app.md`
- `wiki/design_patterns/ai_and_wearable_augmented_caregiver_support.md`
- `wiki/design_patterns/adaptive_mhealth_self_management_platform.md`
- `wiki/design_patterns/clinician_portal_supported_mhealth.md`
- `wiki/design_patterns/caregiver_assessment_and_triage.md`
- `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`
- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`

## Research Question Pages

- `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`

## Initial Technology Pages

- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/technologies/smart_home_technologies.md`

## Workflows

- `wiki/workflows/ingest_source.md`
- `wiki/workflows/query_wiki.md`
- `wiki/workflows/lint_wiki.md`
- `wiki/workflows/generate_research_prompt.md`
- `wiki/workflows/generate_design_spec_prompt.md`
- `wiki/workflows/citation_supported_brainstorming.md`

## Command Templates

- `wiki/commands/README.md`
- `wiki/commands/ingest_source.md`
- `wiki/commands/quick_note.md`
- `wiki/commands/ask_wiki.md`
- `wiki/commands/lint_wiki.md`
- `wiki/commands/generate_research_prompt.md`
- `wiki/commands/generate_design_spec_prompt.md`
- `wiki/commands/citation_supported_brainstorming.md`
