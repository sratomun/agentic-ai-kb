---
type: source
source_type: arxiv
title: "Time is Not a Label: Continuous Phase Rotation for Temporal Knowledge Graphs and Agentic Memory"
authors: Weixian Waylon Li, Jiaxin Zhang, Xianan Jim Yang, Tiejun Ma et al.
url: https://arxiv.org/abs/2604.11544v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [finance-agents, knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Time is Not a Label: Continuous Phase Rotation for Temporal Knowledge Graphs and Agentic Memory

**arXiv:** [2604.11544v1](https://arxiv.org/abs/2604.11544v1) · 2026-04-13 · cs.CL
**Authors:** Weixian Waylon Li, Jiaxin Zhang, Xianan Jim Yang, Tiejun Ma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Structured memory representations such as knowledge graphs are central to autonomous agents and other long-lived systems. However, most existing approaches model time as discrete metadata, either sorting by recency (burying old-yet-permanent knowledge), simply overwriting outdated facts, or requiring an expensive LLM call at every ingestion step, leaving them unable to distinguish persistent facts from evolving ones. To address this, we introduce RoMem, a drop-in temporal knowledge graph module for structured memory systems, applicable to agentic memory and beyond. A pretrained Semantic Speed Gate maps each relation's text embedding to a volatility score, learning from data that evolving relations (e.g., "president of") should rotate fast while persistent ones (e.g., "born in") should remain stable. Combined with continuous phase rotation, this enables geometric shadowing: obsolete facts are rotated out of phase in complex vector space, so temporally correct facts naturally outrank contradictions without deletion. On temporal knowledge graph completion, RoMem achieves state-of-the-art results on ICEWS05-15 (72.6 MRR). Applied to agentic memory, it delivers 2-3x MRR and answer accuracy on temporal reasoning (MultiTQ), dominates hybrid benchmark (LoCoMo), preserves static memory with zero degradation (DMR-MSC), and generalises zero-shot to unseen financial domains (FinTMMBench).

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.11544v1)
