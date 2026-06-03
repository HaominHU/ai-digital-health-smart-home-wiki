---
title: Biomarker-Stratified Neurorehabilitation
type: design_pattern
status: draft
privacy: private
evidence_status: has_sources
tags: [neurorehabilitation, biomarkers, trial-stratification, chronic-conditions, disability, ai-digital-health]
last_updated: 2026-06-03
---

# Biomarker-Stratified Neurorehabilitation

## Pattern Summary

Use baseline brain-health, systemic-health, sensory, and imaging markers to contextualize rehabilitation needs, stratify trials, and interpret recovery trajectories for people with chronic conditions and disabilities.

## Source-Backed Rationale

- `2026-06-03_fridriksson_brain-health-aphasia-recovery`: Lecture notes frame aphasia recovery as shaped by upstream vascular, metabolic, and sensory health; structural brain-health markers such as Brain Age Gap and white matter hyperintensities; network mechanisms such as disconnection and controllability; and the stroke lesion pathway.

## Design Moves

- Capture routine clinical biomarkers at rehabilitation intake, including blood pressure, pulse pressure, glucose or diabetes status, and hearing status when relevant.
- Reuse existing clinical imaging where appropriate, such as documenting white matter hyperintensity burden or Fazekas scoring on the lesion-free hemisphere.
- Treat brain-health profiles as context for rehabilitation planning, trial stratification, and outcome interpretation rather than as deterministic predictions.
- Track acute, subacute, and chronic trajectories so structural brain-health changes can be compared with behavioral recovery.
- Keep prediction, causal inference, and intervention recommendations separate in analytics and reporting.

## Privacy, Equity, and Safety Concerns

- Biomarker and imaging profiles are sensitive health data and require data minimization, consent, access control, secure storage, auditability, and clear retention rules.
- Stratification tools should be monitored for bias and should not be used to deny rehabilitation access or label patients as non-responders without human review and validated evidence.
- Comorbidities such as diabetes, hypertension, and hearing loss should be treated as support needs and trial-design variables, not as grounds for blame or exclusion.

## Evidence Limits

- Current support in this wiki is lecture-note level.
- The pattern needs source-backed literature before being used as a manuscript claim, clinical protocol, or deployed decision-support requirement.

## Related Pages

- `wiki/evidence/fridriksson_2026_brain_health_aphasia_recovery.md`
- `wiki/populations/people_with_chronic_conditions_and_disabilities.md`
- `wiki/care_recipient_needs/self_management_and_secondary_complication_prevention.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/research_questions/biomarker_stratified_neurorehabilitation.md`
