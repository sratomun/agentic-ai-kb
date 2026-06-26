---
type: source
source_type: arxiv
title: "BAPO: Boundary-Aware Policy Optimization for Reliable Agentic Search"
authors: Shiyu Liu, Yongjing Yin, Jianhao Yan, Yunbo Tang et al.
url: https://arxiv.org/abs/2601.11037v2
date: 2026-01-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# BAPO: Boundary-Aware Policy Optimization for Reliable Agentic Search

**arXiv:** [2601.11037v2](https://arxiv.org/abs/2601.11037v2) · 2026-01-16 · cs.AI
**Authors:** Shiyu Liu, Yongjing Yin, Jianhao Yan, Yunbo Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
RL-based agentic search enables LLMs to solve complex questions via dynamic planning and external search. While this approach significantly enhances accuracy with agent policies optimized via large-scale reinforcement learning, we identify a critical gap in reliability: these agents fail to recognize their reasoning boundaries and rarely admit ``I DON'T KNOW'' (IDK) even when evidence is insufficient or reasoning reaches its limit. The lack of reliability often leads to plausible but unreliable answers, introducing significant risks in many real-world scenarios. To this end, we propose Boundary-Aware Policy Optimization (BAPO), a novel RL framework designed to cultivate reliable boundary awareness without compromising accuracy. BAPO introduces two key components: (i) a group-based boundary-aware reward that encourages an IDK response only when the reasoning reaches its limit, and (ii) an adaptive reward modulator that strategically suspends this reward during early exploration, preventing the model from exploiting IDK as a shortcut. Extensive experiments on four benchmarks demonstrate that BAPO substantially enhances the overall reliability of agentic search.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.11037v2)
