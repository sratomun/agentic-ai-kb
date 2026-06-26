---
type: source
source_type: arxiv
title: "CoSearch: Joint Training of Reasoning and Document Ranking via Reinforcement Learning for Agentic Search"
authors: Hansi Zeng, Liam Collins, Bhuvesh Kumar, Neil Shah et al.
url: https://arxiv.org/abs/2604.17555v2
date: 2026-04-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# CoSearch: Joint Training of Reasoning and Document Ranking via Reinforcement Learning for Agentic Search

**arXiv:** [2604.17555v2](https://arxiv.org/abs/2604.17555v2) · 2026-04-19 · cs.AI
**Authors:** Hansi Zeng, Liam Collins, Bhuvesh Kumar, Neil Shah et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic search -- the task of training agents that iteratively reason, issue queries, and synthesize retrieved information to answer complex questions -- has achieved remarkable progress through reinforcement learning (RL). However, existing approaches such as Search-R1, treat the retrieval system as a fixed tool, optimizing only the reasoning agent while the retrieval component remains unchanged. A preliminary experiment reveals that the gap between an oracle and a fixed retrieval system reaches up to +26.8% relative F1 improvement across seven QA benchmarks, suggesting that the retrieval system is a key bottleneck in scaling agentic search performance. Motivated by this finding, we propose CoSearch, a framework that jointly trains a multi-step reasoning agent and a generative document ranking model via Group Relative Policy Optimization (GRPO). To enable effective GRPO training for the ranker -- whose inputs vary across reasoning trajectories -- we introduce a semantic grouping strategy that clusters sub-queries by token-level similarity, forming valid optimization groups without additional rollouts. We further design a composite reward combining ranking quality signals with trajectory-level outcome feedback, providing the ranker with both immediate and long-term learning signals. Experiments on seven single-hop and multi-hop QA benchmarks demonstrate consistent improvements over strong baselines, with ablation studies validating each design choice. Our results show that joint training of the reasoning agent and retrieval system is both feasible and strongly performant, pointing to a key ingredient for future search agents.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17555v2)
