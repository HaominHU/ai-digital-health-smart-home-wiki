---
title: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
type: reference_item
status: ready
privacy: private
source_id: 2020_lewis_retrieval-augmented-generation-knowledge-intensive-nlp
source_type: conference paper
evidence_type: published technical evidence
citation_status: complete
export_ready: true
authors:
  - Patrick Lewis
  - Ethan Perez
  - Aleksandra Piktus
  - Fabio Petroni
  - Vladimir Karpukhin
  - Naman Goyal
  - Heinrich Kuttler
  - Mike Lewis
  - Wen-tau Yih
  - Tim Rocktaschel
  - Sebastian Riedel
  - Douwe Kiela
year: 2020
date: 2020
venue_or_publisher: NeurIPS
journal:
volume:
issue:
pages:
doi:
url:
zotero_key:
endnote_record_number:
source_file: sources/papers/32_lewis_rag_2020.pdf
related_evidence_pages:
  - wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md
related_wiki_pages:
  - wiki/design_patterns/retrieval_grounded_health_ai_support.md
  - wiki/technologies/ai_driven_digital_health.md
topics: [retrieval-augmented generation, RAG, language models, provenance, hallucination]
populations: []
conditions: []
technologies:
  - ai-driven digital health
caregiving_challenges:
  - information access and health literacy
care_recipient_needs:
  - pre-clinic preparation and advocacy
writing_roles:
  - technical method
  - source-grounded AI design rationale
  - hallucination and provenance caution
  - dynamic knowledge update rationale
tags: [reference-item, rag, retrieval-augmented-generation, ai-methods]
last_updated: 2026-05-27
---

# Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks

## Original Citation

Lewis P, Perez E, Piktus A, Petroni F, Karpukhin V, Goyal N, Kuttler H, Lewis M, Yih W, Rocktaschel T, Riedel S, Kiela D. 2020. Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks. 34th Conference on Neural Information Processing Systems.

## RIS Export Fields

- `TY`: CONF
- `AU`: Lewis, Patrick
- `AU`: Perez, Ethan
- `AU`: Piktus, Aleksandra
- `AU`: Petroni, Fabio
- `AU`: Karpukhin, Vladimir
- `AU`: Goyal, Naman
- `AU`: Kuttler, Heinrich
- `AU`: Lewis, Mike
- `AU`: Yih, Wen-tau
- `AU`: Rocktaschel, Tim
- `AU`: Riedel, Sebastian
- `AU`: Kiela, Douwe
- `TI`: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
- `T2`: 34th Conference on Neural Information Processing Systems
- `PY`: 2020
- `DO`:
- `UR`:
- `AB`: Technical paper introducing RAG, a retrieval-augmented generation architecture combining parametric seq2seq generation with non-parametric dense retrieval over an external document index.
- `KW`: retrieval-augmented generation; RAG; language models; dense retrieval; hallucination; provenance
- `ER`:

## Why This Source Matters

This source provides a core architecture for retrieval-grounded language generation. It supports future wiki reasoning about AI systems that need source-grounded outputs, inspectable retrieved context, updateable knowledge, and reduced hallucination risk.

## Supported Claims or Knowledge Roles

- RAG combines a parametric seq2seq generator with a non-parametric dense retrieval index.
- RAG-Sequence uses the same retrieved document across the generated sequence; RAG-Token can condition different tokens on different documents.
- The non-parametric memory can be replaced to update model knowledge without retraining the generator.
- Retrieval can improve factuality and specificity in benchmark generation tasks, but does not guarantee correctness.
- RAG is a technical method source, not healthcare effectiveness evidence.

## Writing Roles

- Technical method.
- AI architecture rationale.
- Source-grounded content design.
- Hallucination and provenance caution.
- Dynamic knowledge update rationale.
- Future digital health design rationale.

## Topic Links

- `wiki/evidence/lewis_2020_rag_knowledge_intensive_nlp.md`
- `wiki/design_patterns/retrieval_grounded_health_ai_support.md`
- `wiki/technologies/ai_driven_digital_health.md`

## Evidence Limits

- Evaluated on NLP benchmarks, not healthcare, caregiving, disability, aging, or smart-home tasks.
- Uses Wikipedia as an external index in the reported experiments; this is not a health-grade knowledge base.
- Retrieved documents may be biased, incomplete, outdated, or wrong.
- Does not establish clinical safety, caregiver usability, or intervention effectiveness.

## Privacy or Sensitivity Notes

No PHI or identifiable participant data detected in the extracted text.

## Export Notes

Ready for basic RIS export. DOI not available from extracted text.
