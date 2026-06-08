---
title: "ReAct: Synergizing Reasoning and Acting in Language Models"
type: reference_item
status: ready
privacy: private
source_id: 2023_yao_react-reasoning-acting-language-models
source_type: conference paper
evidence_type: published technical evidence
citation_status: complete
export_ready: true
authors:
  - Shunyu Yao
  - Jeffrey Zhao
  - Dian Yu
  - Nan Du
  - Izhak Shafran
  - Karthik Narasimhan
  - Yuan Cao
year: 2023
date: 2023
venue_or_publisher: ICLR
journal:
volume:
issue:
pages:
doi:
url:
zotero_key:
endnote_record_number:
source_file: sources/papers/cg_system_core/29b_yao_react_2022.pdf
related_evidence_pages:
  - wiki/evidence/yao_2023_react_reasoning_acting_language_models.md
related_wiki_pages:
  - wiki/design_patterns/reasoning_action_health_ai_agent.md
  - wiki/technologies/ai_driven_digital_health.md
topics: [ReAct, language agents, reasoning, acting, tool use, human oversight]
populations: []
conditions: []
technologies:
  - ai-driven digital health
  - smart home technologies
caregiving_challenges:
  - care coordination and shared access
  - information access and health literacy
care_recipient_needs:
  - pre-clinic preparation and advocacy
  - autonomy privacy and dignity
writing_roles:
  - technical method
  - agentic AI design rationale
  - tool-use architecture
  - inspectability and human oversight rationale
  - action-space safety caution
tags: [reference-item, react, language-agents, ai-methods]
last_updated: 2026-05-27
---

# ReAct: Synergizing Reasoning and Acting in Language Models

## Original Citation

Yao S, Zhao J, Yu D, Du N, Shafran I, Narasimhan K, Cao Y. 2023. ReAct: Synergizing Reasoning and Acting in Language Models. Published as a conference paper at ICLR 2023. arXiv:`2210.03629v3`.

## RIS Export Fields

- `TY`: CONF
- `AU`: Yao, Shunyu
- `AU`: Zhao, Jeffrey
- `AU`: Yu, Dian
- `AU`: Du, Nan
- `AU`: Shafran, Izhak
- `AU`: Narasimhan, Karthik
- `AU`: Cao, Yuan
- `TI`: ReAct: Synergizing Reasoning and Acting in Language Models
- `T2`: International Conference on Learning Representations
- `PY`: 2023
- `DO`:
- `UR`:
- `AB`: Technical paper introducing ReAct, a prompting paradigm that interleaves language-model reasoning traces with task-specific actions for question answering, fact verification, and interactive decision-making benchmarks.
- `KW`: ReAct; language agents; reasoning; acting; tool use; human oversight
- `ER`:

## Why This Source Matters

This source provides a technical method for interleaving reasoning and action in language-model agents. It is relevant to future AI-driven digital health design only as architecture rationale for bounded, inspectable, tool-using knowledge support.

## Supported Claims or Knowledge Roles

- ReAct interleaves reasoning traces and task-specific actions.
- Reasoning traces can support plan tracking, exception handling, and state maintenance.
- Actions can gather information from external sources or environments.
- Intermediate traces and observations can improve inspectability and diagnosability.
- Connecting language models to action spaces creates safety and privacy risks if actions are consequential, private, or harmful.

## Writing Roles

- Technical method.
- Agentic AI architecture rationale.
- Tool-use and external-information design rationale.
- Human oversight and inspectability rationale.
- Safety and action-space caution.
- Future digital health design rationale.

## Topic Links

- `wiki/evidence/yao_2023_react_reasoning_acting_language_models.md`
- `wiki/design_patterns/reasoning_action_health_ai_agent.md`
- `wiki/technologies/ai_driven_digital_health.md`

## Evidence Limits

- Evaluated on benchmark tasks, not healthcare or caregiving workflows.
- Does not establish safety, effectiveness, usability, or equity in health settings.
- ReAct can still hallucinate, fail, choose poor actions, or exceed context limits.
- Health-related uses require permissioned action spaces, privacy controls, auditability, and human oversight.

## Privacy or Sensitivity Notes

No PHI or identifiable participant data detected in the extracted text.

## Export Notes

Ready for basic RIS export. DOI not available from extracted text.
