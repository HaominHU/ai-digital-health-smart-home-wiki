---
title: Smart Home Technologies
type: technology
status: draft
privacy: private
evidence_status: has_sources
tags: [smart-home, sensing, caregiving, technology-lens]
last_updated: 2026-05-28
---

# Smart Home Technologies

## Scope

Primary technology focus for the wiki.

## Intended Support Role

Smart home technologies may support monitoring, safety, automation, communication, environmental fit, and caregiver awareness, depending on the source and context.

## Privacy, Security, and Safety Concerns

Track privacy in the home, consent among multiple household members, passive sensing risks, re-identification, data retention, access control, and false reassurance.

## Evidence

- `2026-05-18_hu_dissertation-family-caregiver-mhealth-app`: The dissertation identifies web cameras, GPS, sensors, and intelligent agents as technologies relevant to smart home care and caregiver monitoring/support. Co-design participants also raised concerns about smart home device cost, learning curve, insufficient support, and reliability.
- `2016_nasem_families-caring-for-an-aging-america`: The report identifies assistive technologies, remote monitoring and sensing systems, telehealth applications, and tools linked to health and social service providers as innovation targets for caregiving families.
- `2020_schulz_family-caregiving-for-older-adults`: The review supports technology as a caregiver support route for training, monitoring, and performance support, while emphasizing access, accessibility, reliability, and integration concerns.
- `2001_glasgow_re-aim-framework-chronic-illness-management`: RE-AIM supports evaluating smart-home interventions by who they reach, which homes or care systems adopt them, whether implementation is consistent, and whether operation is maintained over time.
- `2023_yao_react-reasoning-acting-language-models`: ReAct can inform speculative reasoning-plus-action orchestration patterns, but should not be used to justify autonomous home actions or safety-critical automation.
- `2025-12-30_malhotra_carebuddy-mobile-care-ecosystem-dementia-caregiving`: CareBuddy includes GPS location monitoring for wandering, Google Maps location display, navigation to last detected location, and battery reminders; this supports location-safety design rationale, not proof of safety effectiveness.

## Design Implications

- Treat smart home and intelligent-agent support as part of a broader caregiver support ecosystem, not only as passive monitoring.
- Include cost, setup burden, learning curve, reliability, and multi-user consent in smart home caregiving design.
- Do not cite these general caregiving sources as proof of smart home effectiveness; use them for design rationale and implementation concerns until technology-specific studies are ingested.
- Use RE-AIM-style questions to test whether smart-home systems are accessible, adoptable, maintainable, and feasible in routine home contexts.
- If AI agents interact with smart-home devices, constrain actions through explicit permissions, audit logs, human confirmation, and emergency boundaries.
- Treat GPS/location monitoring as privacy-sensitive care-recipient data requiring consent, role boundaries, access control, and clear escalation expectations.
