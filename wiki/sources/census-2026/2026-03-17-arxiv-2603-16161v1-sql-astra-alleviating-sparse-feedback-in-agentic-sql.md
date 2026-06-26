---
type: source
source_type: arxiv
title: "SQL-ASTRA: Alleviating Sparse Feedback in Agentic SQL via Column-Set Matching and Trajectory Aggregation"
authors: Long Li, Zhijian Zhou, Jiangxuan Long, Peiyang Liu et al.
url: https://arxiv.org/abs/2603.16161v1
date: 2026-03-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [data-query-agents, agentic-rl, arxiv, auto-ingested]
---

# SQL-ASTRA: Alleviating Sparse Feedback in Agentic SQL via Column-Set Matching and Trajectory Aggregation

**arXiv:** [2603.16161v1](https://arxiv.org/abs/2603.16161v1) · 2026-03-17 · cs.AI
**Authors:** Long Li, Zhijian Zhou, Jiangxuan Long, Peiyang Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Reinforcement Learning (RL) shows promise for complex tasks, but Text-to-SQL remains mostly restricted to single-turn paradigms. A primary bottleneck is the credit assignment problem. In traditional paradigms, rewards are determined solely by the final-turn feedback, which ignores the intermediate process and leads to ambiguous credit evaluation. To address this, we propose Agentic SQL, a framework featuring a universal two-tiered reward mechanism designed to provide effective trajectory-level evaluation and dense step-level signals. First, we introduce Aggregated Trajectory Reward (ATR) to resolve multi-turn credit assignment. Using an asymmetric transition matrix, ATR aggregates process-oriented scores to incentivize continuous improvement. Leveraging Lyapunov stability theory, we prove ATR acts as an energy dissipation operator, guaranteeing a cycle-free policy and monotonic convergence. Second, Column-Set Matching Reward (CSMR) provides immediate step-level rewards to mitigate sparsity. By executing queries at each turn, CSMR converts binary (0/1) feedback into dense [0, 1] signals based on partial correctness. Evaluations on BIRD show a 5% gain over binary-reward GRPO. Notably, our approach outperforms SOTA Arctic-Text2SQL-R1-7B on BIRD and Spider 2.0 using identical models, propelling Text-to-SQL toward a robust multi-turn agent paradigm.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rl|Agentic RL]]
- **Entities:** [[bird-benchmark]] · [[spider-benchmark]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.16161v1)
