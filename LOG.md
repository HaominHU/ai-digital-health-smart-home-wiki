# LOG.md

Chronological project log for the AI Digital Health and Smart Home Research Wiki.

Use this as the Karpathy-style append-only timeline of meaningful ingests, queries, lint checks, architecture changes, workflow updates, generated outputs, and memory updates.

Entry format:

```text
## [YYYY-MM-DD] type | Short title

- Summary: One or two lines.
- Files touched: `path`, `path`.
- Notes: Optional.
```

Recommended types:

- `ingest`: Source-backed knowledge integrated into the wiki.
- `query`: A meaningful wiki query or synthesis whose result should be preserved.
- `lint`: Wiki health check, privacy check, source-support check, or conceptual consistency check.
- `architecture`: Folder structure, schema, or project design change.
- `workflow`: Workflow file or operating-rule update.
- `output`: Generated artifact such as a preview, brief, prompt, or report.
- `prompt`: AI-ready research, design, or spec prompt generation.
- `memory`: Compressed state update in `MEMORY.md`.

Logging rule: if the work changes wiki source content, generated outputs, architecture, workflow state, or project memory, append a `LOG.md` entry in the same turn.

## [2026-05-18] architecture | Initialized research wiki scaffold

- Summary: Created the initial Karpathy-style research wiki structure for AI-driven digital health and smart home technologies, including raw source, wiki, output, and private note folders.
- Files touched: `AGENTS.md`, `README.md`, `INDEX.md`, `LOG.md`, `MEMORY.md`, `sources/`, `wiki/`, `outputs/`, `private_notes/`.
- Notes: Established privacy-sensitive healthcare handling, clinical decision boundaries, source tracking, and Obsidian-compatible Markdown conventions.

## [2026-05-18] workflow | Defined local raw source storage policy

- Summary: Added local-only raw source storage defaults, gitignore rules, source filename conventions, and lint reminders for source retention review.
- Files touched: `.gitignore`, `sources/README.md`, `private_notes/README.md`, `AGENTS.md`, `README.md`, `MEMORY.md`, `wiki/workflows/ingest_source.md`, `wiki/workflows/lint_wiki.md`, `LOG.md`.
- Notes: User will manually handle commits and git management. Raw sources are ignored by git by default and should not be deleted automatically.

## [2026-05-18] workflow | Simplified README usage instructions

- Summary: Revised `README.md` to match the restaurant wiki's icon-led format and replaced AI-facing reproduction steps with user-facing prompt examples for ingest, quick notes, queries, prompt generation, and linting.
- Files touched: `README.md`, `sources/README.md`, `LOG.md`.
- Notes: Clarified that command files are reusable instruction recipes, not terminal commands, and that Codex can copy local files into `sources/` when asked.

## [2026-05-18] architecture | Expanded condition priority list

- Summary: Added systemic sclerosis-associated Raynaud phenomenon and postpartum women as priority condition/context overlays before gynecological cancer.
- Files touched: `AGENTS.md`, `README.md`, `INDEX.md`, `MEMORY.md`, `wiki/overview/domain_map.md`, `wiki/conditions/systemic_sclerosis_associated_raynaud_phenomenon.md`, `wiki/conditions/postpartum_women.md`, `LOG.md`.
- Notes: New condition pages are scaffold entries only and contain no source-backed claims yet.

## [2026-05-18] ingest | Human-centered design recommendations for generative AI in caregiver mHealth

- Summary: Created an ingest preview for an AMIA abstract on human-centered design recommendations for generative AI in mHealth apps for family caregivers.
- Files touched: `sources/abstracts/Hu_podium_abstract_User_centered_design_family_caregiver_AI_vision_submit.pdf`, `outputs/ingest_previews/2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth_preview.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user; review status is pending before wiki integration.

## [2026-05-18] ingest | Integrated generative AI caregiver mHealth abstract

- Summary: Integrated the approved AMIA abstract preview into population, condition, technology, caregiving challenge, design pattern, and evidence pages.
- Files touched: `outputs/ingest_previews/2026-05-18_hu_hcd-generative-ai-family-caregiver-mhealth_preview.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/emotional_and_social_support.md`, `wiki/design_patterns/adaptive_ai_layer_for_caregiver_mhealth.md`, `wiki/design_patterns/trajectory_sensitive_caregiver_content.md`, `wiki/evidence/hcd_generative_ai_family_caregiver_mhealth.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user. Broad neurological-condition evidence was mapped cautiously to spinal cord injury only where no specific non-SCI neurological condition was named.

