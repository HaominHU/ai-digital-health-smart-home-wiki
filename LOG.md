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

## [2026-06-03] ingest | Koroshetz morning lecture neuroscience takeaways translated to SCI

- Summary: Integrated standalone morning first lecture notes from Dr. Walter Koroshetz at the 2026 University of Pittsburgh Rehabilitation Research Institute day event as SCI research, clinical trial, and engineering framing.
- Files touched: `sources/presentation_notes/2026-06-03_koroshetz_neuroscience-take-home-points-sci-translation.md`, `wiki/evidence/koroshetz_2026_neuroscience_takeaways_sci_translation.md`, `wiki/conditions/spinal_cord_injury.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is lecture notes; evidence type is presentation takeaway; privacy level is private/non-sensitive. User specified that Gemini 3.5 Flash translated original slide points from `image.png` into SCI-specific settings. Citation-memory status: no formal citation record created because this is not a citation-bearing publication. Review status: automatically integrated as low-risk standalone event notes, separate from the ongoing caregiver system ingest and separate from the middle Mac setup talk.

## [2026-06-03] ingest | Fridriksson brain health and aphasia recovery lecture

- Summary: Integrated standalone second lecture notes from Dr. Julius Fridriksson as chronic-condition/disability neurorehabilitation framing for brain health, aphasia recovery, biomarker tracking, trial stratification, and longitudinal rehabilitation analytics.
- Files touched: `sources/presentation_notes/2026-06-03_fridriksson_brain-health-aphasia-recovery.md`, `wiki/evidence/fridriksson_2026_brain_health_aphasia_recovery.md`, `wiki/design_patterns/biomarker_stratified_neurorehabilitation.md`, `wiki/research_questions/biomarker_stratified_neurorehabilitation.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`, `wiki/technologies/ai_driven_digital_health.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is lecture notes; evidence type is presentation takeaway; privacy level is private/non-sensitive. Aphasia was not added as a focused condition overlay per user instruction; it was treated as chronic-condition/disability neurorehabilitation context. Citation-memory status: no formal citation record created because this is not a citation-bearing publication.

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

## [2026-06-02] ingest | Previewed dementia caregiver intervention sources 10, 11, 12, 13, and 42

