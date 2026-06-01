---
title: Yao 2023 ReAct Reasoning and Acting in Language Models
type: evidence_summary
status: ready
privacy: private
source_id: 2023_yao_react-reasoning-acting-language-models
source_file: sources/papers/37_yao_react_2022.pdf
reference_item: wiki/references/items/2023_yao_react-reasoning-acting-language-models.md
evidence_type: published technical evidence
source_type: conference paper
tags: [react, language-agents, tool-use, ai-methods, human-oversight]
last_updated: 2026-05-27
---

# Yao 2023 ReAct Reasoning and Acting in Language Models

## Summary

Yao et al. 2023 introduces ReAct, a prompting paradigm that interleaves language-model reasoning traces with task-specific actions. The paper evaluates ReAct on question answering, fact verification, text-based decision-making, and web-shopping benchmarks.

## Source-Backed Findings

- ReAct prompts language models to generate reasoning traces and task-specific actions in an interleaved manner.
- Reasoning traces can support plan creation, plan tracking, exception handling, and task-state maintenance.
- Actions allow the model to interact with external sources or environments, including a Wikipedia API and benchmark environments.
- On HotpotQA and FEVER, ReAct used external information interaction to address some hallucination and error-propagation issues.
- On ALFWorld and WebShop, ReAct outperformed action-only prompting and reported stronger success rates than imitation or reinforcement learning baselines in the paper's few-shot setup.
- The paper presents ReAct trajectories as more interpretable and diagnosable because humans can inspect thoughts, actions, and observations.
- The ethics statement warns that connecting language models to external environments can create risks, including inappropriate/private information access or harmful actions.

## Wiki-Relevant Interpretation

ReAct is useful for this wiki as a technical method for bounded AI agents that reason, retrieve, and act through permissioned tools. It is relevant to future research/design prompts for pre-clinic preparation, resource lookup, care coordination drafts, or smart-home support only when the action space is safe, auditable, and non-autonomous for clinical decisions.

## Design Uses

- Structure multi-step AI support around explicit observe-think-act loops.
- Separate internal reasoning support from user-facing summaries and source-backed outputs.
- Use tool actions for source lookup, draft generation, task tracking, or resource navigation.
- Keep health-related actions permissioned, logged, reversible where possible, and subject to human confirmation.
- Inspect and evaluate action traces for failure modes, privacy violations, unsafe escalation, and burden shifting.

## Evidence Limits

- This is not healthcare, caregiving, disability, aging, or smart-home evidence.
- Benchmark success does not establish clinical safety or caregiver utility.
- ReAct can still hallucinate, fail to recover from errors, or choose inappropriate actions.
- The paper's experiments intentionally limited action spaces; health and home environments require stricter governance.

## Source Citation

- `2023_yao_react-reasoning-acting-language-models`: Yao S, Zhao J, Yu D, Du N, Shafran I, Narasimhan K, Cao Y. ReAct: Synergizing Reasoning and Acting in Language Models. ICLR 2023. arXiv:`2210.03629v3`. Source file: `sources/papers/37_yao_react_2022.pdf`.
