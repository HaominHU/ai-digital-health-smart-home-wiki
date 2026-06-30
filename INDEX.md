---
title: AI Digital Health and Smart Home Wiki Index
type: index
status: draft
privacy: private
last_updated: 2026-06-30
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

- `sources/papers/`: Published papers and paper notes. Purpose-specific paper lanes can be added under this folder as new source groups emerge.
- `sources/papers/cg_system_core/`: Example lane for the ongoing numbered key citation set for caregiver system-design evidence ingest. Use `wiki/references/cg_system_core_reference_plan.md` as the live status map for integrated, planned, skipped, future, and background-only sources.
- `sources/papers/monthly_pubmed/`: Example lane for flat monthly PubMed push storage before triage, selection, preview, or integration. Add another hierarchy later only if volume or workflow needs justify it.
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

## Overview and Synthesis Pages

- `wiki/overview/domain_map.md`: Top-level architecture, knowledge ownership, and routing page for the whole wiki.
- `wiki/overview/caregiver_system_core_sota_synthesis.md`: Living owner-facing SoTA synthesis for the current integrated `cg_system_core` evidence, summarizing family caregiving outcomes, digital health intervention types/mechanisms/modalities, condition-specific dementia/SCI/gynecological cancer details, evidence boundaries, and research directions to keep current after future ingests.

## Source-Backed Evidence Pages

- `wiki/evidence/hcd_generative_ai_family_caregiver_mhealth.md`
- `wiki/evidence/raynaud_mhealth_usability_systemic_sclerosis.md`
- `wiki/evidence/chatgpt_health_sci_preclinic_preparation.md`
- `wiki/evidence/dissertation_family_caregiver_mhealth_app.md`
- `wiki/evidence/setiawan_2019_adaptive_mhealth_self_management.md`
- `wiki/evidence/aneshensel_avison_2015_stress_process_appreciation_pearlin.md`
- `wiki/evidence/schulz_sherwood_2008_physical_mental_health_effects_family_caregiving.md`
- `wiki/evidence/graven_2021_telehealth_interventions_family_caregivers_chronic_conditions.md`
- `wiki/evidence/zhai_2023_digital_health_interventions_support_family_caregivers.md`
- `wiki/evidence/schulz_2020_family_caregiving_older_adults.md`
- `wiki/evidence/nasem_2016_families_caring_aging_america.md`
- `wiki/evidence/van_houtven_2011_caregiver_intervention_framework.md`
- `wiki/evidence/mohammed_2023_sci_family_caregiver_experiences_ghana.md`
- `wiki/evidence/hartnett_2016_caregiver_burden_end_stage_ovarian_cancer.md`
- `wiki/evidence/glasgow_2001_reaim_chronic_illness_management.md`
- `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`
- `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`
- `wiki/evidence/hasan_2025_carebuddy_multi_agent_conversational_ai_alzheimers.md`
- `wiki/evidence/malhotra_2025_carebuddy_mobile_care_ecosystem_dementia_caregiving.md`
- `wiki/evidence/nichols_2017_reach_dementia_caregiver_healthcare_costs.md`
- `wiki/evidence/gitlin_2010_cope_dementia_home_based_intervention.md`
- `wiki/evidence/hepburn_2003_savvy_caregiver_transportable_program.md`
- `wiki/evidence/hepburn_2022_telesavvy_online_dementia_caregiver_program.md`
- `wiki/evidence/walter_pinquart_2020_dementia_caregiver_interventions_meta_analysis.md`
- `wiki/evidence/cheng_2020_meta_review_dementia_caregiver_interventions.md`
- `wiki/evidence/bressan_2020_dementia_caregiver_needs_mixed_method_review.md`
- `wiki/evidence/ruggiano_2021_chatbots_dementia_caregivers.md`
- `wiki/evidence/elliott_2008_problem_solving_videoconferencing_sci_caregivers.md`
- `wiki/evidence/elliott_2009_brief_problem_solving_training_sci_caregivers.md`
- `wiki/evidence/smith_2016_caregiving_services_sci_systematic_review.md`
- `wiki/evidence/conti_2019_secondary_conditions_caregiver_burden_sci.md`
- `wiki/evidence/espino_2022_coping_social_support_caregiver_wellbeing_sci.md`
- `wiki/evidence/ugalde_2019_cancer_caregiver_interventions_implementation_potential.md`
- `wiki/evidence/becque_2023_supportive_interventions_advanced_cancer_caregivers.md`
- `wiki/evidence/campbell_2024_gynecologic_cancer_caregiver_mhealth_self_management_needs.md`
- `wiki/evidence/dave_2024_cancer_caregiver_needs_patient_advocacy_groups.md`
- `wiki/evidence/koroshetz_2026_neuroscience_takeaways_sci_translation.md`
- `wiki/evidence/fridriksson_2026_brain_health_aphasia_recovery.md`
- `wiki/evidence/kingsada_2026_preferences_digital_health_technologies.md`

## Citation Memory

