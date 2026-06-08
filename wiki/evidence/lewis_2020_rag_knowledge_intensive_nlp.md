---
title: Lewis 2020 Retrieval-Augmented Generation for Knowledge-Intensive NLP
type: evidence_summary
status: ready
privacy: private
source_id: 2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp
source_file: sources/papers/cg_system_core/29a_lewis_rag_2020.pdf
reference_item: wiki/references/items/2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp.md
evidence_type: published technical evidence
source_type: conference paper
tags: [rag, retrieval-augmented-generation, ai-methods, source-grounding]
last_updated: 2026-05-27
---

# Lewis 2020 Retrieval-Augmented Generation for Knowledge-Intensive NLP

## Summary

Lewis et al. 2020 introduces retrieval-augmented generation, or RAG, as a method that combines a parametric sequence-to-sequence generator with an explicit non-parametric retrieval index. In the paper, a BART generator is paired with a DPR retriever over a dense vector index of Wikipedia passages.

## Source-Backed Findings

- RAG retrieves top-K text passages for an input and uses those passages as additional context during generation.
- The retrieved document is treated as a latent variable and marginalized during generation.
- RAG-Sequence conditions the whole generated sequence on the same retrieved passage.
- RAG-Token can condition different output tokens on different retrieved passages.
- The retriever query encoder and generator are fine-tuned end-to-end without direct supervision on which document should be retrieved.
- The paper evaluates RAG on open-domain QA, abstractive QA, question generation, and fact verification benchmarks.
- In the reported experiments, RAG outperformed a parametric-only BART baseline on factuality/specificity-oriented generation tasks and achieved strong open-domain QA results.
- The authors show that the non-parametric memory can be replaced to update model knowledge without retraining the generator.

## Wiki-Relevant Interpretation

RAG is useful for this wiki as a technical method for source-grounded AI support. It can inform future caregiver education, resource navigation, pre-clinic preparation, and research-support tools when those tools need to retrieve from an approved source base and produce user-adapted outputs.

## Design Uses

- Ground generated caregiver or care-recipient support in a curated source index.
- Preserve links between AI outputs and retrieved source passages.
- Update the knowledge base without retraining the whole model.
- Separate source retrieval quality from generation quality during evaluation.
- Support source review by clinicians, researchers, or domain experts before deployment.

## Evidence Limits

- This is not healthcare, caregiving, disability, aging, or smart-home evidence.
- Wikipedia retrieval in the paper is not equivalent to a curated health knowledge base.
- Retrieval can reduce some hallucination patterns but cannot guarantee correctness.
- RAG outputs still require source-quality checks, safety review, privacy controls, and human oversight in health-related settings.

## Source Citation

- `2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp`: Lewis P, Perez E, Piktus A, Petroni F, Karpukhin V, Goyal N, Kuttler H, Lewis M, Yih W, Rocktaschel T, Riedel S, Kiela D. Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks. 34th Conference on Neural Information Processing Systems. 2020. Source file: `sources/papers/cg_system_core/29a_lewis_rag_2020.pdf`.