## [2026-05-18] ingest | Raynaud mHealth app usability preview

- Summary: Created an ingest preview for an AMIA abstract on usability evaluation and iterative refinement of a Raynaud's phenomenon mHealth app for people with systemic sclerosis.
- Files touched: `sources/abstracts/202605_AMIA_Hu_Raynaud_Usability_resubmit_poster.pdf`, `outputs/ingest_previews/2026-05-18_hu_raynaud-phenomenon-mhealth-usability_preview.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user; review status is pending before wiki integration.

## [2026-05-18] ingest | Integrated Raynaud mHealth app usability abstract

- Summary: Integrated the approved AMIA abstract preview into the systemic sclerosis-associated Raynaud phenomenon condition page, chronic condition/disability and older-adult population pages, care-recipient symptom tracking, design patterns, and evidence pages.
- Files touched: `outputs/ingest_previews/2026-05-18_hu_raynaud-phenomenon-mhealth-usability_preview.md`, `wiki/conditions/systemic_sclerosis_associated_raynaud_phenomenon.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/populations/older_adults.md`, `wiki/care_recipient_needs/symptom_self_reporting_and_tracking.md`, `wiki/design_patterns/accessibility_first_mhealth_symptom_reporting.md`, `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`, `wiki/evidence/raynaud_mhealth_usability_systemic_sclerosis.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user. Older-adult relevance is limited to accessibility/usability barriers and is not treated as aging-related disease evidence.

## [2026-05-18] ingest | ChatGPT Health SCI pre-clinic preparation preview

- Summary: Created an ingest preview for an AMIA abstract comparing ChatGPT and a source-reported ChatGPT Health interface for spinal cord injury pre-clinic preparation without connected records.
- Files touched: `sources/abstracts/Hu_poster_abstract_ChatGPT_ChatGPTHealth_Comparison_submit.pdf`, `outputs/ingest_previews/2026-05-18_hu_chatgpt-health-sci-preclinic-preparation_preview.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user; review status is pending before wiki integration. Product/model details are source-reported and not independently verified during ingest.

## [2026-05-18] ingest | Integrated ChatGPT Health SCI pre-clinic preparation abstract

- Summary: Integrated the approved AMIA abstract preview into the spinal cord injury condition page, AI-driven digital health technology page, care-recipient privacy/autonomy page, pre-clinic preparation hub, design patterns, and evidence page.
- Files touched: `outputs/ingest_previews/2026-05-18_hu_chatgpt-health-sci-preclinic-preparation_preview.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`, `wiki/design_patterns/ai_assisted_pre_clinic_preparation.md`, `wiki/design_patterns/care_recipient_style_prompting_for_empathy.md`, `wiki/evidence/chatgpt_health_sci_preclinic_preparation.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is AMIA conference submission abstract; evidence type is conference takeaway; privacy level is private/non-sensitive per user. Product/model details are source-reported and should be re-verified before current-state OpenAI product claims.

## [2026-05-18] ingest | Family caregiver mHealth dissertation preview

- Summary: Created an ingest preview for Hu's doctoral dissertation on developing a multi-component mHealth app for family caregivers of people with chronic conditions and disabilities.
- Files touched: `sources/papers/Hu_ETD_241205_submission.pdf`, `outputs/ingest_previews/2026-05-18_hu_dissertation-family-caregiver-mhealth-app_preview.md`, `LOG.md`.
- Notes: Source type is doctoral dissertation; evidence type is dissertation; privacy level is private/non-sensitive per user; review status is pending before wiki integration. Preview is scoped to wiki-relevant populations, technologies, SCI, and gynecological cancer; non-wiki conditions remain source-context only.

## [2026-05-18] ingest | Integrated family caregiver mHealth dissertation

