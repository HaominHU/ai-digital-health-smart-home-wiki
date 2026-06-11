---
title: Caregiver System Core SoTA Synthesis
type: overview_synthesis
status: draft
privacy: private
evidence_status: source_backed_synthesis
tags: [caregiver-system-core, family-caregiving, digital-health, sota-synthesis]
last_updated: 2026-06-11
scope: cg_system_core
---

# Caregiver System Core SoTA Synthesis

## Purpose

This page is the living general-knowledge synthesis of the `cg_system_core` Tier 1 ingest. It is for the wiki owner as a research-state map: what the caregiver-system section currently knows, what should be kept in mind when citing the literature, and what design or research directions can be envisioned from the accumulated wiki.

This is not a clinical recommendation, treatment guide, grant section, manuscript section, or task-specific output. It should be revised after future relevant article ingests, especially when new caregiver intervention trials, implementation studies, AI-enabled caregiver systems, smart-home caregiving studies, or condition-specific evidence are added.

## Umbrella Frame

The current core evidence frames family caregiving as a chronic condition management problem that sits across individuals, dyads, households, care teams, and service systems. The caregiver is not only an informal helper. The caregiver may be a care coordinator, health-literacy translator, symptom observer, medication or treatment supporter, transportation manager, financial navigator, emotional support person, hands-on personal-care worker, backup system when formal services are thin, and a person with their own health risks.

Three distinctions should travel with this whole section:

- Caregiver outcomes, care-recipient outcomes, dyadic outcomes, utilization outcomes, and implementation outcomes are different constructs. Van Houtven et al. 2011 is the cleanest organizing framework for this distinction, while Glasgow et al. 2001 adds reach, adoption, implementation, and maintenance logic.
- Chronic caregiving can be a chronic stress exposure, but burden is not the only outcome. Schulz and Sherwood 2008, Schulz et al. 2020, NASEM 2016, and Aneshensel/Avison 2015 support a broad stress-process view that includes primary stressors, secondary role strain, coping resources, social support, mastery, appraisal, positive meaning, and health outcomes.
- Conditions are overlays, not interchangeable categories. Dementia is not normal aging; acquired SCI is not aging-related mobility decline; gynecological cancer is a disease condition that may be age-associated but is not itself an aging issue.

## Leading Outcomes of Family Caregiving

This section describes leading outcomes of being a family caregiver and providing care. These outcomes are not automatically intervention targets, and they should not be treated as evidence that a specific digital health intervention works. They describe what caregiving can do to caregivers, care recipients, dyads, and systems.

### Caregiver Health and Well-Being Outcomes

Family caregiving can affect psychological health, physical health, health behaviors, sleep, self-care, social life, and perceived quality of life. The recurring caregiver outcomes in the core include burden, depressive symptoms, anxiety or stress, physical fatigue or pain, disrupted health routines, reduced time for self-care, social isolation, caregiver confidence, preparedness, coping/problem solving, mastery, self-efficacy, and positive caregiving meaning.

Burden should be kept broad rather than reduced to one score. In the current core, burden can mean emotional strain, practical load, schedule disruption, financial pressure, physical care strain, vigilance, role captivity, or difficulty balancing caregiving with work and family life. Positive meaning and caregiver esteem can coexist with heavy practical burden, especially in advanced cancer and end-of-life caregiving.

### Role, Time, Financial, and Work-Life Outcomes

Caregiving changes roles and daily structure. Caregivers may become coordinators, hands-on care workers, health-information translators, symptom observers, transportation planners, medication supporters, appointment managers, household managers, insurance or financial navigators, and advocates. These roles can disrupt work, school, sleep, household routines, social participation, and personal health care.

Financial outcomes include direct care expenses, lost work time, reduced income, transportation costs, medication or equipment costs, insurance/benefits navigation, and the need for financial aid or advocacy resources. Hartnett 2016 and cancer caregiver sources make this especially visible, while SCI sources show how sudden injury can produce abrupt household and employment disruption.

### Caregiving Work and Process Outcomes

