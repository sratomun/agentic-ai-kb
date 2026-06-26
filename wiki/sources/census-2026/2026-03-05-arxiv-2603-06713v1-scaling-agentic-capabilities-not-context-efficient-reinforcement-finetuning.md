---
type: source
source_type: arxiv
title: "Scaling Agentic Capabilities, Not Context: Efficient Reinforcement Finetuning for Large Toolspaces"
authors: Karan Gupta, Pranav Vajreshwari, Yash Pandya, Raghav Magazine et al.
url: https://arxiv.org/abs/2603.06713v1
date: 2026-03-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [agentic-rl, agent-protocols, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Scaling Agentic Capabilities, Not Context: Efficient Reinforcement Finetuning for Large Toolspaces

**arXiv:** [2603.06713v1](https://arxiv.org/abs/2603.06713v1) · 2026-03-05 · cs.LG
**Authors:** Karan Gupta, Pranav Vajreshwari, Yash Pandya, Raghav Magazine et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic systems operating over large tool ecosystems must plan and execute long-horizon workflows under weak or non-verifiable supervision. While frontier models mitigate these challenges through scale and large context budgets, small language models (SLMs) remain brittle: eager tool loading saturates context, execution errors compound over time, and sparse rewards limit learning. We introduce ATLAS, a reinforcement finetuning framework that enables SLMs to operate effectively in large-scale toolspace environments by learning how to acquire context and how to execute actions. Our approach makes two key contributions. First, we treat context control and execution structure as learnable decisions, combining iterative tool loading with programmatic tool orchestration to bound context growth and stabilize long-horizon trajectories. Second, we propose rubric-based reinforcement finetuning, which decomposes task success into structured, task-aligned criteria and enables scalable training using small judge models. Across MCP benchmarks, these design choices yield large and consistent gains over generic RL baselines, allowing a 4B SLM to approach frontier-agent performance under far tighter parameter and context budgets.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.06713v1)
