---
title: Monitoring and Safety Awareness
type: caregiving_challenge
status: draft
privacy: private
evidence_status: has_sources
tags: [monitoring, safety, caregiving]
last_updated: 2026-09-03
---

# Monitoring and Safety Awareness

## Challenge Summary

Reusable caregiving challenge hub for awareness of safety, risk, daily status, and changes over time.

## Caregiver Need

- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`: Vigilance demands are part of why caregiving can function as chronic stress, especially when ongoing supervision is required.
- `2020_schulz_family-caregiving-for-older-adults`: Caregivers may monitor care-recipient functioning, symptoms, medications, behavior, and location as needs increase across the care trajectory.
- `2016_nasem_families-caring-for-an-aging-america`: Safety risks can emerge when there is a mismatch between caregiver capacity and older-adult health needs or circumstances.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`: SCI caregivers in Ghana performed hands-on care tasks such as turning, toileting, diaper changes, bowel/bladder-related support, feeding, grooming, and transport.
- `2016_smith_caregiving-services-sci-systematic-review`: SCI caregiving service interventions included training and health-maintenance education with preliminary knowledge gains for secondary health conditions, respiratory complications, spasticity, autonomic dysreflexia, aging effects, and community services.
- `2019_conti_secondary-conditions-caregiver-burden-sci`: SCI secondary conditions such as bladder dysfunction, UTIs, pressure injuries, and chronic pain were associated with caregiver burden dimensions, making monitoring and prevention routines caregiver workload issues as well as care-recipient health issues.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes GPS location monitoring for wandering, Google Maps display of the last detected location, navigation to the tracked location, and battery reminders for the tracker.
- `2010_gitlin_cope-dementia-home-based-intervention`: COPE included home safety, patient capability assessment, medication review, and screening for treatable medical conditions, supporting safety awareness without relying on passive sensing.
- `2026-06-24_zhai_smart-home-technologies-ageing-in-place`: A smart-home systematic review found that monitoring, functional/emergency detection, and safety functions can support aging in place and caregiver/family reassurance, but heterogeneous evidence and implementation barriers limit broad effectiveness claims.

## Care Recipient Connection

Monitoring can support safety and unmet-need detection, but it can also affect privacy, autonomy, dignity, and the care recipient's relationship with caregivers.

## Technology Support Lens

Smart home, remote monitoring, sensing, telehealth, and caregiver-facing digital tools may support awareness and coordination, but effectiveness and safety claims require technology-specific evidence.

- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: GPS monitoring is a dementia-specific safety feature in CareBuddy, but the source reports usability/acceptability rather than safety outcome effectiveness.

## Implemented Versus Proposed Monitoring

AlzCare describes abnormal-value flags and geolocation-related support, but real-time physiological and location functions were not implemented in the evaluated version. Do not represent planned functions as tested safety systems. Separate manual reports, sensor data, flags, and human response; validate false alerts, missed alerts, non-alert meaning, consent, and response ownership before deployment. See `wiki/evidence/almeida_2026_alzcare_dementia_caregiver_app.md`.

## Evidence

- `2020_schulz_family-caregiving-for-older-adults`.
- `2008_schulz-sherwood_physical-mental-health-effects-family-caregiving`.
- `2016_nasem_families-caring-for-an-aging-america`.
- `2023-04-21_mohammed_sci-family-caregiver-experiences-ghana`.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`.
- `2010_gitlin_cope-dementia-home-based-intervention`.
- `2016_smith_caregiving-services-sci-systematic-review`.
- `2019_conti_secondary-conditions-caregiver-burden-sci`.
- `2026-06-24_zhai_smart-home-technologies-ageing-in-place`.
- `2026-07-23_fritz_community-in-the-loop-smart-home-monitoring`: A community-linked prototype converted 37 million readings into 4,719 alerts and 1,060 human contacts, while 93% required no action. Use as feasibility and workflow evidence, not diagnostic accuracy or effectiveness evidence; absence of an alert did not establish stability.
- `2026-07-15_pemberton_smart-home-connected-care-adoption`: Passive connected care may reduce repeated checking and provide reassurance, but adoption and responsibility are shared. Reliability, privacy, cost, dependency, and fail-safe behavior remain central.
- `2026-07-31_ding_wearable-healthcare-bibliometric-analysis`: Wearable-healthcare research increasingly connects monitoring with telemedicine, IoMT, EHRs, and AI, but bibliometric prominence does not establish sensing validity or clinical usefulness.

## Design Implications

- Assess caregiver capacity before assigning monitoring responsibilities.
- Separate safety awareness from surveillance.
- Include consent, auditability, and human escalation pathways.
- For location tracking, explicitly handle care-recipient consent, access permissions, data retention, and caregiver escalation expectations.
- For SCI secondary-condition support, separate caregiver/attendant knowledge and monitoring responsibilities from autonomous clinical decision-making.
- For SCI secondary-condition monitoring, track caregiver workload and burden dimensions rather than assuming more vigilance is always acceptable or beneficial.
- For smart-home alerts and monitoring, define who receives alerts, who is responsible for response, how false positives/negatives are handled, and whether the system reduces or increases caregiver vigilance burden.
- State what a non-alert means, who must respond, and when users should bypass the system for urgent help.
- Track `digital distress`, including irrelevant alerts, missed changes, intrusiveness, confusion, and unclear responsibility.