- Summary: Checked current source status and created pending ingest previews for REACH II/REACH VA healthcare cost evidence, the COPE randomized trial, the Savvy Caregiver transportability field test, the Tele-Savvy randomized trial, and Walter and Pinquart's updated dementia caregiver intervention meta-analysis, plus a batch crosswalk.
- Files touched: `sources/papers/10_reachii_reachva.pdf`, `sources/papers/11_laura_cope.pdf`, `sources/papers/12_hepburn_savvy.pdf`, `sources/papers/13_hepburn_telesavvy.pdf`, `sources/papers/42_walter_updated_caregiver_intervention_analysis.pdf`, `outputs/ingest_previews/2026-06-02_nichols_reach-dementia-caregiver-healthcare-costs-2017_preview.md`, `outputs/ingest_previews/2026-06-02_gitlin_cope-dementia-home-based-intervention-2010_preview.md`, `outputs/ingest_previews/2026-06-02_hepburn_savvy-caregiver-transportable-program-2003_preview.md`, `outputs/ingest_previews/2026-06-02_hepburn_telesavvy-online-dementia-caregiver-program-2022_preview.md`, `outputs/ingest_previews/2026-06-02_walter-pinquart_dementia-caregiver-interventions-meta-analysis-2020_preview.md`, `outputs/ingest_previews/2026-06-02_batch-10-13-42_dementia-caregiver-intervention-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. These sources are dementia caregiver intervention, implementation, cost, transportability, online delivery, and meta-analytic evidence. They should not be treated as AI-agent, smart-home, normal-aging, or dementia treatment evidence.

## [2026-06-02] ingest | Integrated dementia caregiver intervention sources 10, 11, 12, 13, and 42

- Summary: Integrated approved previews for REACH II/REACH VA costs, COPE, Savvy Caregiver, Tele-Savvy, and Walter and Pinquart 2020 into citation memory, evidence pages, dementia and family caregiver pages, caregiver challenge hubs, care-recipient need pages, design patterns, research questions, index, memory, and log.
- Files touched: `outputs/ingest_previews/2026-06-02_*`, `wiki/references/items/2017_nichols_reach-dementia-caregiver-healthcare-costs.md`, `wiki/references/items/2010_gitlin_cope-dementia-home-based-intervention.md`, `wiki/references/items/2003_hepburn_savvy-caregiver-transportable-program.md`, `wiki/references/items/2022_hepburn_telesavvy-online-dementia-caregiver-program.md`, `wiki/references/items/2020_walter-pinquart_dementia-caregiver-interventions-meta-analysis.md`, `wiki/evidence/nichols_2017_reach_dementia_caregiver_healthcare_costs.md`, `wiki/evidence/gitlin_2010_cope_dementia_home_based_intervention.md`, `wiki/evidence/hepburn_2003_savvy_caregiver_transportable_program.md`, `wiki/evidence/hepburn_2022_telesavvy_online_dementia_caregiver_program.md`, `wiki/evidence/walter_pinquart_2020_dementia_caregiver_interventions_meta_analysis.md`, `wiki/conditions/dementia.md`, `wiki/populations/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `wiki/environments/home.md`, `wiki/technologies/ai_driven_digital_health.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready except Gitlin 2010 lacks DOI/URL from extracted text. Claims are bounded to dementia caregiver intervention, implementation, cost, transportability, online delivery, and meta-analytic evidence.

## [2026-06-04] workflow | Documented paper source purpose lanes

- Summary: Updated the source-layer structure to distinguish the ongoing caregiver system-design core citation lane from the monthly PubMed push storage lane, and repaired current source references for moved core papers.
- Files touched: `AGENTS.md`, `README.md`, `INDEX.md`, `MEMORY.md`, `wiki/workflows/ingest_source.md`, `wiki/evidence/`, `wiki/references/items/`, `outputs/ingest_previews/`, `LOG.md`.
- Notes: `sources/papers/cg_system_core/` and `sources/papers/monthly_pubmed/` are example purpose-specific lanes, not a closed list. New paper-group folders can be added as new stable source groups emerge. `monthly_pubmed` should remain flat for now, with another hierarchy added later only if needed. Top-level `sources/papers/` remains available for legacy, standalone, or unassigned papers.

## [2026-06-04] memory | Revised non-ingested paper status

- Summary: Updated `MEMORY.md` after a quick source-status sweep to mark the current non-ingested paper explicitly.
- Files touched: `MEMORY.md`, `LOG.md`.
- Notes: `sources/papers/monthly_pubmed/kingsada_2026_preferences_dh_scope_review.pdf` is stored but not yet previewed, integrated, or represented in citation memory. Current core citation papers through source 42 remain previewed and integrated.

## [2026-06-04] ingest | Previewed monthly PubMed paper on DHT preferences

- Summary: Created a pending ingest preview for Kingsada et al. 2026, a Health Economics Review scoping review on patient preferences toward digital health technologies.
- Files touched: `sources/papers/monthly_pubmed/kingsada_2026_preferences_dh_scope_review.pdf`, `outputs/ingest_previews/2026-06-04_kingsada_preferences-digital-health-technologies-2026_preview.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source type is scoping review; evidence type is published evidence; privacy level is private/non-sensitive. Review status is pending before wiki integration. This source belongs to the monthly PubMed lane and remains separate from the `cg_system_core` caregiver system-design ingest.

## [2026-06-04] ingest | Integrated monthly PubMed DHT preferences review