- Summary: Integrated the approved dissertation preview into population, SCI, gynecological cancer, technology, caregiving challenge, care-recipient privacy, design pattern, and evidence pages.
- Files touched: `outputs/ingest_previews/2026-05-18_hu_dissertation-family-caregiver-mhealth-app_preview.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/technologies/smart_home_technologies.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/emotional_and_social_support.md`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `wiki/design_patterns/one_stop_caregiver_support_app.md`, `wiki/design_patterns/ai_and_wearable_augmented_caregiver_support.md`, `wiki/evidence/dissertation_family_caregiver_mhealth_app.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is doctoral dissertation; evidence type is dissertation; privacy level is private/non-sensitive per user. Non-wiki conditions from study composition were not added as condition overlays.

## [2026-05-18] ingest | Setiawan 2019 adaptive mHealth self-management preview

- Summary: Created an ingest preview for a JMIR Formative Research paper on iMHere 2.0, an adaptive mHealth system for self-management among people with chronic conditions and disabilities.
- Files touched: `sources/papers/Setiawan 2019_imhere.pdf`, `outputs/ingest_previews/2026-05-18_setiawan_2019_adaptive-mhealth-self-management_preview.md`, `LOG.md`.
- Notes: Source type is journal article; evidence type is published evidence; privacy level is private/non-sensitive per user; review status is pending before wiki integration. Non-wiki conditions from the paper remain source-context only.

## [2026-05-18] ingest | Integrated Setiawan 2019 adaptive mHealth self-management paper

- Summary: Integrated the approved JMIR paper preview into PwCCD, SCI, care-recipient self-management, privacy/autonomy, accessibility, reliability, adaptive mHealth, clinician portal, and shared-access pages.
- Files touched: `outputs/ingest_previews/2026-05-18_setiawan_2019_adaptive-mhealth-self-management_preview.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/care_recipient_needs/symptom_self_reporting_and_tracking.md`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/design_patterns/accessibility_first_mhealth_symptom_reporting.md`, `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`, `wiki/design_patterns/adaptive_mhealth_self_management_platform.md`, `wiki/design_patterns/clinician_portal_supported_mhealth.md`, `wiki/evidence/setiawan_2019_adaptive_mhealth_self_management.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is journal article; evidence type is published evidence; privacy level is private/non-sensitive per user. User note recorded: Setiawan 2019 and Hu's dissertation jointly ground the caregiver research, system infrastructure, and future system expansion.

## [2026-05-22] architecture | Added citation memory and Zotero/EndNote export workflow

- Summary: Added a knowledge-level citation-memory layer, RIS export convention, citation-supported brainstorming workflow, command template, output template, and one backfilled export-ready reference record for Setiawan 2019.
- Files touched: `AGENTS.md`, `README.md`, `INDEX.md`, `MEMORY.md`, `wiki/references/README.md`, `wiki/references/items/2019-04-25_setiawan_adaptive-mhealth-self-management.md`, `wiki/templates/reference_item_template.md`, `wiki/templates/source_record_template.md`, `wiki/templates/citation_supported_brainstorming_output_template.md`, `wiki/workflows/ingest_source.md`, `wiki/workflows/lint_wiki.md`, `wiki/workflows/citation_supported_brainstorming.md`, `wiki/commands/README.md`, `wiki/commands/ingest_source.md`, `wiki/commands/citation_supported_brainstorming.md`, `outputs/citation_exports/README.md`, `outputs/citation_exports/.gitkeep`, `LOG.md`.
- Notes: Existing wiki had source IDs and original citation text in evidence pages, but no dedicated citation-memory layer or Zotero/EndNote-compatible export workflow. The new default is wiki-first citation brainstorming with RIS exports only when metadata is complete; incomplete references are marked for backfill rather than guessed.

## [2026-05-22] workflow | Refined external citation seed search rules

- Summary: Updated citation-supported brainstorming to assess citation coverage quality rather than using a fixed citation-count threshold, and to separate wiki citations from searched external candidate citations in both Markdown outputs and RIS export files.
- Files touched: `AGENTS.md`, `README.md`, `MEMORY.md`, `wiki/references/README.md`, `wiki/workflows/citation_supported_brainstorming.md`, `wiki/commands/citation_supported_brainstorming.md`, `wiki/templates/citation_supported_brainstorming_output_template.md`, `outputs/citation_exports/README.md`, `LOG.md`.
- Notes: External searched citations are treated as bibliography-building candidates until reviewed or ingested. Wiki citation RIS files and external candidate RIS files should remain separate for rigor and easier Zotero/EndNote import.

## [2026-05-26] ingest | Previewed systematic caregiver ingest sources 04 to 06

- Summary: Created pending ingest previews for Schulz et al. 2020, National Academies 2016, and Van Houtven et al. 2011, plus a batch crosswalk for many-to-many citation mapping across caregiver, condition, technology, design, and evaluation fields.
- Files touched: `sources/papers/04_schulz_family_caregiving_for_older_adults_2020.pdf`, `sources/papers/05_families_caring_for_an_aging_america_2016.pdf`, `sources/papers/06_van_houtven_organizing_framework_2011.pdf`, `outputs/ingest_previews/2026-05-26_schulz_family-caregiving-for-older-adults-2020_preview.md`, `outputs/ingest_previews/2026-05-26_nasem_families-caring-for-an-aging-america-2016_preview.md`, `outputs/ingest_previews/2026-05-26_van-houtven_organizing-framework-informal-caregiver-interventions-2011_preview.md`, `outputs/ingest_previews/2026-05-26_batch-04-06_systematic-ingest-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Source types are journal review article, National Academies consensus report, and journal article; evidence types are published evidence and formal report. No PHI or identifiable participant data detected in extracted text. Citation-memory records are proposed but not created pending approval.

