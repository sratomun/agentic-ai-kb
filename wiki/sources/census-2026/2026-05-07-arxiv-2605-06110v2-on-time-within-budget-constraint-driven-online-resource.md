---
type: source
source_type: arxiv
title: "On Time, Within Budget: Constraint-Driven Online Resource Allocation for Agentic Workflows"
authors: Xinglin Wang, Zishen Liu, Shaoxiong Feng, Peiwen Yuan et al.
url: https://arxiv.org/abs/2605.06110v2
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [finance-agents, multi-agent-systems, arxiv, auto-ingested]
---

# On Time, Within Budget: Constraint-Driven Online Resource Allocation for Agentic Workflows

**arXiv:** [2605.06110v2](https://arxiv.org/abs/2605.06110v2) · 2026-05-07 · cs.AI
**Authors:** Xinglin Wang, Zishen Liu, Shaoxiong Feng, Peiwen Yuan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic systems increasingly solve complex user requests by executing orchestrated workflows, where subtasks are assigned to specialized models or tools and coordinated according to their dependencies. While recent work improves agent efficiency by optimizing the performance--cost--latency frontier, real deployments often impose concrete requirements: a workflow must be completed within a specified budget and before a specified deadline. This shifts the goal from average efficiency optimization to maximizing the probability that the entire workflow completes successfully under explicit budget and deadline constraints. We study \emph{constraint-driven online resource allocation for agentic workflows}. Given a dependency-structured workflow and estimates of success rates and generation lengths for each subtask--model pair, the executor dynamically allocates models and parallel samples across simultaneously executable subtasks while managing the remaining budget and time. We formulate this setting as a finite-horizon stochastic online allocation problem and propose \emph{Monte Carlo Portfolio Planning} (MCPP), a lightweight closed-loop planner that directly estimates constrained completion probability through simulated workflow executions and replans after observed outcomes. Experiments on CodeFlow and ProofFlow demonstrate that MCPP consistently improves constrained completion probability over strong baselines across a wide range of budget--deadline constraints.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.06110v2)
