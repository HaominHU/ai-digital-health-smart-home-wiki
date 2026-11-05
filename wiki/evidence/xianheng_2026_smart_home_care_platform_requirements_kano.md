---
title: "Research on requirements for smart home-based older adult(s) care service platforms based on the Kano model"
type: "evidence_summary"
status: "ready"
privacy: "private"
source_id: "2026-10-20_xianheng_smart-home-care-platform-requirements-kano"
source_file: "sources/papers/monthly_pubmed/smart_home_and_ambient_care/2026-10-20_xianheng_smart-home-care-platform-requirements-kano.pdf"
source_lane: "monthly_pubmed"
ingest_month: "2026-11"
source_id_date_basis: "electronic_publication_date"
publication_date: "2026-10-20"
reference_item: "wiki/references/items/2026-10-20_xianheng_smart-home-care-platform-requirements-kano.md"
evidence_type: "published evidence"
source_type: "exploratory mixed-methods requirements study with retrospective case alignment"
evidence_role: "Provides exploratory multi-stakeholder requirements for smart-home care platforms, including family interest in service-status visibility. Numerical sensitivity rankings, category tallies, and age-bin definitions have internal inconsistencies and should not determine firm design priorities."
tags: ["smart-home", "older-adults", "requirements", "Kano", "care-coordination", "reporting-caveats"]
last_updated: "2026-11-05"
reporting_caution: "Internal sensitivity-score, category-count, and age-bin inconsistencies; avoid quantitative priority claims."
---

# Research on requirements for smart home-based older adult(s) care service platforms based on the Kano model

## Source Role

Provides exploratory multi-stakeholder requirements for smart-home care platforms, including family interest in service-status visibility. Numerical sensitivity rankings, category tallies, and age-bin definitions have internal inconsistencies and should not determine firm design priorities.

## Study Picture

- Qualitative item generation involved eight interviewees: five adult-child family caregivers and three front-line service staff. Subsequent questionnaires yielded 506 valid older-adult responses, plus simplified questionnaires from 58 family caregivers and 41 service providers.
- The older-adult sample was urban, community-dwelling, aged at least 65, and required basic smartphone operation and independent questionnaire comprehension. Bedridden people, those unable to complete the survey because of severe cognitive impairment/dementia, and people with no smartphone-operation ability were excluded. Only 27 participants were in the reported oldest age category.
- Nineteen requirements cover user, service, and environment dimensions. The qualitative material highlights emergency response, service-status transparency, operational simplicity, and service-dispatch information. Older-user and family/professional perspectives should remain separate rather than merged into one universal priority list.
- The authors report age/living-arrangement/education differences and family-caregiver preference for service-status visibility. Their proposed Creation-Analysis-Application model was retrospectively aligned with four deployed platform cases, reporting 17/19 item matches. This is case alignment, not prospective validation of outcomes, safety, reliability, or causal design benefit.

## Numerical Reporting Caveats Verified in the PDF

The following are source inconsistencies, not extraction artifacts; Tables 1 and 3 were visually inspected.

1. **Sensitivity formula and values disagree.** The text defines `S = (abs(Better) + abs(Worse)) / 2`. For daily care (U1), Table 1 gives Better=0.509 and Worse=-0.601, implying S=0.555 under that formula, but prints S=0.788. Efficient service (U4) similarly implies 0.6165 from 0.691 and -0.542 but prints 0.878. These are arithmetic consistency checks, not a reanalysis or a substitute corrected ranking. Do not export the printed sensitivity ranks as validated priorities.
2. **Category counts disagree.** The abstract reports 8 Must-be, 4 One-dimensional, 5 Attractive, and 2 Indifferent items; Section 3.2.2 reports 7/4/6/2. Counting Table 1's printed labels yields 8/4/4/3. Some discussion refers to stakeholder reclassification, but the presented summaries do not provide a single consistent tally. Preserve that uncertainty rather than choosing a preferred count.
3. **Age bins vary across sections.** Table 2 prints 65-70, 71-80, and 80+; other analyses describe 65-69, 70-79, and 80+. Do not infer exact subgroup boundaries or replicate subgroup tests from these inconsistent labels.
4. The main tables do not provide the full subgroup contingency data or the advertised bootstrap intervals needed to independently verify all tests and precision claims. No quantitative willingness-to-pay or affordability items were collected, despite some discussion implying payment-related priorities.

## Evidence Limits and Interpretation

Use this source as exploratory requirement-elicitation and stakeholder-perspective evidence, subject to the reporting caveats above. Do not use exact sensitivity scores, uncertain category totals, subgroup p-values, inferred aging trajectories, or unmeasured willingness-to-pay claims as firm design requirements. Cross-sectional differences are not evidence that an individual's preferences change because of aging. Exclusion of dementia/nonusers precludes direct dementia requirements or equitable coverage of all older adults.

**Design interpretation:** qualitative needs inform smart-home technology, coordination, monitoring, supported use, privacy, and modular-design questions. Privacy and access protection remain requirements even when a preference questionnaire labels an item indifferent. Technical support, fault reporting, and human response workflows are design proposals to evaluate, not observed effectiveness results.

PDF locators: Table 1 and eligibility p. 3; sample and age bins p. 4; Table 3 and formula p. 5; case alignment/limits pp. 6-7.

## Source Availability and Review

The publisher PDF is preserved locally with its verified SHA-256 hash in the local intake metadata. Supplementary files were not comprehensively retrieved. The article was integrated after explicit approval of the November batch preview on 2026-11-05. Raw sources remain local-only and may be absent after cloning. Bibliographic citation memory belongs in `wiki/references/items/2026-10-20_xianheng_smart-home-care-platform-requirements-kano.md`.

## Related Pages

- `wiki/technologies/smart_home_technologies.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/caregiving_challenges/monitoring_and_safety_awareness.md`
- `wiki/concepts/digital_inclusion_and_supported_use.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`
- `wiki/populations/older_adults.md`
- `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`