- Summary: Integrated the approved Kingsada et al. 2026 scoping review into citation memory, a new evidence page, digital-health technology context, older-adult population context, caregiver/care-recipient preference separation, design patterns, research questions, index, memory, and log.
- Files touched: `outputs/ingest_previews/2026-06-04_kingsada_preferences-digital-health-technologies-2026_preview.md`, `wiki/references/items/2026_kingsada_preferences-digital-health-technologies.md`, `wiki/evidence/kingsada_2026_preferences_digital_health_technologies.md`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/populations/older_adults.md`, `wiki/concepts/caregiver_vs_care_recipient_needs.md`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready with article-in-press limits: final volume, issue, and page/article fields were not available from the accepted manuscript. Claims are bounded to patient preferences, DHT adoption, preference elicitation, HTA/reimbursement rationale, older-adult preference context, and privacy/security design rationale. This source remains separate from `cg_system_core` and is not caregiver-specific or intervention-effectiveness evidence.

## [2026-06-06] memory | Noted part 5 dementia caregiver source gaps

- Summary: Recorded the planned part 5 dementia caregiver source queue and why AHRQ 2020 is not in the immediate ingest batch.
- Files touched: `MEMORY.md`, `LOG.md`.
- Notes: AHRQ 2020 is skipped for now because it is over 500 pages. No source ingest was performed.

## [2026-06-06] memory | Added caregiver system core reference plan

- Summary: Added a planning-only reference map for the caregiver system core source backbone, connecting prior ingest batches to the planned part 5 dementia caregiver sources and later theory, SCI, gynecologic cancer, AI-agent, and implementation/evaluation source families.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: This file is a source-selection and continuity aid, not canonical citation memory or source-backed evidence. Individual citation records should still be created only after preview-first ingest.

## [2026-06-06] workflow | Renumbered core paper source files to updated Tier 1 list

- Summary: Rescanned `sources/papers/cg_system_core/`, then renumbered local core paper files and source references to match the updated core-list structure without ingesting new sources.
- Files touched: `sources/papers/cg_system_core/`, `wiki/evidence/`, `wiki/references/items/`, `outputs/ingest_previews/`, `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `LOG.md`.
- Notes: Part 5 immediate ingest queue is now Cheng 2020, Bressan 2020, and Ruggiano 2021. AHRQ 2020 remains skipped for now. Previously integrated but deprioritized sources were retained in the wiki and moved to the 30+ range where applicable.

## [2026-06-07] memory | Revised core reference plan numbering notes

- Summary: Updated the caregiver system core reference plan so it matches the newly numbered base list through 29 plus 30+ supporting sources.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `LOG.md`.
- Notes: AHRQ 2020 remains skipped for now without an active source number. No source ingest was performed.

## [2026-06-07] memory | Simplified core reference plan to starter list

- Summary: Simplified the caregiver system core reference plan so it keeps only the updated base-through-29 starter list, 30+ supporting-source model, and AHRQ 2020 as a future potential reference.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `LOG.md`.
- Notes: Sources outside the updated starter list are removed from the plan rather than retained as removed/deferred status rows. No source ingest was performed.

## [2026-06-07] ingest | Previewed part 5 dementia caregiver sources 13, 14, and 15

- Summary: Created approved-integrated ingest previews for Cheng and Zhang 2020 on dementia caregiver intervention meta-review evidence, Bressan et al. 2020 on dementia caregiver needs, and Ruggiano et al. 2021 on dementia chatbot functions and quality.
- Files touched: `outputs/ingest_previews/2026-06-07_cheng_meta-review-dementia-caregiver-interventions-2020_preview.md`, `outputs/ingest_previews/2026-06-07_bressan_dementia-caregiver-needs-mixed-method-review-2020_preview.md`, `outputs/ingest_previews/2026-06-07_ruggiano_chatbots-dementia-caregivers-2021_preview.md`, `LOG.md`.
- Notes: The user directly instructed ingest of sources 13-15, so previews were produced and carried into integration in the same run. Cheng and Bressan are dementia caregiver intervention/needs synthesis sources; Ruggiano is chatbot function/quality and evidence-gap evidence.

## [2026-06-07] ingest | Integrated part 5 dementia caregiver sources 13, 14, and 15

