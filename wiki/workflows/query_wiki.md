---
title: Query Wiki Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-06-17
---

# Query Wiki Workflow

## Purpose

Answer questions against the maintained research wiki and preserve valuable synthesis when it should compound into future work.

Use this workflow for:

- General domain questions.
- Evidence synthesis.
- Condition comparisons.
- Caregiving challenge analysis.
- Technology landscape analysis.
- Design reasoning.
- Research gap identification.
- Preparing downstream research, design, coding, or specification prompts.

## Query Steps

1. Read `AGENTS.md` for operating rules.
2. Read `MEMORY.md` for current state and decisions.
3. Read `INDEX.md` to locate relevant pages.
4. Read relevant pages under `wiki/`.
5. Clearly separate evidence-backed claims, interpretation, gaps, and speculative design directions.
6. Respect the clinical decision boundary.
7. Include privacy, security, and human oversight considerations when relevant.
8. Answer the user's question with file references when useful.
9. If the answer creates durable knowledge, ask whether to file it back into the wiki unless the user already requested a durable output.
10. If the query reveals stale overview, synthesis, workflow, index, or memory content, state that clearly and ask whether to update it unless the user already requested a durable check or fix.
11. If files are updated, update `INDEX.md` if needed and append a `query` entry to `LOG.md`.

## Answer Standards

Answers should distinguish:

- What the wiki supports.
- What is uncertain.
- What is a research gap.
- What is interpretation.
- What is speculative design direction.
- What should not be treated as clinical guidance.

## Durable Query Outputs

Durable outputs may be saved under `outputs/query_answers/` when useful.

Potential durable outputs:

- Evidence maps.
- Concept comparisons.
- Research gap lists.
- Design implication summaries.
- Agent knowledge-support notes.
- Cross-condition synthesis.

## Required LOG.md Update

If the query only produces a chat answer and no files change, no `LOG.md` entry is required.

If the query creates or updates durable wiki knowledge or an output file, append a `LOG.md` entry in the same turn.
