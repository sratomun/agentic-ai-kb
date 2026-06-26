---
type: source
source_type: arxiv
title: "IntentCUA: Learning Intent-level Representations for Skill Abstraction and Multi-Agent Planning in Computer-Use Agents"
authors: Seoyoung Lee, Seobin Yoon, Seongbeen Lee et al.
url: https://arxiv.org/abs/2602.17049v2
date: 2026-02-19
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [intent-understanding, computer-use-agents, agent-memory, arxiv, auto-ingested]
---

# IntentCUA: Learning Intent-level Representations for Skill Abstraction and Multi-Agent Planning in Computer-Use Agents

**arXiv:** [2602.17049v2](https://arxiv.org/abs/2602.17049v2) · 2026-02-19 · cs.AI
**Authors:** Seoyoung Lee, Seobin Yoon, Seongbeen Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
Computer-use agents operate over long horizons under noisy perception, multi-window contexts, evolving environment states. Existing approaches, from RL-based planners to trajectory retrieval, often drift from user intent and repeatedly solve routine subproblems, leading to error accumulation and inefficiency. We present IntentCUA, a multi-agent computer-use framework designed to stabilize long-horizon execution through intent-aligned plan memory. A Planner, Plan-Optimizer, and Critic coordinate over shared memory that abstracts raw interaction traces into multi-view intent representations and reusable skills. At runtime, intent prototypes retrieve subgroup-aligned skills and inject them into partial plans, reducing redundant re-planning and mitigating error propagation across desktop applications. In end-to-end evaluations, IntentCUA achieved a 74.83% task success rate with a Step Efficiency Ratio of 0.91, outperforming RL-based and trajectory-centric baselines. Ablations show that multi-view intent abstraction and shared plan memory jointly improve execution stability, with the cooperative multi-agent loop providing the largest gains on long-horizon tasks. These results highlight that system-level intent abstraction and memory-grounded coordination are key to reliable and efficient desktop automation in large, dynamic environments.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[computer-use-agents|Computer-use agents]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.17049v2)
