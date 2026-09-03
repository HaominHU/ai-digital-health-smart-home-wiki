---
title: "Co-Design and Development of Digital Health Solution for Informal Alzheimer's Caregivers"
type: evidence_summary
status: ready
privacy: private
source_id: 2026-08-27_almeida_alzcare-dementia-caregiver-app
source_file: sources/papers/monthly_pubmed/caregiving_support_systems/2026-08-27_almeida_alzcare-dementia-caregiver-app.pdf
source_lane: monthly_pubmed
reference_item: wiki/references/items/2026-08-27_almeida_alzcare-dementia-caregiver-app.md
evidence_type: published evidence
source_type: mixed-methods needs assessment and prototype usability study
tags: ["dementia","caregivers","mhealth","co-design","usability"]
last_updated: 2026-09-03
---

# Co-Design and Development of Digital Health Solution for Informal Alzheimer's Caregivers

## Source Role

AlzCare adds integrated dementia caregiver app design and short-term usability evidence. Its contribution is a needs-informed prototype, not demonstrated caregiver or care-recipient benefit.

## Study and System Picture

- A needs assessment combined an online questionnaire and six semistructured interviews with professionals experienced in Alzheimer care.
- Sixty-eight questionnaire responses were collected; 52 were included after excluding 16 people without Alzheimer-disease contact. The included group contained eight current caregivers, eight former caregivers, and 36 family members of people with Alzheimer disease.
- AlzCare was developed as a React Native/Expo app with Firebase. Its five modules were Home, Tasks, Exercises, Patient Profile, and Caregiver Hub.
- Proposed functions included reminders, daily routine and health tracking, cognitive exercises, clinical/personal information storage, abnormal-value flags, location/geofencing alerts, reminiscence through the "Who Am I?" feature, caregiver resources, and three versions of the Zarit Burden Interview with automated scoring and history.
- Twenty-five participants evaluated the app through task-based interaction, interviews, and the System Usability Scale: 11 "common users" and 14 health-care experts. Only seven were current or former caregivers; 24 of 25 rated their technology comfort at 4 or 5 on a five-point scale. Eighteen sessions were in person, while seven remote sessions used researcher demonstration by screen sharing.

## Main Findings

- Recurring needs involved daily task management, health and safety monitoring, cognitive stimulation, caregiver support, simplicity, customization, and adaptation to disease progression.
- Mean SUS was 90.9, categorized by the authors as "Best Imaginable."
- Participants valued centralized care organization, cognitive activities, caregiver burden self-monitoring, and the shared reminiscence feature.
- Manual data entry, digital literacy, small icons, ambiguous controls, insufficient automation, and lack of implemented real-time physiological and geolocation functions were identified as limitations or future work.
- Divergent views about independent care-recipient use suggest that the app may function more realistically as a caregiver-supported dyadic tool, especially as dementia progresses.

## Evidence Limits and Safety Boundaries

- The study supports design relevance and perceived usability in a short, simulated evaluation; it does not establish sustained use, caregiver benefit, care-recipient benefit, clinical validity, safety, or effectiveness.
- The evaluation sample was highly digitally confident and contained more professionals than current/former caregivers. People living with dementia were not clearly represented as evaluators.
- Remote sessions were demonstrations rather than equivalent hands-on use, weakening comparability across evaluation modes.
- Some described capabilities, including location tracking and automated physiological data, were not implemented. Feature descriptions must be separated from validated functionality.
- The paper gives only high-level claims about secure storage and real-time synchronization. It does not provide enough evidence to endorse Firebase configuration, consent, access controls, retention, auditability, or protection of location and clinical data.
- Abnormal-value flags, caregiver-burden scoring, and geofencing require explicit escalation, consent, false-alarm, non-alert, and human-review safeguards before any clinical or real-world use.

## Wiki Interpretation and Design Implications

Separate planned sensing and location features from tested functionality. Centralizing care tasks, cognitive activities, and caregiver self-monitoring is a design option; whether this reduces workload or improves outcomes requires real-world longitudinal evaluation with actual caregivers and people living with dementia.

These implications support research and design, not diagnosis, treatment recommendations, or autonomous care decisions.

## Related Pages

- `wiki/conditions/dementia.md`
- `wiki/design_patterns/one_stop_caregiver_support_app.md`
- `wiki/caregiving_challenges/caregiver_self_care_and_health_tracking.md`
- `wiki/references/items/2026-08-27_almeida_alzcare-dementia-caregiver-app.md`

## Source Citation

Almeida MM, Fernandes CS, Campos Ferreira M. Co-Design and Development of Digital Health Solution for Informal Alzheimer's Caregivers. Alzheimer Disease and Associated Disorders. Published online August 27, 2026. doi:10.1097/WAD.0000000000000740. PMID: 42657604.
