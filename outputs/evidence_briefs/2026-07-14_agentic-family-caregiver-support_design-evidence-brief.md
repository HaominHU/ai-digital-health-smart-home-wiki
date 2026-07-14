---
title: Wiki-Inspired Evidence Brief for Next-Generation Agentic Family Caregiver Support
type: evidence_brief
status: ready
privacy: private
evidence_scope: maintained_wiki_only
source_project_reviewed: agentic-cg-support README concept and goals only
tags: [family-caregivers, agentic-ai, multi-agent-systems, digital-health, design-evidence]
created: 2026-07-14
last_updated: 2026-07-14
---

# Wiki-Inspired Evidence Brief for Next-Generation Agentic Family Caregiver Support

## Purpose

Inform the design of a multi-agent-coordinated family caregiver support backend using only knowledge already maintained in this wiki. This brief is a design-time evidence feed, not an ingest of the external project, a clinical specification, or proof that an agentic caregiver system is effective.

The external project is treated as read-only. At the time this brief was produced, only its `Concept & Goal` section had been read. The rest of that README is intentionally evaluated after this brief so the wiki can function as an independent inspiration source rather than merely rationalizing an existing design.

## Concept Being Informed

The proposed system has four defining ideas:

1. A multi-agent backend coordinates family caregiver support while a separate frontend provides the user interface.
2. The backend can be offered as an integrated, coordinator-first service or as smaller role-specific services.
3. A maintained Markdown AI-wiki informs design and development and may also serve as a runtime knowledge source.
4. A separate RAG implementation over the same content enables a comparative or complementary research question involving accuracy, empathy, and response structure.

## Bottom Line

The maintained wiki supports a **modular, condition-aware, caregiver-centered system with assessment, coordination, source-grounded information support, and tightly bounded actions**. It also supports using reusable caregiver functions with condition-specific overlays rather than building isolated systems for every diagnosis.

The wiki does **not** establish that a multi-agent implementation is superior to a single-agent or conventional service architecture. Direct multi-agent caregiver evidence is limited to an abstract-level CareBuddy study, while broader CareBuddy evidence supports a multicomponent ecosystem only at development, usability, acceptability, and short-term engagement levels. Agent boundaries should therefore be treated as testable software and interaction hypotheses, not evidence-established intervention components.

The wiki supports RAG as a technical source-grounding method but contains no direct empirical comparison between a human/LLM-navigated Markdown wiki and vector retrieval. The AI-wiki-versus-RAG study is therefore a legitimate research gap. It should compare controlled access strategies over the same versioned knowledge, not assume that either approach is inherently more accurate, empathetic, or useful.

## Evidence-to-Design Map

| Design question | What the maintained wiki supports | Evidence strength and boundary |
|---|---|---|
| Should support be integrated or modular? | Use a modular suite with general caregiver functions, reusable condition-aware interfaces, and condition-unique modules. An integrated experience may reduce fragmentation, but progressive disclosure is needed to avoid feature overload. | Strong design rationale from caregiver mHealth, digital-health, and intervention synthesis; limited effectiveness evidence for a one-stop digital product. |
| Should a coordinator route work across services? | Coordination is useful for fragmented tasks, changing needs, resource navigation, and role-aware sharing. A central orchestrator with specialized agents is technically plausible. | Care coordination is strongly supported as a need. Multi-agent orchestration itself has only early abstract-level caregiver-system evidence and technical-method rationale. |
| What should assessment do? | Identify the caregiver; assess risks, needs, strengths, preferences, capacity, willingness, digital access, care context, and support resources; then route to suitable information, training, services, or human escalation. | Strong assessment and intervention-matching rationale. Assessment must not become autonomous diagnosis or clinical triage. Exploratory profiles are not validated risk categories. |
| Should there be condition-specific agents? | Preserve reusable cross-condition caregiver challenges while applying condition and trajectory overlays. Dementia, SCI, and gynecological cancer require different priorities and must not be flattened into one caregiver model. | Strong synthesis-level rationale for condition awareness. Evidence does not require each condition to be implemented as a separate autonomous agent. |
| What should a knowledge function do? | Retrieve curated, versioned material; adapt it to literacy, role, condition, and trajectory; preserve provenance; state uncertainty and scope; and offer safe fallback or escalation. | Strong need and design rationale. Evidence for AI-generated caregiver education effectiveness remains weak. |
| What actions may an agent take? | Low-risk knowledge and workflow support: source lookup, resource navigation, appointment preparation, checklist generation, draft communication, reminders, and task tracking. | Bounded design rationale. External communication, data sharing, purchases, care-plan changes, device actions, or clinical escalation require explicit human confirmation and accountable ownership. |
| What must remain separate? | Caregiver needs, care-recipient needs, dyadic needs, implementation outcomes, and clinical outcomes. Private caregiver, private care-recipient, shared, and clinician-facing spaces need distinct permissions. | Strong conceptual and ethical requirement across the wiki. |
| What should evaluation measure? | Match each mechanism to proximal and distal outcomes; measure technical quality, user experience, caregiver workload, caregiver and care-recipient outcomes, safety, reach, adoption, implementation, maintenance, and cost separately. | Strong framework support. Usability, satisfaction, or completion must not be presented as effectiveness. |

