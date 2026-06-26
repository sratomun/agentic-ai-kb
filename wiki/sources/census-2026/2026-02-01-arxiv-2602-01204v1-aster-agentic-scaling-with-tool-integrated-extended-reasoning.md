---
type: source
source_type: arxiv
title: "ASTER: Agentic Scaling with Tool-integrated Extended Reasoning"
authors: Xuqin Zhang, Quan He, Zhenrui Zheng, Zongzhang Zhang et al.
url: https://arxiv.org/abs/2602.01204v1
date: 2026-02-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agentic-rl, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# ASTER: Agentic Scaling with Tool-integrated Extended Reasoning

**arXiv:** [2602.01204v1](https://arxiv.org/abs/2602.01204v1) · 2026-02-01 · cs.CL
**Authors:** Xuqin Zhang, Quan He, Zhenrui Zheng, Zongzhang Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement learning (RL) has emerged as a dominant paradigm for eliciting long-horizon reasoning in Large Language Models (LLMs). However, scaling Tool-Integrated Reasoning (TIR) via RL remains challenging due to interaction collapse: a pathological state where models fail to sustain multi-turn tool usage, instead degenerating into heavy internal reasoning with only trivial, post-hoc code verification. We systematically study three questions: (i) how cold-start SFT induces an agentic, tool-using behavioral prior, (ii) how the interaction density of cold-start trajectories shapes exploration and downstream RL outcomes, and (iii) how the RL interaction budget affects learning dynamics and generalization under varying inference-time budgets. We then introduce ASTER (Agentic Scaling with Tool-integrated Extended Reasoning), a framework that circumvents this collapse through a targeted cold-start strategy prioritizing interaction-dense trajectories. We find that a small expert cold-start set of just 4K interaction-dense trajectories yields the strongest downstream performance, establishing a robust prior that enables superior exploration during extended RL training. Extensive evaluations demonstrate that ASTER-4B achieves state-of-the-art results on competitive mathematical benchmarks, reaching 90.0% on AIME 2025, surpassing leading frontier open-source models, including DeepSeek-V3.2-Exp.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.01204v1)
