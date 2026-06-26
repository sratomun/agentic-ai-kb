---
type: source
source_type: arxiv
title: "HiMAP-Travel: Hierarchical Multi-Agent Planning for Long-Horizon Constrained Travel"
authors: The Viet Bui, Wenjun Li, Yong Liu
url: https://arxiv.org/abs/2603.04750v1
date: 2026-03-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agentic-rl, agent-protocols, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# HiMAP-Travel: Hierarchical Multi-Agent Planning for Long-Horizon Constrained Travel

**arXiv:** [2603.04750v1](https://arxiv.org/abs/2603.04750v1) · 2026-03-05 · cs.AI
**Authors:** The Viet Bui, Wenjun Li, Yong Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Sequential LLM agents fail on long-horizon planning with hard constraints like budgets and diversity requirements. As planning progresses and context grows, these agents drift from global constraints. We propose HiMAP-Travel, a hierarchical multi-agent framework that splits planning into strategic coordination and parallel day-level execution. A Coordinator allocates resources across days, while Day Executors plan independently in parallel. Three key mechanisms enable this: a transactional monitor enforcing budget and uniqueness constraints across parallel agents, a bargaining protocol allowing agents to reject infeasible sub-goals and trigger re-planning, and a single policy trained with GRPO that powers all agents through role conditioning. On TravelPlanner, HiMAP-Travel with Qwen3-8B achieves 52.78% validation and 52.65% test Final Pass Rate (FPR). In a controlled comparison with identical model, training, and tools, it outperforms the sequential DeepTravel baseline by +8.67~pp. It also surpasses ATLAS by +17.65~pp and MTP by +10.0~pp. On FlexTravelBench multi-turn scenarios, it achieves 44.34% (2-turn) and 37.42% (3-turn) FPR while reducing latency 2.5x through parallelization.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.04750v1)