- Summary: Integrated Cheng 2020, Bressan 2020, and Ruggiano 2021 into citation memory, evidence pages, dementia and family caregiver pages, caregiver challenge hubs, care-recipient privacy/autonomy, AI/RAG technology and design patterns, caregiver evaluation logic, index, memory, and the core reference plan.
- Files touched: `wiki/references/items/2020_cheng_meta-review-dementia-caregiver-interventions.md`, `wiki/references/items/2020_bressan_dementia-caregiver-needs-mixed-method-review.md`, `wiki/references/items/2021_ruggiano_chatbots-dementia-caregivers.md`, `wiki/evidence/cheng_2020_meta_review_dementia_caregiver_interventions.md`, `wiki/evidence/bressan_2020_dementia_caregiver_needs_mixed_method_review.md`, `wiki/evidence/ruggiano_2021_chatbots_dementia_caregivers.md`, `wiki/conditions/dementia.md`, `wiki/populations/family_caregivers.md`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/design_patterns/`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Part 5 closes the narrowed dementia/ADRD caregiver Tier 1 branch in section 3 of the updated core reference plan. Claims are bounded to review-level dementia caregiver intervention synthesis, needs synthesis, and chatbot function/quality evidence; usability, acceptability, app-store availability, or chatbot feature review are not treated as effectiveness evidence.

## [2026-06-07] ingest | Refined part 5 previews with review-level story strategy

- Summary: Revised the Part 5 ingest previews so Cheng 2020, Bressan 2020, and Ruggiano 2021 each include an explicit review-level takeaway and story section, making the preview strategy from the prior batch visible before wiki integration.
- Files touched: `outputs/ingest_previews/2026-06-07_cheng_meta-review-dementia-caregiver-interventions-2020_preview.md`, `outputs/ingest_previews/2026-06-07_bressan_dementia-caregiver-needs-mixed-method-review-2020_preview.md`, `outputs/ingest_previews/2026-06-07_ruggiano_chatbots-dementia-caregivers-2021_preview.md`, `LOG.md`.
- Notes: All three Part 5 sources are reviews, so the added sections use review-level takeaway/story framing rather than standalone empirical full-study storytelling.

## [2026-06-10] memory | Noted source 22 SCI website boundary before part 6

- Summary: Added a pre-ingest planning note that source 22 is the NINDS spinal cord injury knowledge website, not a local PDF to ingest in Part 6.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source 22 should be checked only when disease-background knowledge is needed and should not be treated as caregiver-specific, intervention-effectiveness, digital health, AI, or smart-home evidence.

## [2026-06-10] ingest | Previewed part 6 SCI caregiver problem-solving sources 16 and 17

- Summary: Created pending ingest previews for Elliott et al. 2008 on videoconferencing problem-solving training for SCI caregivers and Elliott and Berry 2009 on brief problem-solving training for recent-onset SCI caregivers, plus a batch crosswalk.
- Files touched: `outputs/ingest_previews/2026-06-10_elliott_problem-solving-videoconferencing-sci-caregivers-2008_preview.md`, `outputs/ingest_previews/2026-06-10_elliott_brief-problem-solving-training-sci-caregivers-2009_preview.md`, `outputs/ingest_previews/2026-06-10_batch-16-17_sci-problem-solving-intervention-crosswalk.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Both sources are SCI caregiver randomized controlled trial evidence for problem-solving support. Source 16 includes telehealth/videoconferencing delivery and possible care-recipient social-functioning spillover; source 17 supports brief PST plus education for dysfunctional problem-solving style but not caregiver depression. Neither source should be treated as AI-agent, smart-home, disease-treatment, or broad clinical-effectiveness evidence.

## [2026-06-10] ingest | Integrated part 6 SCI caregiver problem-solving sources 16 and 17