- `wiki/references/README.md`: Citation-memory policy and Zotero/EndNote export boundary.
- `wiki/references/cg_system_core_reference_plan.md`: Planning-only map for the caregiver system core reference backbone, staged ingest batches, source roles, and deferred/skipped sources.
- `wiki/references/items/2019-04-25_setiawan_adaptive-mhealth-self-management.md`
- `wiki/references/items/2015_aneshensel-avison_stress-process-appreciation-pearlin.md`
- `wiki/references/items/2008_schulz-sherwood_physical-mental-health-effects-family-caregiving.md`
- `wiki/references/items/2021_graven_telehealth-interventions-family-caregivers-chronic-conditions.md`
- `wiki/references/items/2023_zhai_digital-health-interventions-support-family-caregivers.md`
- `wiki/references/items/2020_schulz_family-caregiving-for-older-adults.md`
- `wiki/references/items/2016_nasem_families-caring-for-an-aging-america.md`
- `wiki/references/items/2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions.md`
- `wiki/references/items/2023-04-21_mohammed_sci-family-caregiver-experiences-ghana.md`
- `wiki/references/items/2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer.md`
- `wiki/references/items/2001_glasgow_re-aim-framework-chronic-illness-management.md`
- `wiki/references/items/2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp.md`
- `wiki/references/items/2023_yao_react-reasoning-acting-language-models.md`
- `wiki/references/items/2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers.md`
- `wiki/references/items/2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving.md`
- `wiki/references/items/2017_nichols_reach-dementia-caregiver-healthcare-costs.md`
- `wiki/references/items/2010_gitlin_cope-dementia-home-based-intervention.md`
- `wiki/references/items/2003_hepburn_savvy-caregiver-transportable-program.md`
- `wiki/references/items/2022_hepburn_telesavvy-online-dementia-caregiver-program.md`
- `wiki/references/items/2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis.md`
- `wiki/references/items/2020_cheng_meta-review-dementia-caregiver-interventions.md`
- `wiki/references/items/2020_bressan_dementia-caregiver-needs-mixed-method-review.md`
- `wiki/references/items/2021_ruggiano_chatbots-dementia-caregivers.md`
- `wiki/references/items/2008_elliott_problem-solving-videoconferencing-sci-caregivers.md`
- `wiki/references/items/2009_elliott_brief-problem-solving-training-sci-caregivers.md`
- `wiki/references/items/2016_smith_caregiving-services-sci-systematic-review.md`
- `wiki/references/items/2019_conti_secondary-conditions-caregiver-burden-sci.md`
- `wiki/references/items/2022_espino_coping-social-support-caregiver-wellbeing-sci.md`
- `wiki/references/items/2019_ugalde_cancer-caregiver-interventions-implementation-potential.md`
- `wiki/references/items/2023_becque_supportive-interventions-family-caregivers-advanced-cancer.md`
- `wiki/references/items/2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs.md`
- `wiki/references/items/2024_dave_cancer-caregiver-needs-patient-advocacy-groups.md`
- `wiki/references/items/2026_kingsada_preferences-digital-health-technologies.md`

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
- `outputs/lint_reports/2026-06-17_wiki_structure_knowledge_workflow_check.md`: Structure, knowledge, logic, and workflow check that updated the domain map and added living overview/synthesis maintenance guardrails.
- `outputs/lint_reports/2026-06-17_deep_overview_conflict_compliance_check.md`: Deep overview and knowledge-conflict compliance scan focused on old workflow contamination.
- `outputs/citation_exports/`: Generated Zotero/EndNote-compatible citation exports, usually RIS.

## Privacy-Sensitive Space

- `private_notes/`: Sensitive scratch space and private working notes.

Do not store identifiable participant data, PHI, clinical records, or raw sensitive study material unless the user explicitly provides a safe handling policy.

## Core Concept Pages

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
- `wiki/design_patterns/biomarker_stratified_neurorehabilitation.md`

## Research Question Pages

- `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`
- `wiki/research_questions/biomarker_stratified_neurorehabilitation.md`

## Initial Technology Pages

- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/technologies/smart_home_technologies.md`

## Environment Pages

- `wiki/environments/home.md`

## Workflows

- `wiki/workflows/ingest_source.md`
- `wiki/workflows/query_wiki.md`
- `wiki/workflows/lint_wiki.md`: Default `health check`; Karpathy-style wiki knowledge lint for contradictions, stale claims, structural gaps, knowledge gaps, source tracking, privacy, and conceptual consistency.
- `wiki/workflows/repo_health_check.md`: `repo health check`; repository/worktree/git hygiene before asking whether to commit and push.
- `wiki/workflows/generate_research_prompt.md`
- `wiki/workflows/generate_design_spec_prompt.md`
- `wiki/workflows/citation_supported_brainstorming.md`

## Command Templates

- `wiki/commands/README.md`
- `wiki/commands/ingest_source.md`
- `wiki/commands/quick_note.md`
- `wiki/commands/ask_wiki.md`
- `wiki/commands/lint_wiki.md`: Default `health check`.
- `wiki/commands/repo_health_check.md`: `repo health check`.
- `wiki/commands/generate_research_prompt.md`
- `wiki/commands/generate_design_spec_prompt.md`
- `wiki/commands/citation_supported_brainstorming.md`