## Design Principles the Evidence Supports

### 1. Organize around reusable caregiver challenges, then apply condition overlays

The system should not equate a diagnosis with a complete support pathway. Reusable functions include information access, care coordination, emotional and social support, problem solving, caregiver self-care, monitoring uncertainty, and resource navigation. Condition overlays should change content, risks, trajectory logic, and escalation context.

Examples from the maintained synthesis:

- Dementia emphasizes behavior response, supervision, mastery, long trajectories, respite, future planning, and dignity.
- SCI emphasizes sudden role entry, hands-on and physical care, secondary complications, functional dependence, training, coping, and transition planning.
- Gynecological cancer emphasizes treatment and symptom uncertainty, schedule and financial strain, curated information, expert or peer support, and granular dyadic sharing.

This supports condition-specific capabilities but not necessarily one LLM agent per disease. A condition service, ruleset, content pack, or specialist agent are alternative implementations that should be compared on reliability, maintainability, and user experience.

### 2. Treat the caregiver as a direct support recipient

The caregiver is not merely a proxy data source or operator for the care recipient. The system should directly support caregiver health, preparedness, skills, coping, self-efficacy, social support, time burden, and resource needs.

At the same time, caregiver support must not override care-recipient autonomy. Data models and workflows should separately represent:

- caregiver needs and preferences;
- care-recipient needs and preferences;
- dyadic or household decisions;
- role, consent, and sharing permissions;
- caregiver, care-recipient, dyadic, service, and implementation outcomes.

### 3. Make assessment multidimensional and routing-oriented

A defensible assessment function should capture more than a single burden score. Candidate domains include:

- primary care demands, vigilance, and task load;
- secondary work, family, financial, and social strains;
- caregiver physical and mental health;
- coping, problem-solving orientation, mastery, and positive meaning;
- social support, respite, and backup care;
- skills, preparedness, health literacy, and digital access;
- willingness, capacity, preferences, and privacy expectations;
- care-recipient function, behavior, symptoms, and condition-specific context;
- care trajectory and recent transitions.

Its output should be a transparent support plan or routing recommendation with the caregiver's confirmation. High-risk or urgent findings need a predefined human pathway. The agent should not silently convert assessment results into diagnosis, treatment advice, medication changes, or autonomous clinical escalation.

### 4. Use a coordinator to manage support continuity, not clinical authority

A coordinator can maintain task context, route requests, assemble outputs from specialist functions, preserve permissions, and show the user what happened. This is consistent with caregiver needs for reduced fragmentation and with bounded reasoning-action patterns.

The coordinator should not become an unreviewable super-agent. It needs:

- explicit routing rules and role contracts;
- minimum necessary context passed to each component;
- visible source and agent provenance;
- permission checks before sensitive tools or data are used;
- structured fallback when no service is appropriate;
- confirmation before consequential external actions;
- concise action logs rather than hidden or exposed chain-of-thought;
- failure recovery that does not repeatedly shift work back to the caregiver.

### 5. Design for scarce caregiver time and attention

Caregivers may have little capacity to browse, configure, or complete long modules. Digital delivery does not automatically remove participation barriers. The system should favor:

- low-friction onboarding;
- just-in-time support;
- short, task-oriented outputs;
- progressive disclosure;
- saved state and resumable workflows;
- accessible language and multimodal alternatives;
- configurable reminders;
- explicit handoff between integrated and focused services;
- measurement of caregiver time saved or added.

An integrated product may reduce search and coordination work, but it can also create feature overload. The integrated mode and microservice mode should share core data contracts and safety rules so the caregiver does not have to repeat information or reconcile conflicting answers.

### 6. Keep knowledge support source-grounded and inspectable

Whether retrieval uses index-guided Markdown navigation, vector search, or both, the system should:

- use curated and versioned health-related content;
- preserve the exact page or passage provenance supporting a claim;
- distinguish retrieved evidence from model interpretation and design suggestion;
- expose uncertainty, missing coverage, and conflicting evidence;
- adapt language without changing the source meaning;
- define out-of-scope and urgent-query behavior;
- protect sensitive user data before retrieval, indexing, or logging;
- evaluate source quality, retrieval quality, and generation quality separately.

Retrieval is not proof of correctness. A fluent answer based on irrelevant or weak material remains unsafe.

