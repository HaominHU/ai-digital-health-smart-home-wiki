---
title: Ingest Preview - Preferences Towards Digital Health Technologies
type: ingest_preview
status: approved_integrated
privacy: private
source_id: 2026_kingsada_preferences-digital-health-technologies
source_file: sources/papers/monthly_pubmed/kingsada_2026_preferences_dh_scope_review.pdf
evidence_type: published evidence
source_type: scoping review
source_lane: monthly_pubmed
last_updated: 2026-06-04
---

# Ingest Preview: Preferences Towards Digital Health Technologies

## Review Status

Approved by user and integrated into the wiki on 2026-06-04.

This source is part of the monthly PubMed paper lane. It is separate from the `cg_system_core` staged caregiver system-design ingest.

## Source Context

- Source title: Preferences Towards Digital Health Technologies: a Scoping Review
- Authors: Aimee Kingsada; Silvana Briones-Piedrafita; Thomas Rapp; Jonathan Sicsic
- Journal: Health Economics Review
- Publication year: 2026
- Publication status: Article in press / accepted manuscript
- Received: 2025-12-08
- Accepted: 2026-05-19
- DOI: `10.1186/s13561-026-00792-2`
- Source type: Scoping review
- Evidence type: Published evidence
- Source file: `sources/papers/monthly_pubmed/kingsada_2026_preferences_dh_scope_review.pdf`
- Privacy sensitivity: No PHI or identifiable participant data detected in the extracted text.
- Readability: PDF text extraction is readable with Ghostscript. The extracted text has some accepted-manuscript artifacts but the main content is clear.

## Original Citation

Kingsada A, Briones-Piedrafita S, Rapp T, Sicsic J. 2026. Preferences towards digital health technologies: a scoping review. Health Economics Review. doi:10.1186/s13561-026-00792-2.

## Evidence-Backed Extraction

This scoping review synthesizes patient preferences for digital health technologies, including eHealth, telehealth, telemedicine, and mHealth. It is best used as broad patient-preference, digital-health adoption, and health-economics/HTA design evidence rather than caregiver-specific evidence.

Primary evidence roles:

- Broad digital health preference evidence across patient populations.
- Preference-elicitation methods anchor for DCE, conjoint analysis, best-worst scaling, contingent valuation, qualitative interviews, focus groups, and mixed methods.
- Design rationale for usability, personalization, affordability, privacy, data security, convenience, hybrid care, and face-to-face fallback.
- Older-adult digital health adoption context, especially for chronic condition management.
- HTA and reimbursement rationale for incorporating patient preferences into digital health assessment.

Key source-backed points:

- The review followed PRISMA-ScR guidance but did not register a protocol because the authors framed it as a scoping review rather than a systematic literature review.
- Searches covered PubMed, EMBASE, CINAHL, Scopus, and Web of Science for literature published from 2000 to 2026.
- The review focused on peer-reviewed English-language studies and excluded grey literature, commentaries, editorials, protocols, and conference abstracts.
- The database search identified 2,419 records; after duplicate removal and screening, 85 studies met inclusion criteria.
- Included studies comprised 27 qualitative studies, 45 quantitative studies, and 13 mixed-methods studies.
- Included study publication years ranged from 2005 to 2026, with 60% published from 2022 to 2026.
- Quantitative studies most often used attribute-based preference methods; discrete choice experiments were the dominant method.
- Six quantitative studies used contingent valuation to estimate willingness to pay for digital health technologies.
- Qualitative studies most often used interviews and focus groups, with thematic, deductive, inductive, and mixed analytic approaches.
- Studies addressed broad DHT characteristics as well as condition-specific contexts; common clinical areas included mental health, cardiology, dermatology, arthritis, cancer, neurological disorders, sexual and reproductive health, asthma, diabetes, HIV, prenatal care, rheumatic diseases, addiction, and chronic diseases.
- DHT categories included mHealth, telehealth, telemedicine, and eHealth; mHealth was the most frequently studied category.
- Recurring preference domains included cost, privacy, time management, convenience, ease of use, utility, data security, personalization, interaction with clinicians, feedback, and hybrid digital/in-person models.
- Older-adult preference evidence was limited but suggested that older adults often value simple, clearly explained, tailored tools, multimodal education, initial face-to-face interaction, privacy, comfort, and clinical support.
- The review cautions that preferences vary by DHT type, health condition, age, user group, national reimbursement context, and healthcare-system setting.