Caregiving itself produces process-level outcomes: the ability to monitor symptoms, coordinate appointments, manage information, perform or supervise care tasks, communicate with clinicians, respond to behavior or symptom changes, navigate formal services, and maintain routines over time. These process outcomes describe the quality and sustainability of care work.

Process outcomes matter because family caregivers often carry work that would otherwise fall to formal systems. When a caregiver lacks training, information, time, respite, or coordination support, the quality of care work can become fragile even before a clinical outcome changes.

### Care-Recipient and Dyadic Outcomes

Family caregiving can affect care recipients through practical support, symptom observation, treatment or medication support, daily function support, secondary-complication prevention, safety awareness, behavioral symptom response, appointment preparation, and help staying in the home or desired community setting. These are not automatically positive: support can also create dependency, privacy loss, conflict, unwanted surveillance, or reduced care-recipient autonomy if boundaries are poorly handled.

Dyadic outcomes include shared care planning, communication quality, trust, mutual adjustment, patient-caregiver boundary management, controlled sharing, and conflict or role strain. The dyadic layer is especially important for dementia, SCI, and gynecological cancer because caregiver support often intersects with care-recipient identity, autonomy, dignity, and sensitive health information.

### System and Service Outcomes

Family caregiving also has health-system and service-level consequences. Caregivers can support home-based care, clinic preparation, symptom documentation, treatment follow-through, resource navigation, and reduced fragmentation. At the same time, systems can shift substantial hidden labor onto families without identifying, training, assessing, or supporting caregivers.

System outcomes to track include caregiver identification, caregiver assessment, service navigation, formal/informal care mix, care hours, use of respite, provider communication, care transitions, healthcare utilization, cost, and whether caregiver support is actually reachable and maintainable in routine care.

## Informed Intervention Design

The outcomes above inform intervention design, but they should not be collapsed into intervention effects. The safer logic is: first identify what caregiving changes; then identify which mechanism might plausibly support which outcome; then test whether the intervention actually changes that outcome.

Dementia meta-review evidence, especially Cheng 2020 and Walter/Pinquart 2020, supports outcome-matched intervention logic: depression may be more consistently modifiable than burden, anxiety, or social support, and active caregiver participation often matters. SCI evidence similarly suggests that problem-solving style or coping resources can be meaningful intervention targets even when depression does not change. Cancer caregiver reviews show psycho-emotional, daily-functioning, social, practical, and financial outcome domains, but implementation readiness and population reach remain major constraints.

For the wiki owner's research, this means digital systems should be explicit about whether they are trying to improve a caregiver outcome, a caregiving process outcome, a care-recipient outcome, a dyadic outcome, or an implementation outcome. A system may improve information access, preparedness, documentation, or coordination without yet proving reduced burden, reduced hospitalization, or improved care-recipient safety.

Design implications:

- Match intervention mechanisms to outcomes instead of assuming all caregiver interventions should reduce global burden.
- Treat proximal changes such as knowledge, preparedness, mastery, coping, self-efficacy, or coordination as distinct from distal outcomes such as health status, utilization, safety, or sustained quality of life.
- Preserve dyadic ethics: caregiver support can become intrusive if it weakens care-recipient autonomy, over-monitors private behavior, or routes information to family members without consent and role clarity.
- Evaluate reach, adoption, implementation, and maintenance alongside caregiver and care-recipient outcomes.

Implementation outcomes include reach, representativeness, adoption, appropriateness, acceptability, feasibility, fidelity, delivery resources, cost, penetration, sustainability, and maintenance. RE-AIM and Proctor-style logic should sit next to caregiver outcome logic. Ugalde 2019 is especially useful here because it shows that cancer caregiver intervention studies often underreport adoption partners, staff training, eligible-caregiver reach, fidelity, delivery resources, and implementation cost.

The key citation habit: do not treat completion, satisfaction, usability, or acceptability as effectiveness. They are necessary, often valuable signals, but they answer a different question.

## Core Challenges Digital Health Responds To

The `cg_system_core` evidence repeatedly points to several reusable caregiver-system challenges.

