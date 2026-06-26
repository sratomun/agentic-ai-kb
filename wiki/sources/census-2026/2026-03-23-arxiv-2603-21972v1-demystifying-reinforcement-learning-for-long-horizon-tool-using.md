---
type: source
source_type: arxiv
title: "Demystifying Reinforcement Learning for Long-Horizon Tool-Using Agents: A Comprehensive Recipe"
authors: Xixi Wu, Qianguo Sun, Ruiyang Zhang, Chao Song et al.
url: https://arxiv.org/abs/2603.21972v1
date: 2026-03-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.LG
tags: [agentic-rl, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Demystifying Reinforcement Learning for Long-Horizon Tool-Using Agents: A Comprehensive Recipe

**arXiv:** [2603.21972v1](https://arxiv.org/abs/2603.21972v1) · 2026-03-23 · cs.LG
**Authors:** Xixi Wu, Qianguo Sun, Ruiyang Zhang, Chao Song et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement Learning (RL) is essential for evolving Large Language Models (LLMs) into autonomous agents capable of long-horizon planning, yet a practical recipe for scaling RL in complex, multi-turn environments remains elusive. This paper presents a systematic empirical study using TravelPlanner, a challenging testbed requiring tool orchestration to satisfy multifaceted constraints. We decompose the agentic RL design space along 5 axes: reward shaping, model scaling, data composition, algorithm selection, and environmental stability. Our controlled experiments yield 7 key takeaways, e.g., (1) reward and algorithm choices are scale-dependent as smaller models benefit from staged rewards and enhanced exploration, whereas larger models converge efficiently with simpler dense rewards, (2) ~ 1K training samples with a balanced difficulty mixture mark a sweet spot for both in-domain and out-of-domain performance, and (3) environmental stability is critical to prevent policy degradation. Based on our distilled recipe, our RL-trained models achieve state-of-the-art performance on TravelPlanner, significantly outperforming leading LLMs.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.21972v1)
