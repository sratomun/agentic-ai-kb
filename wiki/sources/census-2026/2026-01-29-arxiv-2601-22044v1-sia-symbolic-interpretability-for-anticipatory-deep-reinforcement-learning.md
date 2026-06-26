---
type: source
source_type: arxiv
title: "SIA: Symbolic Interpretability for Anticipatory Deep Reinforcement Learning in Network Control"
authors: MohammadErfan Jabbari, Abhishek Duttagupta, Claudio Fiandrino, Leonardo Bonati et al.
url: https://arxiv.org/abs/2601.22044v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.NI
tags: [knowledge-graph, agentic-rl, arxiv, auto-ingested]
---

# SIA: Symbolic Interpretability for Anticipatory Deep Reinforcement Learning in Network Control

**arXiv:** [2601.22044v1](https://arxiv.org/abs/2601.22044v1) · 2026-01-29 · cs.NI
**Authors:** MohammadErfan Jabbari, Abhishek Duttagupta, Claudio Fiandrino, Leonardo Bonati et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deep reinforcement learning (DRL) promises adaptive control for future mobile networks but conventional agents remain reactive: they act on past and current measurements and cannot leverage short-term forecasts of exogenous KPIs such as bandwidth. Augmenting agents with predictions can overcome this temporal myopia, yet uptake in networking is scarce because forecast-aware agents act as closed-boxes; operators cannot tell whether predictions guide decisions or justify the added complexity. We propose SIA, the first interpreter that exposes in real time how forecast-augmented DRL agents operate. SIA fuses Symbolic AI abstractions with per-KPI Knowledge Graphs to produce explanations, and includes a new Influence Score metric. SIA achieves sub-millisecond speed, over 200x faster than existing XAI methods. We evaluate SIA on three diverse networking use cases, uncovering hidden issues, including temporal misalignment in forecast integration and reward-design biases that trigger counter-productive policies. These insights enable targeted fixes: a redesigned agent achieves a 9% higher average bitrate in video streaming, and SIA's online Action-Refinement module improves RAN-slicing reward by 25% without retraining. By making anticipatory DRL transparent and tunable, SIA lowers the barrier to proactive control in next-generation mobile networks.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22044v1)