- Summary: Integrated approved previews for Elliott et al. 2008 and Elliott and Berry 2009 into citation memory, evidence pages, SCI, family caregiver and PwCCD population pages, caregiver challenge hubs, care-recipient outcomes, home context, design patterns, AI/digital health delivery boundary, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-10_elliott_problem-solving-videoconferencing-sci-caregivers-2008_preview.md`, `outputs/ingest_previews/2026-06-10_elliott_brief-problem-solving-training-sci-caregivers-2009_preview.md`, `outputs/ingest_previews/2026-06-10_batch-16-17_sci-problem-solving-intervention-crosswalk.md`, `wiki/references/items/2008_elliott_problem-solving-videoconferencing-sci-caregivers.md`, `wiki/references/items/2009_elliott_brief-problem-solving-training-sci-caregivers.md`, `wiki/evidence/elliott_2008_problem_solving_videoconferencing_sci_caregivers.md`, `wiki/evidence/elliott_2009_brief_problem_solving_training_sci_caregivers.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/populations/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/technologies/ai_driven_digital_health.md`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Claims are bounded to SCI caregiver problem-solving intervention evidence. Source 16 supports remote/videoconferencing delivery and dyadic outcome evaluation with high-attrition and mechanism limits. Source 17 supports brief PST plus education for dysfunctional problem-solving style, not caregiver depression effectiveness. Neither source is AI-agent, smart-home, disease-treatment, or autonomous clinical decision evidence.

## [2026-06-11] ingest | Previewed part 6 SCI caregiving services source 18

- Summary: Created a pending ingest preview for Smith et al. 2016, a PRISMA-guided systematic review of caregiving services in spinal cord injury.
- Files touched: `outputs/ingest_previews/2026-06-11_smith_caregiving-services-sci-systematic-review-2016_preview.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. The source synthesizes SCI caregiving service structure, formal/informal care, care hours, functional predictors, and caregiver/attendant training evidence. It explicitly excludes caregiver experience and burden studies, so it should not be used as the main SCI caregiver burden synthesis. It is not AI, smart-home, mHealth, or SCI disease-background evidence.

## [2026-06-11] ingest | Integrated part 6 SCI caregiving services source 18

- Summary: Integrated approved preview for Smith et al. 2016 into citation memory, evidence, SCI, family caregiver and PwCCD population pages, caregiver challenge hubs, care-recipient secondary-complication support, home context, design patterns, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-11_smith_caregiving-services-sci-systematic-review-2016_preview.md`, `wiki/references/items/2016_smith_caregiving-services-sci-systematic-review.md`, `wiki/evidence/smith_2016_caregiving_services_sci_systematic_review.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/populations/family_caregivers.md`, `wiki/populations/people_with_chronic_conditions_and_disabilities.md`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready. Claims are bounded to SCI caregiving service structure, formal/informal care, care hours, functional predictors, service-quality gaps, and caregiver/attendant training. The review excluded caregiver burden and lived-experience studies, so it should not be used as the primary SCI caregiver burden synthesis. It is not AI, smart-home, mHealth, autonomous care, or SCI disease-background evidence.

## [2026-06-11] ingest | Previewed part 6 SCI caregiver burden and well-being sources 20 and 21

- Summary: Created pending ingest previews for Conti et al. 2019 on secondary conditions and SCI family caregiver burden, and Ryerson Espino et al. 2022 on coping, social support, and SCI caregiver well-being.
- Files touched: `outputs/ingest_previews/2026-06-11_conti_secondary-conditions-caregiver-burden-sci-2019_preview.md`, `outputs/ingest_previews/2026-06-11_espino_coping-social-support-caregiver-wellbeing-sci-2022_preview.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Source 20 is cross-sectional correlational dyad evidence linking care-recipient physical secondary conditions and functional independence to caregiver burden dimensions. Source 21 is mixed-method/profile evidence for coping, social support, unmet needs, and caregiver well-being. Neither source is AI, smart-home, autonomous care, digital intervention-effectiveness, or SCI disease-background evidence.

## [2026-06-11] ingest | Integrated part 6 SCI caregiver burden and well-being sources 20 and 21

