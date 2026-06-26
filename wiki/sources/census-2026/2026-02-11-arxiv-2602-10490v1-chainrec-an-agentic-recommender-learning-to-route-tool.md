---
type: source
source_type: arxiv
title: "ChainRec: An Agentic Recommender Learning to Route Tool Chains for Diverse and Evolving Interests"
authors: Fuchun Li, Qian Li, Xingyu Gao, Bocheng Pan et al.
url: https://arxiv.org/abs/2602.10490v1
date: 2026-02-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.IR
tags: [recommendation-agents, arxiv, auto-ingested]
---

# ChainRec: An Agentic Recommender Learning to Route Tool Chains for Diverse and Evolving Interests

**arXiv:** [2602.10490v1](https://arxiv.org/abs/2602.10490v1) · 2026-02-11 · cs.IR
**Authors:** Fuchun Li, Qian Li, Xingyu Gao, Bocheng Pan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are increasingly integrated into recommender systems, motivating recent interest in agentic and reasoning-based recommendation. However, most existing approaches still rely on fixed workflows, applying the same reasoning procedure across diverse recommendation scenarios. In practice, user contexts vary substantially-for example, in cold-start settings or during interest shifts, so an agent should adaptively decide what evidence to gather next rather than following a scripted process. To address this, we propose ChainRec, an agentic recommender that uses a planner to dynamically select reasoning tools. ChainRec builds a standardized Tool Agent Library from expert trajectories. It then trains a planner using supervised fine-tuning and preference optimization to dynamically select tools, decide their order, and determine when to stop. Experiments on AgentRecBench across Amazon, Yelp, and Goodreads show that ChainRec consistently improves Avg HR@{1,3,5} over strong baselines, with especially notable gains in cold-start and evolving-interest scenarios. Ablation studies further validate the importance of tool standardization and preference-optimized planning.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.10490v1)