- Information access and health literacy: caregivers need plain-language, trustworthy, timely, condition-specific information that changes across the care trajectory.
- Emotional and social support: caregivers need validation, coping support, peer connection, distress monitoring, and routes to human support.
- Problem solving and skill training: caregivers often need coaching, role training, task training, behavioral response strategies, and confidence-building.
- Care coordination and shared access: caregivers need reminders, shared records, role-based access, appointment preparation, provider communication, resource directories, and task coordination.
- Monitoring and escalation uncertainty: caregivers need help knowing what to observe, when to escalate, and how to document changing symptoms without replacing professional judgment.
- Time burden and engagement fatigue: caregivers often cannot explore complex apps, complete long modules, or sustain high-burden digital routines.
- Privacy, autonomy, and dyadic boundaries: family access, location monitoring, private caregiver spaces, and shared patient-caregiver spaces require granular controls.
- Implementation burden: caregiver interventions fail if they are not reachable, adoptable by services, maintainable, affordable, culturally usable, and compatible with workflows.

## Digital Health Intervention Landscape

### Telehealth and Remote Coaching

Telehealth has the strongest broad caregiver intervention base among digital modalities in the current core. Graven 2021 synthesizes RCTs across chronic conditions, with telephone, web, and combined delivery modes. In SCI, Elliott 2008 supports videoconference-delivered problem-solving support, while Elliott and Berry 2009 supports brief problem-solving plus education around recent-onset SCI transition. In dementia, Tele-Savvy supports online synchronous/asynchronous psychoeducation effects on depression, perceived stress, reactions to behaviors, and mastery.

Mechanism: remote access, repeated contact, coaching, psychoeducation, problem solving, and reduced travel burden.

Challenge response: geographically dispersed caregivers, transition-period uncertainty, limited access to in-person caregiver programs, and need for scalable skills training.

Boundary: telehealth delivery evidence is not AI evidence, smart-home evidence, or proof that all digital caregiver interventions are effective.

### mHealth and Modular Self-Management Support

mHealth evidence in the wiki spans care-recipient self-management infrastructure, caregiver-facing apps, and condition-specific formative design. Setiawan 2019 grounds adaptive mHealth infrastructure for people with chronic conditions and disabilities. Hu's dissertation extends that line toward family caregiver support through multi-component caregiver modules, self-care, training, reminders, resources, and shared-access logic. Campbell 2024 adds direct gynecologic cancer patient-caregiver formative mHealth design evidence.

Mechanism: modular education, reminders, self-monitoring, care coordination, tailored content, shared access, caregiver self-care support, and resource navigation.

Challenge response: fragmented caregiving tasks, changing needs over time, limited caregiver bandwidth, condition-specific information gaps, and dyadic sharing needs.

Boundary: formative design, feasibility, usability, and acceptability are not the same as effectiveness.

### Web-Based Psychoeducation and Skills Training

Dementia has the strongest tradition here. Savvy Caregiver supports manualized caregiver role training and transportability; COPE supports home-based dyadic training, environmental tailoring, activity support, and medical review; Tele-Savvy supports online delivery of dementia caregiver psychoeducation; REACH II/REACH VA add implementation and cost logic. Cheng 2020 and Walter/Pinquart 2020 synthesize this intervention family and caution against one-size-fits-all claims.

Mechanism: caregiver mastery, behavior response skills, environmental fit, confidence, role reframing, structured practice, and support from trained facilitators.

Challenge response: dementia behavioral symptoms, caregiver uncertainty, reduced mastery, stress, and home-management strain.

Boundary: dementia caregiver intervention evidence is caregiver or dyadic support evidence, not dementia disease-modification evidence.

### Peer, Group, and Advocacy-Ecosystem Support

Across conditions, caregivers need social support and resource navigation. In advanced cancer, Becque 2023 includes individual, dyadic/family, and group formats. Dave 2024 foregrounds patient advocacy groups as education, navigation, counseling, peer support, financial aid, and policy actors. Dementia sources also support peer forum and community logic, while SCI caregiver evidence points to social support, respite, system navigation, and future planning.

Mechanism: normalization, emotional support, practical knowledge exchange, service linkage, and advocacy.