- Summary: Integrated approved previews for Conti et al. 2019 and Ryerson Espino et al. 2022 into citation memory, evidence pages, SCI, family caregiver and PwCCD population pages, caregiver challenge hubs, care-recipient secondary-complication and autonomy pages, home context, design patterns, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-11_conti_secondary-conditions-caregiver-burden-sci-2019_preview.md`, `outputs/ingest_previews/2026-06-11_espino_coping-social-support-caregiver-wellbeing-sci-2022_preview.md`, `wiki/references/items/2019_conti_secondary-conditions-caregiver-burden-sci.md`, `wiki/references/items/2022_espino_coping-social-support-caregiver-wellbeing-sci.md`, `wiki/evidence/conti_2019_secondary_conditions_caregiver_burden_sci.md`, `wiki/evidence/espino_2022_coping_social_support_caregiver_wellbeing_sci.md`, `wiki/conditions/spinal_cord_injury.md`, `wiki/populations/`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Source 20 is bounded to cross-sectional correlational SCI burden-mechanism evidence linking care-recipient physical secondary conditions, functional independence, and caregiver burden dimensions. Source 21 is bounded to mixed-method exploratory evidence for SCI caregiver coping, social support, unmet needs, red flags, respite, and support profiles. Neither source is AI, smart-home, autonomous care, digital intervention-effectiveness, or SCI disease-background evidence.

## [2026-06-11] memory | Noted source 27 NCI PDQ link boundary before part 7

- Summary: Added a pre-ingest planning note that source 27 is the NCI PDQ family caregiver professional page, not a local PDF to ingest in Part 7.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `LOG.md`.
- Notes: Source 27 should be checked only when cancer caregiver background, framework, or clinical-context knowledge is needed and should not be treated as a PDF ingest source, AI evidence, digital health evidence, smart-home evidence, or intervention-effectiveness evidence unless later source review directly supports that role.

## [2026-06-11] ingest | Previewed part 7 advanced cancer caregiver intervention source 24

- Summary: Created a pending ingest preview for Becque et al. 2023, a systematic review of supportive interventions for family caregivers of patients with advanced cancer.
- Files touched: `sources/papers/cg_system_core/24_becque_2023_supportive_interention_caregiver_advanced_cancer.pdf`, `outputs/ingest_previews/2026-06-11_becque_supportive-interventions-family-caregivers-advanced-cancer-2023_preview.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. The PDF has a two-column journal layout; Ghostscript extraction was usable for abstract, methods, narrative results, discussion, and conclusions, while long tables contained extraction artifacts. Claims should stay bounded to broad advanced cancer caregiver supportive-intervention taxonomy and outcome mapping, not gynecological-cancer-specific effectiveness, AI-agent, smart-home, mHealth, or cancer-treatment evidence.

## [2026-06-11] ingest | Integrated part 7 advanced cancer caregiver intervention source 24

- Summary: Integrated approved preview for Becque et al. 2023 into citation memory, evidence, family caregiver, gynecological cancer, caregiver challenge, home environment, design pattern, research question, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-11_becque_supportive-interventions-family-caregivers-advanced-cancer-2023_preview.md`, `wiki/references/items/2023_becque_supportive-interventions-family-caregivers-advanced-cancer.md`, `wiki/evidence/becque_2023_supportive_interventions_advanced_cancer_caregivers.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/populations/family_caregivers.md`, `wiki/caregiving_challenges/`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready. Claims are bounded to broad advanced cancer caregiver supportive-intervention taxonomy, target-population matching, and caregiver outcome-domain mapping. The source is not gynecological-cancer-specific effectiveness evidence, AI-agent evidence, smart-home evidence, mHealth effectiveness evidence, autonomous care evidence, or cancer-treatment evidence.

## [2026-06-11] ingest | Previewed part 7 cancer caregiver implementation source 23

- Summary: Created a pending ingest preview for Ugalde et al. 2019, a systematic review appraising cancer caregiver interventions for implementation potential.
- Files touched: `sources/papers/cg_system_core/23_ugalde_A systematic review of cancer caregiver interventions  Appraising the potential for.pdf`, `outputs/ingest_previews/2026-06-11_ugalde_cancer-caregiver-interventions-implementation-potential-2019_preview.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Ghostscript extraction was usable for abstract, methods, narrative results, discussion, conclusions, and references; long study-characteristics tables contained layout artifacts. Claims should stay bounded to broad cancer caregiver intervention implementation-readiness evidence using Proctor implementation outcomes, not gynecological-cancer-specific effectiveness, AI-agent, smart-home, mHealth, autonomous-care, or cancer-treatment evidence.

## [2026-06-11] ingest | Integrated part 7 cancer caregiver implementation source 23

