---
title: Generate Research Prompt Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-05-18
---

# Generate Research Prompt Workflow

## Purpose

Generate an AI-ready research or writing prompt from accumulated wiki knowledge.

Use this workflow for:

- Literature review prompts.
- Research question development.
- Study framing.
- Manuscript section drafting.
- Grant or proposal brainstorming.
- Evidence synthesis planning.
- Agent plan-mode prompts for research tasks.

## Steps

1. Read `AGENTS.md`, `MEMORY.md`, and `INDEX.md`.
2. Identify the target topic, audience, and downstream agent role.
3. Read relevant wiki pages.
4. Extract evidence-backed context, gaps, conceptual cautions, and design or research implications.
5. Keep evidence, interpretation, and speculation separate.
6. Include privacy, consent, ethics, data security, and clinical decision-boundary instructions when relevant.
7. Generate the prompt under `outputs/research_prompts/` if the user asks for a file or durable output.
8. Append a `prompt` or `output` entry to `LOG.md` if a file is created.

## Prompt Should Include

- Task objective.
- Background context.
- Relevant populations.
- Conditions and condition-overlap cautions.
- Caregiver vs care recipient distinction.
- Evidence summary.
- Known gaps.
- Privacy and security constraints.
- Clinical decision boundary.
- Desired output format.
- Quality criteria.

## Boundary Rule

Research prompts may support evidence synthesis and writing. They must not ask an agent to provide clinical decisions, diagnosis, treatment recommendations, or patient-specific safety instructions.
