---
type: source
source_type: arxiv
title: "Mock Worlds, Real Skills: Building Small Agentic Language Models with Synthetic Tasks, Simulated Environments, and Rubric-Based Rewards"
authors: Yuanjie Lyu, Chengyu Wang, Lei Shen, Jun Huang et al.
url: https://arxiv.org/abs/2601.22511v2
date: 2026-01-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [agentic-rl, agent-skills, tool-use, arxiv, auto-ingested]
---

# Mock Worlds, Real Skills: Building Small Agentic Language Models with Synthetic Tasks, Simulated Environments, and Rubric-Based Rewards

**arXiv:** [2601.22511v2](https://arxiv.org/abs/2601.22511v2) · 2026-01-30 · cs.CL
**Authors:** Yuanjie Lyu, Chengyu Wang, Lei Shen, Jun Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Small LLMs often struggle to match the agentic capabilities of large, costly models. While reinforcement learning can help, progress has been limited by two structural bottlenecks: existing open-source agentic training data are narrow in task variety and easily solved; real-world APIs lack diversity and are unstable for large-scale reinforcement learning rollout processes. We address these challenges with SYNTHAGENT, a framework that jointly synthesizes diverse tool-use training data and simulates complete environments. Specifically, a strong teacher model creates novel tasks and tool ecosystems, then rewrites them into intentionally underspecified instructions. This compels agents to actively query users for missing details. When handling synthetic tasks, an LLM-based user simulator provides user-private information, while a mock tool system delivers stable tool responses. For rewards, task-level rubrics are constructed based on required subgoals, user-agent interactions, and forbidden behaviors. Across 14 challenging datasets in math, search, and tool use, models trained on our synthetic data achieve substantial gains, with small models outperforming larger baselines.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22511v2)