- Summary: Integrated approved preview for Ugalde et al. 2019 into citation memory, evidence, family caregiver, gynecological cancer, caregiver challenge, home environment, design pattern, research question, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-11_ugalde_cancer-caregiver-interventions-implementation-potential-2019_preview.md`, `wiki/references/items/2019_ugalde_cancer-caregiver-interventions-implementation-potential.md`, `wiki/evidence/ugalde_2019_cancer_caregiver_interventions_implementation_potential.md`, `wiki/populations/family_caregivers.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/caregiving_challenges/`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory record is RIS export-ready. Claims are bounded to broad cancer caregiver intervention implementation-readiness evidence using Proctor implementation outcomes, including acceptability, adoption, appropriateness, feasibility, fidelity, cost, caregiver co-design, reach/enrollment, workforce, and delivery-resource reporting. The source is not gynecological-cancer-specific effectiveness evidence, AI-agent evidence, smart-home evidence, mHealth effectiveness evidence, autonomous-care evidence, or cancer-treatment evidence.

## [2026-06-11] ingest | Previewed part 7 gynecologic and cancer caregiver sources 25 and 28

- Summary: Created pending ingest previews for Campbell et al. 2024 on gynecologic cancer patient-caregiver mHealth self-management needs and Dave et al. 2024 on broad cancer caregiver needs, intervention examples, and patient advocacy group roles.
- Files touched: `sources/papers/cg_system_core/25_campbell_2024_needs_mHealth_self_management_focus_group.pdf`, `sources/papers/cg_system_core/28_dave_2024_Identifying and addressing the needs of caregivers of patients with cancer  evidence on interventions and the role of patient advocacy groups.pdf`, `outputs/ingest_previews/2026-06-11_campbell_gynecologic-cancer-caregiver-mhealth-self-management-2024_preview.md`, `outputs/ingest_previews/2026-06-11_dave_cancer-caregiver-needs-patient-advocacy-groups-2024_preview.md`, `LOG.md`.
- Notes: Review status is pending before wiki integration. Source 25 is direct gynecologic cancer formative qualitative mHealth design evidence, not mHealth effectiveness, AI, smart-home, autonomous triage, or cancer-treatment evidence. Source 28 is a narrative review and advocacy-ecosystem framing source, not a systematic review, gynecological-cancer-specific evidence, intervention-effectiveness proof, AI, smart-home, or mHealth effectiveness evidence.

## [2026-06-11] ingest | Integrated part 7 gynecologic and cancer caregiver sources 25 and 28

- Summary: Integrated approved previews for Campbell et al. 2024 and Dave et al. 2024 into citation memory, evidence, family caregiver, gynecological cancer, caregiver challenge, care-recipient autonomy/privacy, home environment, design pattern, research question, index, memory, and the core reference plan.
- Files touched: `outputs/ingest_previews/2026-06-11_campbell_gynecologic-cancer-caregiver-mhealth-self-management-2024_preview.md`, `outputs/ingest_previews/2026-06-11_dave_cancer-caregiver-needs-patient-advocacy-groups-2024_preview.md`, `wiki/references/items/2024_campbell_gynecologic-cancer-caregiver-mhealth-self-management-needs.md`, `wiki/references/items/2024_dave_cancer-caregiver-needs-patient-advocacy-groups.md`, `wiki/evidence/campbell_2024_gynecologic_cancer_caregiver_mhealth_self_management_needs.md`, `wiki/evidence/dave_2024_cancer_caregiver_needs_patient_advocacy_groups.md`, `wiki/populations/family_caregivers.md`, `wiki/conditions/gynecological_cancer.md`, `wiki/caregiving_challenges/`, `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`, `wiki/environments/home.md`, `wiki/design_patterns/`, `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`, `wiki/references/cg_system_core_reference_plan.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Citation-memory records are RIS export-ready. Source 25 is bounded to direct gynecologic cancer formative mHealth design evidence around curated information, self-triage needs, trajectory tailoring, expert/peer support, private spaces, and sharing controls. Source 28 is bounded to broad cancer caregiver unmet-needs and patient advocacy ecosystem framing. Neither source should be treated as mHealth effectiveness, AI-agent, smart-home, autonomous-care, cancer-treatment, or unsupported clinical decision evidence; source 28 is not a systematic review.

