---
type: source
source_type: arxiv
title: "Internalizing Multi-Agent Reasoning for Accurate and Efficient LLM-based Recommendation"
authors: Yang Wu, Haoze Wang, Qian Li, Jun Zhang et al.
url: https://arxiv.org/abs/2602.09829v2
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.IR
tags: [recommendation-agents, multi-agent-systems, arxiv, auto-ingested]
---

# Internalizing Multi-Agent Reasoning for Accurate and Efficient LLM-based Recommendation

**arXiv:** [2602.09829v2](https://arxiv.org/abs/2602.09829v2) · 2026-02-10 · cs.IR
**Authors:** Yang Wu, Haoze Wang, Qian Li, Jun Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) are reshaping recommender systems by leveraging extensive world knowledge and semantic reasoning to interpret user intent. However, effectively integrating these capabilities with collaborative signals while avoiding prohibitive inference latency remains a critical bottleneck. To address this, we propose a trajectory-driven internalization framework to develop a Single-agent Trajectory-Aligned Recommender (STAR). Specifically, to internalize complex reasoning capabilities into a single efficient model, we first design a multi-agent teacher system capable of multi-turn tool usage and reflection. This teacher utilizes a Collaborative Signal Translation mechanism to explicitly convert latent behavioral patterns into descriptive natural language evidence to enhance reasoning accuracy. Subsequently, a trajectory-driven distillation pipeline transfers this agentic logic, including planning, tool usage, and self-reflection, into the compact STAR model. Extensive experiments demonstrate that STAR surpasses its teacher by 8.7% to 39.5% while eliminating iterative latency, paving the way for real-time, reasoning-enhanced recommendation.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.09829v2)
