---
type: source
source_type: arxiv
title: "APEX-MEM: Agentic Semi-Structured Memory with Temporal Reasoning for Long-Term Conversational AI"
authors: Pratyay Banerjee, Masud Moshtaghi, Shivashankar Subramanian, Amita Misra et al.
url: https://arxiv.org/abs/2604.14362v1
date: 2026-04-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [knowledge-graph, agent-reliability, agent-memory, arxiv, auto-ingested]
---

# APEX-MEM: Agentic Semi-Structured Memory with Temporal Reasoning for Long-Term Conversational AI

**arXiv:** [2604.14362v1](https://arxiv.org/abs/2604.14362v1) · 2026-04-15 · cs.CL
**Authors:** Pratyay Banerjee, Masud Moshtaghi, Shivashankar Subramanian, Amita Misra et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models still struggle with reliable long-term conversational memory: simply enlarging context windows or applying naive retrieval often introduces noise and destabilizes responses. We present APEX-MEM, a conversational memory system that combines three key innovations: (1) a property graph which uses domain-agnostic ontology to structure conversations as temporally grounded events in an entity-centric framework, (2) append-only storage that preserves the full temporal evolution of information, and (3) a multi-tool retrieval agent that understands and resolves conflicting or evolving information at query time, producing a compact and contextually relevant memory summary. This retrieval-time resolution preserves the full interaction history while suppressing irrelevant details. APEX-MEM achieves 88.88% accuracy on LOCOMO's Question Answering task and 86.2% on LongMemEval, outperforming state-of-the-art session-aware approaches and demonstrating that structured property graphs enable more temporally coherent long-term conversational reasoning.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14362v1)
