---
type: source
source_type: arxiv
title: "Collaborative Multi-Agent Test-Time Reinforcement Learning for Reasoning"
authors: Zhiyuan Hu, Yunhai Hu, Juncheng Liu, Shuyue Stella Li et al.
url: https://arxiv.org/abs/2601.09667v2
date: 2026-01-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agent-reliability, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Collaborative Multi-Agent Test-Time Reinforcement Learning for Reasoning

**arXiv:** [2601.09667v2](https://arxiv.org/abs/2601.09667v2) · 2026-01-14 · cs.AI
**Authors:** Zhiyuan Hu, Yunhai Hu, Juncheng Liu, Shuyue Stella Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent systems have evolved into practical LLM-driven collaborators for many applications, gaining robustness from diversity and cross-checking. However, multi-agent RL (MARL) training is resource-intensive and unstable: co-adapting teammates induce non-stationarity, and rewards are often sparse and high-variance. Therefore, we introduce \textbf{Multi-Agent Test-Time Reinforcement Learning (MATTRL)}, a framework that injects structured textual experience into multi-agent deliberation at inference time. MATTRL forms a multi-expert team of specialists for multi-turn discussions, retrieves and integrates test-time experiences, and reaches consensus for final decision-making. We also study credit assignment for constructing a turn-level experience pool, then reinjecting it into the dialogue. Across challenging benchmarks in medicine, math, and education, MATTRL improves accuracy by an average of 3.67\% over a multi-agent baseline, and by 8.67\% over comparable single-agent baselines. Ablation studies examine different credit-assignment schemes and provide a detailed comparison of how they affect training outcomes. MATTRL offers a stable, effective and efficient path to distribution-shift-robust multi-agent reasoning without tuning.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.09667v2)