Challenge response: isolation, low system literacy, financial or practical strain, and uncertainty about available help.

Boundary: advocacy and peer-support framing should not be overread as intervention-effectiveness evidence unless the source evaluates outcomes.

### Chatbots, RAG, and AI-Agent Architecture

The wiki now has two different AI evidence layers. First, caregiver-facing AI system evidence: Ruggiano 2021 reviews dementia chatbot functions and quality but does not show caregiver outcome effectiveness. CareBuddy sources provide dementia caregiver mHealth usability/acceptability and abstract-level multi-agent design evidence, not clinical effectiveness. Hu's abstracts and dissertation provide design rationale for generative AI as an adaptive support layer. Second, technical method sources: Lewis 2020 RAG and Yao 2023 ReAct are architecture references for retrieval-grounded generation and reasoning-plus-action orchestration.

Mechanism: source-grounded answers, structured task support, adaptive prompts, resource retrieval, conversational guidance, tool orchestration, and inspectable action paths.

Challenge response: information overload, resource lookup, pre-clinic preparation, caregiver task planning, and condition-tailored education.

Boundary: AI method papers are not caregiver evidence. RAG and ReAct justify possible architecture patterns, not clinical safety, caregiver effectiveness, equity, usability, or autonomous care.

### Smart-Home and Sensing-Relevant Support

Smart-home evidence is currently more design rationale than effectiveness evidence in the core. NASEM 2016 and Schulz 2020 identify remote monitoring, sensing, telehealth, assistive technology, and linked tools as caregiver-support opportunities. Hu's dissertation includes cameras, GPS, sensors, intelligent agents, and caregiver concerns around cost, setup burden, reliability, and learning curve. CareBuddy adds location monitoring for wandering as dementia caregiver mHealth design rationale.

Mechanism: passive or semi-passive awareness, location support, environmental fit, reminders, and linked caregiver notification.

Challenge response: safety awareness, wandering/location concern, secondary-complication routines, remote caregiver awareness, and care-recipient independence support.

Boundary: the core does not yet contain strong smart-home effectiveness evidence. Treat smart-home claims as design and implementation logic unless future smart-home-specific studies are ingested.

## Condition-Specific Synthesis

### Dementia and ADRD

Dementia is the deepest caregiver intervention branch in the current core. The evidence base is mature enough to support intervention taxonomy, needs taxonomy, outcome matching, and implementation questions.

Leading caregiver outcomes: depression, perceived stress, mastery, reaction to behavioral symptoms, burden, anxiety, quality of life, confidence, coping, and caregiver health. The strongest design lesson is not simply "reduce burden." It is to match intervention mechanisms to outcomes: skills training for mastery and response confidence, psychoeducation for knowledge and stress appraisal, home-environment tailoring for dyadic function, and implementation evaluation for reach and sustainability.

Digital modalities: online psychoeducation, synchronous/asynchronous training, mHealth care ecosystems, caregiver forums, care planning tools, provider messaging, RAG-supported chat, chatbot functions, GPS/location monitoring, and AI-agent design concepts.

What to cite:

- Cheng 2020 for dementia caregiver intervention synthesis and outcome-matching caution.
- Bressan 2020 for dementia caregiver needs at home: support, accessible personalized information, training to manage change, and balance.
- Walter/Pinquart 2020 for intervention taxonomy, small-to-moderate average effects, active participation, and heterogeneity.
- COPE, Savvy, Tele-Savvy, and REACH sources for signature intervention examples and implementation/economic dimensions.
- Ruggiano 2021 and CareBuddy sources for chatbot and AI-enabled design boundaries.

What to keep in mind: dementia is not normal aging. Dementia technology support must preserve care-recipient dignity, privacy, comprehension, and escalation boundaries. Chatbot availability, usability, or feature richness should not be cited as caregiver outcome effectiveness.

### Spinal Cord Injury

SCI evidence in the current core is strongest for caregiver role disruption, practical service structure, problem-solving support, secondary-condition burden mechanisms, coping, social support, unmet needs, and transition planning. The caregiver work is often hands-on, sudden, physically demanding, and tied to care-recipient function and secondary conditions.

