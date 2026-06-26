---
type: source
source_type: arxiv
title: "MemWeaver: Weaving Hybrid Memories for Traceable Long-Horizon Agentic Reasoning"
authors: Juexiang Ye, Xue Li, Xinyu Yang, Chengkai Huang et al.
url: https://arxiv.org/abs/2601.18204v1
date: 2026-01-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# MemWeaver: Weaving Hybrid Memories for Traceable Long-Horizon Agentic Reasoning

**arXiv:** [2601.18204v1](https://arxiv.org/abs/2601.18204v1) · 2026-01-26 · cs.CL
**Authors:** Juexiang Ye, Xue Li, Xinyu Yang, Chengkai Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model-based agents operating in long-horizon interactions require memory systems that support temporal consistency, multi-hop reasoning, and evidence-grounded reuse across sessions. Existing approaches largely rely on unstructured retrieval or coarse abstractions, which often lead to temporal conflicts, brittle reasoning, and limited traceability. We propose MemWeaver, a unified memory framework that consolidates long-term agent experiences into three interconnected components: a temporally grounded graph memory for structured relational reasoning, an experience memory that abstracts recurring interaction patterns from repeated observations, and a passage memory that preserves original textual evidence. MemWeaver employs a dual-channel retrieval strategy that jointly retrieves structured knowledge and supporting evidence to construct compact yet information-dense contexts for reasoning. Experiments on the LoCoMo benchmark demonstrate that MemWeaver substantially improves multi-hop and temporal reasoning accuracy while reducing input context length by over 95\% compared to long-context baselines.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.18204v1)
