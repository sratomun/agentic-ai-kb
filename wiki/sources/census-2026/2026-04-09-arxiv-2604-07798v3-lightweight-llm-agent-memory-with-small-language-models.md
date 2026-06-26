---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Lightweight LLM Agent Memory with Small Language Models"
authors: Jiaquan Zhang et al.
url: https://arxiv.org/abs/2604.07798v3
date: 2026-04-09
score: 11
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, agent-memory, agentic-rag, clinical-agents]
---

# Lightweight LLM Agent Memory with Small Language Models

**arXiv:** [2604.07798v3](https://arxiv.org/abs/2604.07798v3) · 2026-04-09 · cs.AI
**Authors:** Jiaquan Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Although LLM agents can leverage tools for complex tasks, they still need memory to maintain cross-turn consistency and accumulate reusable information in long-horizon interactions. However, retrieval-based external memory systems incur low online overhead but suffer from unstable accuracy due to limited query construction and candidate filtering. In contrast, many systems use repeated large-model calls for online memory operations, improving accuracy but accumulating latency over long interactions. We propose LightMem, a lightweight memory system for better agent memory driven by Small Language Models (SLMs). LightMem modularizes memory retrieval, writing, and long-term consolidation, and separates online processing from offline consolidation to enable efficient memory invocation under bounded compute. We organize memory into short-term memory (STM) for immediate conversational context, mid-term memory (MTM) for reusable interaction summaries, and long-term memory (LTM) for consolidated knowledge, and uses user identifiers to support independent retrieval and incremental maintenance in multi-user settings. Online, LightMem operates under a fixed retrieval budget and selects memories via a two-stage procedure: vector-based coarse retrieval followed by semantic consistency re-ranking. Offline, it abstracts reusable interaction evidence and incrementally integrates it into LTM. Experiments show consistent gains across model scales, with an average F1 improvement of about 2.5 over A-MEM on LoCoMo, while achieving higher efficiency and low median latency (83 ms for retrieval and 581 ms end-to-end).

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[agentic-rag]] · [[clinical-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.07798v3)
