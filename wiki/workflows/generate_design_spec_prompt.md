---
title: Generate Design or Spec Prompt Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-05-18
---

# Generate Design or Spec Prompt Workflow

## Purpose

Generate an AI-ready prompt for system design, product reasoning, study protocol design, or implementation planning grounded in the wiki.

Use this workflow for:

- Digital health system design.
- Smart home technology concepts.
- Agent knowledge-support design.
- Caregiver support workflows.
- Coding plan-mode prompts.
- Research prototype specifications.
- Study or evaluation planning.

## Steps

1. Read `AGENTS.md`, `MEMORY.md`, and `INDEX.md`.
2. Identify target system, population, condition overlay, setting, and intended use.
3. Read relevant population, condition, caregiving challenge, care recipient need, technology, concept, evidence, and design pattern pages.
4. Extract constraints, evidence-backed needs, known gaps, and speculative design directions.
5. Distinguish knowledge support from autonomous healthcare decision-making.
6. Include privacy, security, consent, access control, auditability, data minimization, retention, human oversight, and escalation constraints.
7. Generate the prompt under `outputs/design_prompts/` or `outputs/spec_prompts/` if the user asks for a file or durable output.
8. Append a `prompt` or `output` entry to `LOG.md` if a file is created.

## Prompt Should Include

- Target user and stakeholder roles.
- Intended use and non-use.
- Caregiver needs and care recipient needs separately.
- Condition-specific overlays.
- Aging, disability, disease, and multimorbidity cautions.
- Technology lens.
- Evidence-backed requirements.
- Unknowns and assumptions.
- Privacy, data security, ethics, and safety constraints.
- Human oversight and escalation boundaries.
- Output format and acceptance criteria.

## Boundary Rule

Design/spec prompts may support research prototypes, planning, and knowledge support. They must not define an autonomous clinical decision system unless the user explicitly frames it as a regulated clinical system design exercise with appropriate review requirements.