## [2026-05-26] ingest | Integrated systematic caregiver ingest sources 04 to 06

- Summary: Integrated Schulz et al. 2020, National Academies 2016, and Van Houtven et al. 2011 into citation memory, evidence pages, shared caregiver concepts, design patterns, population pages, condition overlays, caregiver challenge hubs, care-recipient needs, technology lenses, and the home environment page.
- Files touched: `outputs/ingest_previews/2026-05-26_schulz_family-caregiving-for-older-adults-2020_preview.md`, `outputs/ingest_previews/2026-05-26_nasem_families-caring-for-an-aging-america-2016_preview.md`, `outputs/ingest_previews/2026-05-26_van-houtven_organizing-framework-informal-caregiver-interventions-2011_preview.md`, `outputs/ingest_previews/2026-05-26_batch-04-06_systematic-ingest-crosswalk.md`, `wiki/references/items/2020_schulz_family-caregiving-for-older-adults.md`, `wiki/references/items/2016_nasem_families-caring-for-an-aging-america.md`, `wiki/references/items/2011-11-22_van-houtven_organizing-framework-informal-caregiver-interventions.md`, `wiki/evidence/schulz_2020_family_caregiving_older_adults.md`, `wiki/evidence/nasem_2016_families_caring_aging_america.md`, `wiki/evidence/van_houtven_2011_caregiver_intervention_framework.md`, `wiki/concepts/`, `wiki/design_patterns/`, `wiki/research_questions/`, `wiki/populations/`, `wiki/conditions/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/`, `wiki/technologies/`, `wiki/environments/home.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. The integration preserves many-to-many citation roles and distinguishes direct evidence from design rationale, policy rationale, and evaluation framework use.

## [2026-05-26] ingest | Mohammed 2023 SCI family caregiver experiences preview

- Summary: Created an ingest preview for a PLOS ONE qualitative study on family caregivers of people with spinal cord injury at Komfo Anokye Teaching Hospital in Ghana.
- Files touched: `sources/papers/24_mohammed_sci_family_caregiver_experiences_2023.pdf`, `outputs/ingest_previews/2026-05-26_mohammed_sci-family-caregiver-experiences-ghana-2023_preview.md`, `LOG.md`.
- Notes: Source type is journal article; evidence type is published qualitative evidence; privacy level is private/non-sensitive. Review status is pending before wiki integration. Source 27 was not previewed because the local PDF appears incomplete.

## [2026-05-26] ingest | Integrated Mohammed 2023 SCI family caregiver experiences

- Summary: Integrated the approved PLOS ONE qualitative study on family caregivers of people with spinal cord injury in Ghana into SCI, family caregiver, PwCCD, caregiver challenge, home environment, design pattern, evidence, and citation-memory pages.
- Files touched: `outputs/ingest_previews/2026-05-26_mohammed_sci-family-caregiver-experiences-ghana-2023_preview.md`, `wiki/references/items/2023-04-21_mohammed_sci-family-caregiver-experiences-ghana.md`, `wiki/evidence/mohammed_2023_sci_family_caregiver_experiences_ghana.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`, `wiki/caregiving_challenges/emotional_and_social_support.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/caregiving_challenges/monitoring_and_safety_awareness.md`, `wiki/environments/home.md`, `wiki/design_patterns/caregiver_assessment_and_triage.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready. Claims are bounded to SCI-specific qualitative evidence from a Ghanaian hospital context and are not treated as prevalence or intervention-effectiveness evidence.