Leading caregiver outcomes: burden dimensions, depression, dysfunctional problem-solving style, coping orientation, social support, unmet needs, well-being, caregiver physical symptoms, respite needs, and system-navigation strain.

Digital modalities: videoconference problem-solving training, brief PST plus education and follow-up, adaptive mHealth support for SCI self-management context, pre-clinic AI preparation as exploratory support, and design opportunities for secondary-condition routines, caregiver training, and resource navigation.

What to cite:

- Mohammed 2023 for context-specific qualitative evidence on sudden caregiver role entry, hands-on care, physical burden, financial strain, and coping in Ghana.
- Smith 2016 for SCI caregiving service structure, formal/informal care, care hours, functional predictors, and training gaps.
- Elliott 2008 and Elliott/Berry 2009 for SCI caregiver problem-solving intervention evidence, with attrition and mechanism limits.
- Conti 2019 for correlational burden links with secondary physical conditions and functional independence.
- Espino 2022 for coping, social support, unmet needs, respite, health red flags, and exploratory profiles.

What to keep in mind: SCI caregiver evidence should not be collapsed into general older-adult caregiving or dementia caregiving. Remote problem-solving evidence exists, but the intervention evidence is not a blanket endorsement of AI, smart-home, or autonomous care. Secondary-condition support is a dyadic design opportunity because care-recipient health routines can affect caregiver burden, but causal and effectiveness claims need stronger evidence.

### Gynecological Cancer and Broader Cancer Caregiving

The gynecological cancer branch now has one direct gynecologic cancer formative mHealth study, one end-stage ovarian cancer burden study, and broader cancer caregiver review evidence. This makes the branch usable for design rationale and need framing, but still weaker for gynecological-cancer-specific digital health effectiveness.

Leading caregiver outcomes: schedule disruption, financial strain, practical burden, positive caregiver esteem, psycho-emotional outcomes, daily functioning, social outcomes, information needs, communication needs, emotional needs, practical/financial needs, and implementation outcomes.

Digital modalities: formative mHealth self-management support, curated information, symptom-urgency self-triage support, private and shared dyadic spaces, granular sharing controls, expert/peer interaction, telehealth access, advocacy-resource linkage, and implementation-aware supportive intervention design.

What to cite:

- Hartnett 2016 for end-stage ovarian cancer caregiver burden, especially schedule disruption and financial problems alongside positive meaning.
- Campbell 2024 for direct gynecologic cancer patient-caregiver mHealth design needs.
- Ugalde 2019 for cancer caregiver intervention implementation readiness using Proctor outcomes.
- Becque 2023 for advanced cancer supportive-intervention taxonomy and outcome-domain mapping.
- Dave 2024 for broad cancer caregiver unmet-needs and patient advocacy ecosystem framing.

What to keep in mind: Campbell 2024 is formative qualitative design evidence, not mHealth effectiveness or autonomous triage evidence. Ugalde 2019 and Becque 2023 are broad cancer reviews, not gynecological-cancer-specific effectiveness anchors. Dave 2024 is a narrative review and advocacy ecosystem framing source, not a systematic review.

## Cross-Cutting State of the Research

The current state of the wiki suggests a caregiver system architecture that is condition-aware but not condition-siloed. Many caregiver challenges recur across conditions: information overload, task coordination, emotional strain, time burden, skill gaps, monitoring uncertainty, and fragmented services. But the reasons and design priorities differ by condition. Dementia emphasizes behavioral symptoms, supervision, mastery, and long trajectories. SCI emphasizes sudden disability, functional dependence, secondary complications, physical care, and transition/future planning. Gynecological cancer emphasizes treatment and symptom uncertainty, advanced illness, financial/practical strain, and dyadic information sharing.

The strongest evidence areas are broad caregiver burden and stress-process framing, dementia caregiver intervention taxonomy, dementia caregiver needs, telehealth delivery for caregivers, SCI caregiver service/burden/coping mechanisms, cancer caregiver implementation-readiness, and gynecologic cancer formative mHealth design needs.