## [2026-06-11] output | Caregiver system core SoTA synthesis

- Summary: Created a living owner-facing SoTA synthesis for the completed `cg_system_core` Tier 1 ingest, covering family caregiving outcomes, digital health intervention types/mechanisms/modalities, dementia/SCI/gynecological cancer condition distinctions, evidence boundaries, and research directions.
- Files touched: `wiki/overview/caregiver_system_core_sota_synthesis.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: This is maintained wiki synthesis rather than a task-specific output. It should be revised after future relevant caregiver, digital health, AI, smart-home, implementation, or condition-specific ingests.

## [2026-06-11] output | Revised caregiver system SoTA outcome framing

- Summary: Revised the SoTA synthesis so the leading outcomes section describes outcomes of being a caregiver and providing care, while intervention-response logic now sits under a separate informed intervention design section.
- Files touched: `wiki/overview/caregiver_system_core_sota_synthesis.md`, `LOG.md`.
- Notes: This preserves the distinction between descriptive caregiving outcomes, care-recipient and dyadic effects, and intervention design logic.

## [2026-06-11] memory | Prevent publishing local ingest previews

- Summary: Added a durable commit/publish guardrail that `outputs/ingest_previews/` files are local-only by default and should not be force-added unless explicitly requested.
- Files touched: `MEMORY.md`, `LOG.md`.
- Notes: This was added after the user corrected repeated accidental publication of Part 7 ingest previews. Future commit checks should verify preview files remain ignored (`!!`) rather than staged.

## [2026-06-17] lint | Wiki structure knowledge logic workflow check

- Summary: Ran a wiki-level structure, knowledge, logic, and workflow check focused on stale overview/domain-map evidence, overlapping content ownership, and durable future-ingest behavior.
- Files touched: `AGENTS.md`, `wiki/overview/domain_map.md`, `wiki/workflows/ingest_source.md`, `wiki/workflows/lint_wiki.md`, `wiki/workflows/query_wiki.md`, `wiki/commands/README.md`, `wiki/commands/ingest_source.md`, `wiki/commands/lint_wiki.md`, `outputs/lint_reports/2026-06-17_wiki_structure_knowledge_workflow_check.md`, `INDEX.md`, `MEMORY.md`, `LOG.md`.
- Notes: Added knowledge ownership boundaries and a living overview/synthesis maintenance rule. Future ingests must update affected overview/synthesis/reference-plan/workflow/index/memory pages or log an explicit deferral. `domain_map.md` now acts as a compact evidence map and routing page instead of a stale partial evidence list.

## [2026-06-17] lint | Cleared stale part-based workflow residue

- Summary: Consolidated stale and redundant part-based planning language left from the older staged-ingest workflow into current-state source-status and boundary notes.
- Files touched: `wiki/references/cg_system_core_reference_plan.md`, `MEMORY.md`, `INDEX.md`, `outputs/lint_reports/2026-06-17_wiki_structure_knowledge_workflow_check.md`, `LOG.md`.
- Notes: Removed duplicate pre-ingest/completed-source sections for already integrated SCI and cancer caregiver branches, kept the source 22/source 27 background-only boundaries, and removed the duplicate `domain_map.md` entry from the initial conceptual-page list.

## [2026-06-17] lint | Deep overview conflict compliance check

- Summary: Ran a deep scan of overview, synthesis, reference-plan, workflow, command, memory, index, evidence, and topic pages for old workflow contamination and knowledge conflicts.
- Files touched: `wiki/overview/domain_map.md`, `wiki/overview/caregiver_system_core_sota_synthesis.md`, `wiki/evidence/bressan_2020_dementia_caregiver_needs_mixed_method_review.md`, `INDEX.md`, `MEMORY.md`, `outputs/lint_reports/2026-06-17_deep_overview_conflict_compliance_check.md`, `LOG.md`.
- Notes: Converted `domain_map.md` from a partial evidence map into a routing/governance page, removed remaining current-state `part` wording from memory and Bressan evidence, and found no direct knowledge conflicts around source 22/source 27 boundaries, aging-vs-disease, AI evidence, smart-home effectiveness, or mHealth effectiveness claims.
