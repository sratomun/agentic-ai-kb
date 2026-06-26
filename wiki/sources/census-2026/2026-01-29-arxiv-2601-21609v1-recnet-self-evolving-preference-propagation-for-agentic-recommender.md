---
type: source
source_type: arxiv
title: "RecNet: Self-Evolving Preference Propagation for Agentic Recommender Systems"
authors: Bingqian Li, Xiaolei Wang, Junyi Li, Weitao Li et al.
url: https://arxiv.org/abs/2601.21609v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [recommendation-agents, self-evolving-agents, agentic-rl, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# RecNet: Self-Evolving Preference Propagation for Agentic Recommender Systems

**arXiv:** [2601.21609v1](https://arxiv.org/abs/2601.21609v1) · 2026-01-29 · cs.AI
**Authors:** Bingqian Li, Xiaolei Wang, Junyi Li, Weitao Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic recommender systems leverage Large Language Models (LLMs) to model complex user behaviors and support personalized decision-making. However, existing methods primarily model preference changes based on explicit user-item interactions, which are sparse, noisy, and unable to reflect the real-time, mutual influences among users and items. To address these limitations, we propose RecNet, a self-evolving preference propagation framework that proactively propagates real-time preference updates across related users and items. RecNet consists of two complementary phases. In the forward phase, the centralized preference routing mechanism leverages router agents to integrate preference updates and dynamically propagate them to the most relevant agents. To ensure accurate and personalized integration of propagated preferences, we further introduce a personalized preference reception mechanism, which combines a message buffer for temporary caching and an optimizable, rule-based filter memory to guide selective preference assimilation based on past experience and interests. In the backward phase, the feedback-driven propagation optimization mechanism simulates a multi-agent reinforcement learning framework, using LLMs for credit assignment, gradient analysis, and module-level optimization, enabling continuous self-evolution of propagation strategies. Extensive experiments on various scenarios demonstrate the effectiveness of RecNet in modeling preference propagation for recommender systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21609v1)