The weaker evidence areas are AI-enabled caregiver effectiveness, smart-home caregiving effectiveness, long-term adoption and maintenance, equity and marginalized caregiver inclusion, implementation cost and workforce fit, and direct comparative evidence for adaptive or agentic caregiver systems.

Common overclaims to avoid:

- "Digital health works for caregivers" without naming modality, mechanism, population, and outcome.
- "Caregiver satisfaction means effectiveness."
- "AI method papers support clinical caregiver care."
- "Dementia caregiving evidence generalizes to all chronic conditions."
- "Cancer caregiver review evidence is gynecological-cancer-specific evidence."
- "Smart-home monitoring improves caregiver or care-recipient outcomes" without a smart-home-specific evaluated source.

## What This Enables for the Wiki Owner's Work

The current Tier 1 core supports a research agenda around adaptive caregiver-support systems that combine reusable caregiver architecture with condition-specific overlays.

Promising directions:

- A modular caregiver mHealth platform that separates general caregiver supports from condition-specific content and trajectory-sensitive modules.
- A RAG-supported caregiver knowledge layer that retrieves from curated, reviewed sources and exposes provenance rather than generating unsupported advice.
- A bounded agent layer for low-risk tasks such as appointment preparation, resource lookup, checklist generation, caregiver self-care prompts, and draft communication, with human confirmation before action.
- Dyadic privacy and sharing controls that allow patient-only, caregiver-only, shared, and clinician-facing spaces.
- Condition-aware assessment and triage logic that routes support by caregiver burden, task load, coping/problem-solving orientation, social support, secondary-condition risk, financial strain, and care trajectory.
- Implementation evaluation that measures reach, adoption partners, fidelity, delivery burden, cost, maintenance, and equity rather than stopping at usability or acceptability.

The owner's strongest near-term citation backbone for writing or design justification is:

- General caregiver system frame: Schulz/Sherwood 2008, Schulz 2020, NASEM 2016, Van Houtven 2011, Glasgow 2001.
- Digital caregiver intervention frame: Graven 2021, Zhai 2023, Hu dissertation, Setiawan 2019.
- Dementia intervention and needs frame: Cheng 2020, Bressan 2020, Walter/Pinquart 2020, COPE, Savvy, Tele-Savvy, REACH, Ruggiano 2021, CareBuddy sources.
- SCI caregiver frame: Mohammed 2023, Smith 2016, Elliott 2008, Elliott/Berry 2009, Conti 2019, Espino 2022.
- Cancer and gynecological cancer frame: Hartnett 2016, Ugalde 2019, Becque 2023, Campbell 2024, Dave 2024.
- AI architecture frame: Lewis 2020 and Yao 2023, used only as technical design rationale.

## Living Update Notes

Revise this page whenever a new relevant article changes the state of the caregiver-system core. Future updates should add evidence without flattening condition differences, overstating AI or smart-home effectiveness, or treating implementation outcomes as clinical outcomes.

Useful update triggers:

- New caregiver intervention trials, especially with long-term outcomes.
- New AI-enabled caregiver system evaluations with real caregiver or dyad outcomes.
- Smart-home caregiving studies with safety, privacy, adoption, or burden outcomes.
- Equity, accessibility, cultural tailoring, rural access, language access, and low-resource caregiver evidence.
- Implementation studies that report workforce, cost, fidelity, adoption, penetration, or maintenance.

## Related Wiki Pages

- `wiki/references/cg_system_core_reference_plan.md`
- `wiki/populations/family_caregivers.md`
- `wiki/conditions/dementia.md`
- `wiki/conditions/spinal_cord_injury.md`
- `wiki/conditions/gynecological_cancer.md`
- `wiki/technologies/ai_driven_digital_health.md`
- `wiki/technologies/smart_home_technologies.md`
- `wiki/concepts/caregiving_as_chronic_stress_exposure.md`
- `wiki/concepts/caregiving_activities_vs_outcomes.md`
- `wiki/concepts/reach_adoption_implementation_maintenance.md`
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`
- `wiki/design_patterns/caregiver_assessment_and_triage.md`
- `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