### 7. Bound agentic actions and preserve human accountability

The wiki supports agentic assistance for knowledge and workflow tasks, not autonomous care. Safe early action spaces include drafting, summarizing, organizing, locating, reminding, and preparing. Consequential actions should be permissioned, logged, reviewable, and reversible where possible.

Explicit confirmation should precede:

- sending a portal message or other external communication;
- disclosing caregiver or care-recipient information;
- changing sharing permissions;
- modifying a care plan;
- purchasing or ordering;
- scheduling when commitments or sensitive information are involved;
- actuating a device;
- triggering a clinical or emergency workflow, except for clearly defined emergency-direction messaging that does not pretend the system itself is a responder.

### 8. Treat privacy as a dyadic and household design problem

Caregiver systems may hold information about multiple people whose interests do not always align. A single account-level consent flag is insufficient. The design should support separate identities, purposes, data scopes, and revocable permissions for caregiver-only, care-recipient-only, shared, family-shared, and clinician-facing information.

Minimum design expectations include data minimization, explicit purpose, access control, retention rules, auditability, consent and proxy logic, deletion and correction workflows, and human review for sensitive disclosure. Smart-home, location, conversation, symptom, care-plan, and inferred-behavior data require especially clear governance.

## Suggested Capability Boundaries

The following functional boundaries are evidence-informed. They are not a requirement that every function be implemented as an independent LLM agent.

| Capability | Appropriate responsibility | Must not do autonomously |
|---|---|---|
| Coordination | Clarify intent, manage task state, route to functions, combine results, preserve provenance, request confirmation, and support handoff. | Diagnose, select treatment, suppress disagreement, or bypass user and role permissions. |
| Assessment and support routing | Collect caregiver-centered domains, explain results, identify unmet needs, and suggest evidence-aligned support or human follow-up. | Produce a clinical diagnosis, make an unvalidated risk classification, or trigger care changes without accountable review. |
| Condition-aware support | Apply condition, trajectory, task, and context overlays to reusable caregiver functions. | Generalize one condition's intervention evidence to another or present condition content as individualized medical advice. |
| Wiki knowledge translation | Navigate reviewed Markdown pages, return concise evidence-aware answers, cite pages, label evidence versus interpretation, and flag gaps. | Treat a wiki page as infallible, invent missing support, or expose private repository content outside authorized scope. |
| RAG retrieval | Retrieve relevant passages from a versioned corpus and attach passage-level provenance. | Treat vector similarity as evidence quality or use sensitive user data as retrieval/index content without policy and consent. |
| Bounded task support | Draft messages, prepare appointments, create checklists, find resources, and organize reminders or plans. | Send, share, purchase, prescribe, escalate clinically, or actuate devices without confirmation and responsible human ownership. |

## AI-Wiki and RAG Research Opportunity

### What the wiki currently supports

- RAG is supported as a technical method that retrieves passages from an external index and conditions generation on them.
- Curated, versioned sources and visible provenance are supported as health-AI design requirements.
- Markdown-first knowledge organization is the operating architecture of this research wiki and is a plausible runtime retrieval strategy.

### What the wiki does not currently establish

- No maintained source directly evaluates an LLM navigating a Markdown index/page graph as a caregiver-support retrieval method.
- No maintained source compares such navigation with dense-vector RAG on caregiver questions.
- No evidence establishes that either method improves empathy. Empathy may be influenced by prompt format and interaction design independently of retrieval.
- No evidence establishes that a multi-agent layer improves the retrieval comparison.

### Recommended controlled comparison

Use the same frozen wiki snapshot, question set, model family, answer instructions, user context, and maximum evidence budget across conditions:

1. **AI-wiki navigation:** the model uses the index and linked Markdown pages without vector retrieval.
2. **RAG:** the model receives chunks retrieved from a vector index built over the same snapshot.
3. **Hybrid:** index/page navigation establishes scope and ownership, while vector retrieval locates passages within the selected scope.

Keep an ungrounded model condition only if a baseline is useful and ethically appropriate; it should not be treated as a deployable health-support mode.

### Evaluation dimensions

Evidence-backed evaluation requirements suggest measuring:

- claim correctness and source support;
- citation or page provenance accuracy;
- relevant-evidence coverage and omission;
- contradiction recognition;
- uncertainty and out-of-scope handling;
- separation of caregiver and care-recipient needs;
- condition and trajectory appropriateness;
- clinical-boundary and escalation behavior;
- privacy-sensitive response behavior;
- readability, structure, actionability, and cognitive load;
- empathy and respect, rated separately from factual quality;
- retrieval trace quality and reproducibility;
- latency, token use, cost, and maintenance burden;
- robustness after wiki updates and under missing or stale pages.

