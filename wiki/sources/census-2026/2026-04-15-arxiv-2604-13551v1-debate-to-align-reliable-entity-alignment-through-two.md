---
type: source
source_type: arxiv
title: "Debate to Align: Reliable Entity Alignment through Two-Stage Multi-Agent Debate"
authors: Cunda Wang, Ziying Ma, Po Hu, Weihua Wang et al.
url: https://arxiv.org/abs/2604.13551v1
date: 2026-04-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.CL
tags: [knowledge-graph, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Debate to Align: Reliable Entity Alignment through Two-Stage Multi-Agent Debate

**arXiv:** [2604.13551v1](https://arxiv.org/abs/2604.13551v1) · 2026-04-15 · cs.CL
**Authors:** Cunda Wang, Ziying Ma, Po Hu, Weihua Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Entity alignment (EA) aims to identify entities referring to the same real-world object across different knowledge graphs (KGs). Recent approaches based on large language models (LLMs) typically obtain entity embeddings through knowledge representation learning and use embedding similarity to identify an alignment-uncertain entity set. For each uncertain entity, a candidate entity set (CES) is then retrieved based on embedding similarity to support subsequent alignment reasoning and decision making. However, the reliability of the CES and the reasoning capability of LLMs critically affect the effectiveness of subsequent alignment decisions. To address this issue, we propose AgentEA, a reliable EA framework based on multi-agent debate. AgentEA first improves embedding quality through entity representation preference optimization, and then introduces a two-stage multi-role debate mechanism consisting of lightweight debate verification and deep debate alignment to progressively enhance the reliability of alignment decisions while enabling more efficient debate-based reasoning. Extensive experiments on public benchmarks under cross-lingual, sparse, large-scale, and heterogeneous settings demonstrate the effectiveness of AgentEA.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.13551v1)
