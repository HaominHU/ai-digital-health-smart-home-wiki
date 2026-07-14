---
title: Citation-Supported Brainstorming Workflow
type: workflow
status: draft
privacy: private
last_updated: 2026-07-14
---

# Citation-Supported Brainstorming Workflow

## Purpose

Use stored wiki knowledge and citation-memory records to help brainstorm a manuscript, grant, proposal, or research idea while producing:

- A structured citation map for introduction, background, and significance.
- A citation coverage assessment.
- An AI-ready drafting prompt grounded in wiki context.
- Separate Zotero/EndNote-compatible citation export lists for wiki citations and searched external candidates when applicable, usually RIS.

This workflow keeps the wiki as knowledge-level citation memory and keeps Zotero/EndNote as the paper-level reference manager.

## Use When the User Says

- "I am brainstorming a paper about..."
- "Suggest citations for this paper idea."
- "Generate citations and a prompt for intro/background/significance."
- "Create a Zotero/EndNote import list for this topic."
- "Build a reference set from the wiki for this manuscript."

## Default Mode

Use wiki-first mode:

1. Use citations already represented in `wiki/references/items/`, `wiki/evidence/`, `MEMORY.md`, and relevant wiki pages.
2. Assess coverage quality rather than applying a fixed citation-count threshold.
3. Clearly mark citation gaps where the wiki lacks adequate foundational, state-of-the-art, population, condition, technology, or argumentative-role coverage.
4. Do not invent citations, DOIs, author lists, venues, findings, or source details.
5. Search externally only if the user explicitly asks, approves expanded search, or asks to include searched citations.
6. Keep searched external citations separate from wiki citations and label them as unreviewed candidates until ingested or reviewed.

## Required Inputs

Ask for missing context only when needed. Useful context includes:

- Working paper topic.
- Target section: introduction, background, significance, literature review, aims, design rationale, or another section.
- Target audience or venue.
- Condition, population, technology, caregiving challenge, or care-recipient need focus.
- Whether the user wants a durable output file.
- Whether to use wiki-only, wiki-first, or wiki-first plus external seed search mode.

## Steps

1. Read `AGENTS.md`, `MEMORY.md`, `INDEX.md`, and this workflow.
2. Read `wiki/references/README.md` and relevant records under `wiki/references/items/`.
3. If reference records are missing, inspect relevant evidence pages under `wiki/evidence/` and mark missing citation records as a backfill gap.
4. Read relevant topic pages across populations, conditions, technologies, caregiving challenges, care-recipient needs, concepts, design patterns, and evidence.
5. Interpret the user's topic into wiki concepts without conflating caregiver needs with care recipient needs, disease with aging, or disability with aging-related decline.
6. Assess citation coverage quality:
   - Strong coverage areas.
   - Weak or narrow coverage areas.
   - Missing foundational or classic citations.
   - Missing recent state-of-the-art citations.
   - Missing population, condition, technology, or care-context anchors.
   - Potential over-reliance on one research group, one condition, one technology, one study type, or one evidence category.
   - Whether external seed search is recommended and why.
7. Build a wiki citation map grouped by argumentative role:
   - Foundational/background context.
   - Population or caregiving burden.
   - Condition-specific context.
   - Technology or intervention rationale.
   - Problem significance.
   - Gaps and limitations.
   - Methods, design, or implementation rationale when relevant.
8. If external seed search is requested or approved, build a separate searched candidate citation map:
   - Classic or foundational candidates.
   - Recent state-of-the-art candidates.
   - Review, guideline, framework, or consensus candidates.
   - Directly topic-specific candidates.
   - Search date, search scope, and reason for inclusion.
9. For each recommended wiki citation, include:
   - Source ID.
   - Human-readable citation.
   - Evidence type.
   - Suggested writing role.
   - Claim it can support.
   - Limits or cautions.
10. For each searched external candidate citation, include:
   - Human-readable citation.
   - DOI or URL when verified.
   - Candidate role.
   - Why it may be useful.
   - Status: external candidate, not yet ingested.
   - Metadata confidence.
   - Whether it is RIS export-ready.
11. Generate an AI feed prompt that includes:
   - Purpose.
   - Downstream agent role.
   - Topic interpretation.
   - Wiki citation map.
   - Searched candidate citation map when applicable.
   - Evidence gaps.
   - Privacy, ethics, and clinical decision-boundary constraints.
   - Required output structure.
   - Review criteria.
12. If requested, create a durable output under `outputs/research_prompts/` or `outputs/query_answers/` using `wiki/templates/citation_supported_brainstorming_output_template.md`.
13. If requested, create separate RIS exports under `outputs/citation_exports/`:
   - `YYYY-MM-DD_topic_wiki-citations.ris`
   - `YYYY-MM-DD_topic_external-candidates.ris`
   - Treat generated exports as local-only by default; track a specific export only when the user explicitly asks to preserve or publish it.
14. Append a `prompt`, `query`, or `output` entry to `LOG.md` when creating durable files.

## Output Structure

Use this structure by default:

```text
# Citation-Supported Brainstorming Output

## Topic Interpretation

## Relevant Wiki Concepts

## Citation Coverage Assessment

## Wiki Citation Map

### Introduction and Broad Background

### Population, Caregiving, or Care Recipient Significance

### Condition-Specific Context

### Technology or Intervention Rationale

### Gap and Significance Framing

## Evidence Gaps

## Searched External Candidate Citations

## AI Feed Prompt

## Zotero/EndNote-Compatible RIS Export Files

### Wiki Citation RIS

### External Candidate RIS

## Backfill or Cleanup Notes
```

## RIS Export Rules

RIS is the default export format because Zotero and EndNote both import it.

Only include a citation in RIS when the minimum export fields are available:

- `TY`
- `TI`
- at least one `AU` or organization author when known
- `PY` or source date when known
- `ER`

Use `TY  - JOUR` for journal articles, `TY  - THES` for dissertations, `TY  - CONF` for conference abstracts or proceedings, `TY  - RPRT` for reports, and `TY  - GEN` when the source type is uncertain.

If metadata is incomplete, include the source in the human-readable citation map but place it under "not export-ready" instead of inventing missing RIS fields.

## External Seed Search Rules

External seed search is a supplement for early or incomplete wiki coverage. It should not replace wiki citation memory.

Use a coverage-quality trigger, not a fixed citation-count threshold. External seed search may be useful when the wiki is missing:

- Foundational, classic, or highly influential sources.
- Recent state-of-the-art sources.
- Review, guideline, framework, or consensus sources.
- Population-specific anchors.
- Condition-specific anchors.
- Technology or intervention anchors.
- Evidence for an important argumentative role in the proposed paper.

When external search is used:

- Keep searched citations separate from wiki citations.
- Label them as external candidates and not yet ingested.
- Record search date and search scope.
- Prefer a small, high-signal set rather than a comprehensive bibliography.
- Verify metadata before producing RIS.
- Do not treat searched candidates as established wiki evidence until they are ingested or reviewed.

## Boundary Rules

This workflow supports research, writing, design, and knowledge support. It must not ask an AI agent to make clinical decisions, diagnose, recommend treatment, or provide patient-specific care instructions.

For healthcare and study-related outputs, include privacy, security, consent, data minimization, access control, de-identification, auditability, bias/fairness, vulnerable-population, and human oversight considerations when relevant.