## [2026-05-26] ingest | Hartnett 2016 end-stage ovarian cancer caregiver burden preview

- Summary: Created an ingest preview for a Clinical Journal of Oncology Nursing pilot study on caregiver burden among primary caregivers of patients with end-stage ovarian cancer.
- Files touched: `sources/papers/31_hartnett_caregiver_burden_end_stage_ovarian_cancer_2016.pdf`, `outputs/ingest_previews/2026-05-26_hartnett_caregiver-burden-end-stage-ovarian-cancer-2016_preview.md`, `LOG.md`.
- Notes: Source type is journal article; evidence type is published pilot study evidence; privacy level is private/non-sensitive. The updated local PDF now extracts as a full-text article. Review status is pending before wiki integration.

## [2026-05-27] ingest | Integrated Hartnett 2016 end-stage ovarian cancer caregiver burden

- Summary: Integrated the approved Clinical Journal of Oncology Nursing pilot study on caregiver burden among primary caregivers of patients with end-stage ovarian cancer into gynecological cancer, caregiver challenge, home environment, design pattern, evidence, and citation-memory pages.
- Files touched: `outputs/ingest_previews/2026-05-26_hartnett_caregiver-burden-end-stage-ovarian-cancer-2016_preview.md`, `wiki/references/items/2016-04_hartnett_caregiver-burden-end-stage-ovarian-cancer.md`, `wiki/evidence/hartnett_2016_caregiver_burden_end_stage_ovarian_cancer.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/populations/family_caregivers.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`, `wiki/caregiving_challenges/emotional_and_social_support.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/environments/home.md`, `wiki/design_patterns/caregiver_assessment_and_triage.md`, `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready. Claims are bounded to end-stage ovarian cancer caregiver burden and are not treated as general gynecological cancer, earlier-stage ovarian cancer, causal, or intervention-effectiveness evidence.

## [2026-05-27] ingest | Glasgow 2001 RE-AIM chronic illness management preview

- Summary: Created an ingest preview for a Patient Education and Counseling article using the RE-AIM framework to evaluate chronic illness management intervention modalities.
- Files touched: `sources/papers/39_glasgow_reaim_framework_chronic_illness_2001.pdf`, `outputs/ingest_previews/2026-05-27_glasgow_re-aim-framework-chronic-illness-management-2001_preview.md`, `LOG.md`.
- Notes: Source type is journal article; evidence type is published evidence; privacy level is private/non-sensitive. Review status is pending before wiki integration. Proposed use is as an implementation and evaluation framework, not direct caregiver-specific or condition-specific effectiveness evidence.

## [2026-05-27] ingest | Integrated Glasgow 2001 RE-AIM chronic illness management framework

- Summary: Integrated the approved RE-AIM chronic illness management framework into citation memory, evidence, implementation/evaluation concepts, caregiver intervention evaluation design patterns, technology lenses, populations, home environment, and caregiver challenge hubs.
- Files touched: `outputs/ingest_previews/2026-05-27_glasgow_re-aim-framework-chronic-illness-management-2001_preview.md`, `wiki/references/items/2001_glasgow_re-aim-framework-chronic-illness-management.md`, `wiki/evidence/glasgow_2001_reaim_chronic_illness_management.md`, `wiki/concepts/reach_adoption_implementation_maintenance.md`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`, `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `wiki/design_patterns/clinician_portal_supported_mhealth.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/technologies/smart_home_technologies.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/populations/older_adults.md`, `wiki/environments/home.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready except DOI is unavailable from the extracted text. Claims are bounded to implementation and evaluation framework use, not caregiver-specific, condition-specific, or technology-effectiveness evidence.

## [2026-05-27] ingest | Previewed AI method sources 32 and 33

