---
type: source
source_type: arxiv
title: "Multi-Agent Computer Use"
authors: Jing Yu Koh, Ruslan Salakhutdinov, Daniel Fried
url: https://arxiv.org/abs/2606.01533v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [computer-use-agents, embodied-agents, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Multi-Agent Computer Use

**arXiv:** [2606.01533v1](https://arxiv.org/abs/2606.01533v1) · 2026-06-01 · cs.MA
**Authors:** Jing Yu Koh, Ruslan Salakhutdinov, Daniel Fried

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Computer use agents (CUAs) today are primarily deployed as single serial agents. This setup is suboptimal for complex long-horizon tasks that benefit from task decomposition, parallel execution, and consistent re-planning based on new information. In this paper, we argue that we should instead move towards evaluating and building multi-agent computer use (MACU) systems. These systems, which emphasize planning and parallel execution, alleviate many of the shortcomings of single-agent CUAs. We propose a general multi-agent setup in which a manager model decomposes computer use tasks as a directed acyclic graph (DAG), encoding relevant dependencies and goals for subagents. At each iteration, the manager dispatches parallel CUA subagents to carry out nodes on the ready frontier of the DAG, and continuously revises the DAG (adding, canceling, or rewriting nodes) as new findings arrive from subagents. This design treats the partially observable environment of computer use as a first class challenge: information that downstream agents may not be able to re-observe are retained and passed forward through the manager and DAG structure. We demonstrate that MACU consistently improves over strong single-agent baselines by $3.4-25.5\%$ on desktop (OSWorld) and web navigation (Online-Mind2Web, WebTailBench, Odysseys) benchmarks, exhibits more favorable test-time scaling, and solves complex long-horizon tasks where single-agent CUAs get stuck. On Odysseys, a long-horizon web navigation benchmark, MACU improves average task completion wall-clock time by ${\sim} 1.5 \times$, demonstrating its efficacy in speeding up traditionally slow CUA pipelines. Our findings highlight that multi-agent coordination is a promising axis for scaling computer use agents to work productively for longer and more effectively. We release all code and interactive visualizations at https://jykoh.com/multi-agent-computer-use.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[osworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01533v1)