## Review-Level Takeaway

This paper is useful to the wiki as a broad preference-method and adoption-friction map for digital health technologies. Its core contribution is not showing that DHTs are effective, but showing which DHT attributes patients tend to value and how preference evidence has been elicited across health economics, digital health, and HTA-oriented studies.

For future patient-facing or caregiver-adjacent digital health design, the source supports a practical principle: DHTs should not be treated as acceptable just because they are technically available. Preference-sensitive design should account for cost burden, privacy and data security trust, convenience, personalization, ease of use, clinician connection, and the option to combine digital support with in-person care.

## Proposed Wiki Updates

Recommended new pages after approval:

- `wiki/evidence/kingsada_2026_preferences_digital_health_technologies.md`
- `wiki/references/items/2026_kingsada_preferences-digital-health-technologies.md`

Recommended updates to existing pages:

- `wiki/technologies/ai_driven_digital_health.md`: Add patient-preference and HTA-oriented digital health adoption evidence, while keeping it separate from AI-specific evidence.
- `wiki/populations/older_adults.md`: Add older-adult preference context for simple, tailored, clearly explained, privacy-sensitive digital tools with face-to-face support when needed.
- `wiki/design_patterns/accessibility_first_mhealth_symptom_reporting.md`: Add preference rationale for ease of use, multimodal education, and technical barrier reduction, bounded to patient-facing DHTs.
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`: Add only cautious design rationale about preference-sensitive personalization and hybrid support; do not treat this as caregiver evidence.
- `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`: Add preference-elicitation methods as optional design/evaluation rationale for digital health interventions, especially DCE, best-worst scaling, conjoint analysis, contingent valuation, and mixed methods.
- `wiki/research_questions/caregiver_intervention_implementation_and_evaluation.md`: Add a question about how patient/care-recipient preference elicitation should inform caregiver-facing or shared-access digital health design without conflating caregiver and care-recipient preferences.
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`: Add a caution that patient DHT preferences should not be assumed to equal caregiver preferences, especially in shared-care or proxy-use systems.

## Conditions and Population Handling

Direct mapping:

- Broad patient-facing digital health technologies.
- Older adults as a preference-relevant subgroup when studies specifically address age, chronic condition management, telehealth, mHealth, or face-to-face support preferences.

Cautious or indirect mapping:

- Family caregiving: indirect only. The source is about patient preferences for DHTs, not family caregiver needs or caregiver intervention outcomes.
- Chronic conditions: broad context only unless specific included studies are later ingested.
- Dementia, spinal cord injury, gynecological cancer, postpartum women, systemic sclerosis-associated Raynaud phenomenon, and falls: do not map as condition-specific evidence unless a specific included study is separately ingested and supports that condition.

Do not use this source as evidence that digital health technologies are clinically effective, that AI agents are safe/effective, or that smart-home systems improve outcomes.

## Gaps and Cautions

- This is a scoping review of preferences, not an intervention-effectiveness review.
- Patient preferences are not the same as caregiver preferences, clinician preferences, or care-recipient outcomes.
- Preference heterogeneity is substantial across DHT type, condition, age, healthcare system, and reimbursement context.
- The review excludes grey literature, non-English studies, conference abstracts, protocols, commentaries, and editorials.
- The review does not formally appraise qualitative study quality.
- Cost findings are difficult to compare because payment vehicles and cost perspectives vary across studies.
- Preference evidence should not be treated as universally transferable across countries because reimbursement, regulation, infrastructure, and care models shape patient experience.
- Older-adult conclusions are relevant but limited because only a small number of included studies had average participant age over 60.
- The source supports research, design, HTA, and knowledge support; it does not support clinical decision-making.

## Citation Memory Preview

- RIS export-ready: yes.
- Missing bibliographic fields: final volume, issue, and page/article number are not available from the article-in-press manuscript.
- Writing roles: patient-preference evidence; digital health adoption rationale; HTA/reimbursement rationale; preference-elicitation methods; older-adult digital health accessibility and trust rationale; privacy/security design rationale.

## Proposed Integration Boundary

If approved, integrate this source as a monthly PubMed broad digital-health preference source. Do not merge it into the `cg_system_core` staged caregiver-system citation sequence.