- Summary: Created pending ingest previews for Lewis et al. 2020 on retrieval-augmented generation and Yao et al. 2023 on ReAct reasoning-plus-action language model agents, plus a batch AI-method crosswalk.
- Files touched: `sources/papers/36_lewis_rag_2020.pdf`, `sources/papers/37_yao_react_2022.pdf`, `outputs/ingest_previews/2026-05-27_lewis_rag-knowledge-intensive-nlp-2020_preview.md`, `outputs/ingest_previews/2026-05-27_yao_react-reasoning-acting-language-models-2023_preview.md`, `outputs/ingest_previews/2026-05-27_batch-32-33_ai-methods-crosswalk.md`, `LOG.md`.
- Notes: Source type is conference paper for both; evidence type is published technical evidence; privacy level is private/non-sensitive. Review status is pending before wiki integration. Proposed use is technical architecture/design rationale, not clinical, caregiver-specific, condition-specific, or intervention-effectiveness evidence.

## [2026-05-27] ingest | Integrated AI method sources 32 and 33

- Summary: Integrated approved previews for Lewis et al. 2020 RAG and Yao et al. 2023 ReAct into citation memory, evidence pages, AI design patterns, technology lenses, caregiver challenge hubs, care-recipient privacy/pre-clinic pages, implementation concepts, index, and memory.
- Files touched: `outputs/ingest_previews/2026-05-27_lewis_rag-knowledge-intensive-nlp-2020_preview.md`, `outputs/ingest_previews/2026-05-27_yao_react-reasoning-acting-language-models-2023_preview.md`, `outputs/ingest_previews/2026-05-27_batch-32-33_ai-methods-crosswalk.md`, `wiki/references/items/2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp.md`, `wiki/references/items/2023_yao_react-reasoning-acting-language-models.md`, `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`, `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`, `wiki/design_patterns/retrieval_grounded_health_ai_support.md`, `wiki/design_patterns/reasoning_action_health_ai_agent.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/technologies/smart_home_technologies.md`, `wiki/design_patterns/adaptive_ai_layer_for_caregiver_mhealth.md`, `wiki/design_patterns/ai_assisted_pre_clinic_preparation.md`, `wiki/design_patterns/care_recipient_style_prompting_for_empathy.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/care_recipient_needs/pre_clinic_preparation_and_advocacy.md`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/concepts/reach_adoption_implementation_maintenance.md`, `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`, `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready except DOI fields are unavailable from extracted text. Claims are bounded to technical architecture/design rationale, not clinical, caregiver-specific, condition-specific, safety, usability, or intervention-effectiveness evidence.

## [2026-05-28] ingest | Previewed part 2 CareBuddy abstract and paper

- Summary: Created pending ingest previews for a 2025 Innovation in Aging abstract on CareBuddy multi-agent conversational AI for Alzheimer's care and a 2025 JMIR Aging paper on CareBuddy as a mobile care ecosystem for dementia caregivers, plus a part 2 crosswalk.
- Files touched: `sources/abstracts/2025_gsa_carebuddy.pdf`, `sources/papers/malhotra_carebuddy_2025.pdf`, `outputs/ingest_previews/2026-05-28_hasan_carebuddy-multi-agent-conversational-ai-alzheimers-2025_preview.md`, `outputs/ingest_previews/2026-05-28_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving-2025_preview.md`, `outputs/ingest_previews/2026-05-28_batch-part-2_carebuddy-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. The abstract is conference-level evidence; the JMIR article is published development/usability/acceptability evidence. Neither should be treated as clinical effectiveness evidence.

## [2026-05-28] ingest | Integrated part 2 CareBuddy abstract and paper

- Summary: Integrated approved CareBuddy part 2 sources into citation memory, evidence pages, dementia, family caregiver and older adult population pages, AI/smart-home technology lenses, caregiver challenge hubs, care-recipient privacy, design patterns, evaluation questions, index, memory, and log.
- Files touched: `outputs/ingest_previews/2026-05-28_hasan_carebuddy-multi-agent-conversational-ai-alzheimers-2025_preview.md`, `outputs/ingest_previews/2026-05-28_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving-2025_preview.md`, `outputs/ingest_previews/2026-05-28_batch-part-2_carebuddy-crosswalk.md`, `wiki/references/items/2025_hasan_carebuddy-multi-agent-conversational-ai-alzheimers.md`, `wiki/references/items/2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving.md`, `wiki/evidence/hasan_2025_carebuddy_multi_agent_conversational_ai_alzheimers.md`, `wiki/evidence/malhotra_2025_carebuddy_mobile_care_ecosystem_dementia_caregiving.md`, `wiki/conditions/dementia.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/older_adults.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/technologies/smart_home_technologies.md`, `wiki/caregiving_challenges/information_access_and_health_literacy.md`, `wiki/caregiving_challenges/care_coordination_and_shared_access.md`, `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`, `wiki/caregiving_challenges/emotional_and_social_support.md`, `wiki/caregiving_challenges/monitoring_and_safety_awareness.md`, `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`, `wiki/design_patterns/one_stop_caregiver_support_app.md`, `wiki/design_patterns/retrieval_grounded_health_ai_support.md`, `wiki/design_patterns/reasoning_action_health_ai_agent.md`, `wiki/design_patterns/clinician_portal_supported_mhealth.md`, `wiki/design_patterns/real_world_reliability_for_mhealth_data_capture.md`, `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Claims are bounded to abstract-level usability signals for Hasan 2025 and development/usability/acceptability evidence for Malhotra 2025; neither is treated as clinical effectiveness evidence.