Accuracy, empathy, and response structure are reasonable primary families, but they are not sufficient alone. A polished, empathic answer can still be unsupported or unsafe; an accurate answer can still be unusable or violate dyadic privacy.

## Evaluation Framework for the Caregiver System

For each feature or agent, specify this chain before testing:

`caregiver need -> mechanism -> immediate output -> proximal outcome -> distal outcome -> implementation outcome`

Example:

`information overload -> source-grounded summarization -> cited short answer -> improved comprehension/preparedness -> better care coordination (hypothesis) -> sustained use across caregiver groups`

Do not jump from the immediate output to the distal outcome. Useful evaluation layers are:

1. **Technical:** routing accuracy, retrieval relevance, source faithfulness, task completion, failure recovery, privacy/security tests, and action-log integrity.
2. **Interaction:** usability, accessibility, literacy fit, cognitive load, empathy, trust calibration, and caregiver time added or saved.
3. **Caregiver process:** knowledge, preparedness, self-efficacy, mastery, coping, coordination, skill performance, and navigation completion.
4. **Caregiver outcomes:** burden dimensions, depression, anxiety/stress, physical health, sleep, self-care, social connection, work, and economic effects.
5. **Care-recipient and dyadic outcomes:** autonomy, privacy, function, safety, communication, conflict, shared planning, and quality of life.
6. **Implementation:** reach and representativeness, adoption, appropriateness, feasibility, fidelity, workforce burden, cost, equity, maintenance, and sustainability.

Usability, acceptability, satisfaction, completion, and engagement are valuable but must remain distinct from caregiver or care-recipient effectiveness.

## Accuracy and Overclaim Guardrails

The external design should avoid implying that the maintained wiki proves any of the following:

- multi-agent architecture is better than a single-agent or service-oriented alternative;
- RAG or Markdown navigation guarantees correct health information;
- AI caregiver support reduces burden, improves safety, or improves clinical outcomes;
- assessment scores authorize autonomous clinical triage;
- dementia evidence generalizes to SCI, cancer, or all older adults;
- a caregiver's preference authorizes access to care-recipient data;
- usability, satisfaction, or task completion demonstrates intervention effectiveness;
- an integrated one-stop product necessarily reduces workload;
- HIPAA-oriented technical controls alone establish legal compliance or safe research practice.

## Research and Design Gaps Exposed by the Concept

- Comparative evidence for multi-agent versus single-agent or conventional modular-service architectures in caregiver support.
- Empirical evaluation of index-guided Markdown wiki navigation for health knowledge support.
- Controlled AI-wiki versus RAG versus hybrid comparison over identical content.
- Long-term caregiver and dyadic outcomes from AI-enabled support.
- Safety, workload, and accountability effects of proactive agents.
- Cross-condition generalization without flattening condition differences.
- Equity across literacy, language, culture, technology access, rurality, disability, and socioeconomic constraints.
- Real-world implementation, workforce fit, cost, adoption, fidelity, and maintenance.

## Maintained Wiki Basis

Primary synthesis and design owners:

- `wiki/overview/caregiver_system_core_sota_synthesis.md`
- `wiki/design_patterns/adaptive_modular_caregiver_mhealth.md`
- `wiki/design_patterns/one_stop_caregiver_support_app.md`
- `wiki/design_patterns/caregiver_assessment_and_triage.md`
- `wiki/design_patterns/person_and_family_centered_care_coordination.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`
- `wiki/design_patterns/caregiver_intervention_evaluation_core_outcomes.md`
- `wiki/caregiving_challenges/information_access_and_health_literacy.md`
- `wiki/caregiving_challenges/caregiver_time_burden_and_engagement.md`
- `wiki/caregiving_challenges/care_coordination_and_shared_access.md`
- `wiki/care_recipient_needs/autonomy_privacy_and_dignity.md`
- `wiki/concepts/caregiver_vs_care_recipient_needs.md`
- `wiki/technologies/ai_driven_digital_health.md`

Key source-level evidence pages used to set boundaries:

- `wiki/evidence/dissertation_family_caregiver_mhealth_app.md`
- `wiki/evidence/hcd_generative_ai_family_caregiver_mhealth.md`
- `wiki/evidence/hasan_2025_carebuddy_multi_agent_conversational_ai_alzheimers.md`
- `wiki/evidence/malhotra_2025_carebuddy_mobile_care_ecosystem_dementia_caregiving.md`
- `wiki/evidence/ruggiano_2021_chatbots_dementia_caregivers.md`
- `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`
- `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`

## Clinical and Research Boundary

This brief supports research, product design, architecture review, and knowledge-support planning. It does not authorize clinical decision-making, diagnosis, treatment recommendation, medication guidance, autonomous escalation, or substitution for professional medical, legal, ethics, privacy, security, or IRB review.
