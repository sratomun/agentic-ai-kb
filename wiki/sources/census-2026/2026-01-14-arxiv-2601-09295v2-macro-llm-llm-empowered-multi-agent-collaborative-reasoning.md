---
type: source
source_type: arxiv
title: "MACRO-LLM: LLM-Empowered Multi-Agent Collaborative Reasoning under Spatiotemporal Partial Observability"
authors: Handi Chen, Running Zhao, Xiuzhe Wu, Edith C. H. Ngai
url: https://arxiv.org/abs/2601.09295v2
date: 2026-01-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.MA
tags: [agent-economies, agent-reliability, agentic-rl, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# MACRO-LLM: LLM-Empowered Multi-Agent Collaborative Reasoning under Spatiotemporal Partial Observability

**arXiv:** [2601.09295v2](https://arxiv.org/abs/2601.09295v2) · 2026-01-14 · cs.MA
**Authors:** Handi Chen, Running Zhao, Xiuzhe Wu, Edith C. H. Ngai

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) agents deployed in complex real-world scenarios increasingly operate as spatially distributed entities. However, this physical dispersion constrains agents to limited local perception and finite temporal horizons. We characterize this bottleneck as spatiotemporal partial observability, where spatial and temporal limitations are fundamentally coupled: resolving spatial conflicts requires temporal reasoning about neighbors' future actions, while temporal planning requires spatial context beyond local perception. To bridge this gap, we introduce MACRO-LLM, LLM-empowered multi-agent collaborative reasoning under spatiotemporal partial observability. The architecture interleaves spatial and temporal reasoning within each decision cycle via three interdependent modules: (1) the CoProposer mitigates temporal uncertainty by verifying candidate actions via predictive rollouts; (2) the Negotiator overcomes spatial myopia by resolving conflicts through mean-field statistical aggregation, grounded in the CoProposer's rollout rewards; and (3) the Introspector closes the reasoning loop by analyzing environmental drift and attributing performance changes to refine strategies. Extensive evaluations on two complex long-horizon tasks, cooperative platoon planning and pandemic control, demonstrate that our framework enables robust coordination under spatiotemporal partial observability.

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.09295v2)