## [2026-06-01] workflow | Renumbered paper source filenames to updated citation list

- Summary: Compared `sources/papers/` against the updated citation list, identified newly added non-ingested paper PDFs, and renumbered existing paper filenames to match the updated list while leaving user-authored Hu and Setiawan sources unnumbered.
- Files touched: `sources/papers/`, `wiki/evidence/`, `wiki/references/items/`, `LOG.md`.
- Notes: Newly added but not ingested papers are `03_schulz_PHYSICAL AND MENTAL HEALTH EFFECTS OF FAMILY CAREGIVING.pdf` and `07_zhai_digital_health_fcg_support_systematic_review.pdf`. No new source ingest was performed. Abstract filenames were intentionally left unchanged.

## [2026-06-01] ingest | Previewed stress-process and caregiver health-effects sources 01 and 03

- Summary: Created pending ingest previews for Aneshensel and Avison 2015 on Pearlin's stress-process legacy and Schulz and Sherwood 2008 on physical and mental health effects of family caregiving, plus a batch crosswalk for stress-process and caregiver-health mapping.
- Files touched: `sources/papers/01_the stress process.pdf`, `sources/papers/03_schulz_PHYSICAL AND MENTAL HEALTH EFFECTS OF FAMILY CAREGIVING.pdf`, `outputs/ingest_previews/2026-06-01_aneshensel-avison_stress-process-appreciation-pearlin-2015_preview.md`, `outputs/ingest_previews/2026-06-01_schulz-sherwood_physical-mental-health-effects-family-caregiving-2008_preview.md`, `outputs/ingest_previews/2026-06-01_batch-01-03_stress-and-caregiver-health-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Source 01 is readable but is Aneshensel and Avison 2015, a secondary appreciation/overview of Pearlin's stress-process work, not the original Pearlin et al. 1981 stress-process article. Source 03 is readable and provides caregiver health-effects framing, not technology or intervention-effectiveness evidence.

## [2026-06-01] ingest | Refined source 01 preview with Pearlin stress-process verification

- Summary: Updated the pending source 01 preview and batch crosswalk so Aneshensel and Avison 2015 is framed as a readable modern gateway into Pearlin's original stress-process model, with supplemental online verification of the 1981 original stress-process article, the 1990 caregiving-specific stress-process article, Pearlin's 1989 sociological stress paper, and the later stress-process revisited framing.
- Files touched: `outputs/ingest_previews/2026-06-01_aneshensel-avison_stress-process-appreciation-pearlin-2015_preview.md`, `outputs/ingest_previews/2026-06-01_batch-01-03_stress-and-caregiver-health-crosswalk.md`, `LOG.md`.
- Notes: Supplemental online sources were used for identity and focus verification only; they are not yet integrated wiki evidence or canonical citation-memory records.

## [2026-06-01] ingest | Integrated stress-process and caregiver health-effects sources 01 and 03

- Summary: Integrated approved previews for Aneshensel and Avison 2015 and Schulz and Sherwood 2008 into citation memory, evidence pages, stress-process concepts, caregiver population pages, dementia and older-adult context, caregiver challenge hubs, design patterns, index, memory, and log.
- Files touched: `wiki/references/items/2015_aneshensel-avison_stress-process-appreciation-pearlin.md`, `wiki/references/items/2008_schulz-sherwood_physical-mental-health-effects-family-caregiving.md`, `wiki/evidence/aneshensel_avison_2015_stress_process_appreciation_pearlin.md`, `wiki/evidence/schulz_sherwood_2008_physical_mental_health_effects_family_caregiving.md`, `wiki/concepts/`, `wiki/populations/`, `wiki/conditions/dementia.md`, `wiki/caregiving_challenges/`, `wiki/design_patterns/`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Source 01 is treated as a readable secondary gateway into Pearlin's stress-process architecture, not as the original 1981 or 1990 Pearlin paper. Source 03 is caregiver health-effects framing, not technology or intervention-effectiveness evidence.

## [2026-06-01] ingest | Previewed digital caregiver intervention sources 07 and 09

- Summary: Created pending ingest previews for Graven et al. 2021 on telehealth interventions for family caregivers of people with chronic health conditions and Zhai et al. 2023 on digital health interventions and HCD approaches for family caregivers, plus a batch crosswalk for telehealth, digital health, HCD, and caregiver outcome mapping.
- Files touched: `sources/papers/07_gaven_telehealth_pwccd_rct_review.pdf`, `sources/papers/09_zhai_digital_health_fcg_support_systematic_review.pdf`, `outputs/ingest_previews/2026-06-01_graven_telehealth-interventions-family-caregivers-chronic-conditions-2021_preview.md`, `outputs/ingest_previews/2026-06-01_zhai_digital-health-interventions-support-family-caregivers-2023_preview.md`, `outputs/ingest_previews/2026-06-01_batch-07-09_digital-caregiver-intervention-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Both PDFs extracted readable text with Ghostscript. Source 07 is RCT-focused telehealth caregiver intervention evidence; source 09 is broader modern digital health and HCD evidence. Neither should be treated as AI-agent or smart-home effectiveness evidence.

## [2026-06-01] ingest | Integrated digital caregiver intervention sources 07 and 09

- Summary: Integrated approved previews for Graven et al. 2021 and Zhai et al. 2023 into citation memory, evidence pages, digital health and smart-home technology lenses, family caregiver and older-adult population pages, dementia context, caregiver challenge hubs, design patterns, research questions, index, memory, and log.
- Files touched: `wiki/references/items/2021_graven_telehealth-interventions-family-caregivers-chronic-conditions.md`, `wiki/references/items/2023_zhai_digital-health-interventions-support-family-caregivers.md`, `wiki/evidence/graven_2021_telehealth_interventions_family_caregivers_chronic_conditions.md`, `wiki/evidence/zhai_2023_digital_health_interventions_support_family_caregivers.md`, `wiki/technologies/`, `wiki/populations/`, `wiki/conditions/dementia.md`, `wiki/caregiving_challenges/`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Graven 2021 is telehealth RCT-review evidence; Zhai 2023 is broader digital health and HCD evidence. Neither is treated as AI-agent or smart-home effectiveness evidence, and usability/acceptability remain separate from effectiveness.

## [2026-06-01] workflow | Refined review and single-study ingest depth

- Summary: Updated the source-ingest workflow to require source-type-specific extraction depth, then refined the Graven 2021 and Zhai 2023 evidence and citation-memory records with clearer review-level takeaways, technology/intervention taxonomies, population/equity scope, outcome/evidence-quality framing, and explicit unanswered questions.
- Files touched: `wiki/workflows/ingest_source.md`, `wiki/evidence/graven_2021_telehealth_interventions_family_caregivers_chronic_conditions.md`, `wiki/evidence/zhai_2023_digital_health_interventions_support_family_caregivers.md`, `wiki/references/items/2021_graven_telehealth-interventions-family-caregivers-chronic-conditions.md`, `wiki/references/items/2023_zhai_digital-health-interventions-support-family-caregivers.md`, `MEMORY.md`, `LOG.md`.
- Notes: New ingest standard distinguishes review/meta/scoping source extraction from single-study extraction. Review sources should preserve inclusion logic, technology/intervention taxonomy, outcome taxonomy, equity/HCD/accessibility details, review-level takeaway, and what the review does not answer. Single studies should preserve a compact full-study picture.
