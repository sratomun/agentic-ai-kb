---
type: source
source_type: arxiv
title: "Agent World Model: Infinity Synthetic Environments for Agentic Reinforcement Learning"
authors: Zhaoyang Wang, Canwen Xu, Boyi Liu, Yite Wang et al.
url: https://arxiv.org/abs/2602.10090v3
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Agent World Model: Infinity Synthetic Environments for Agentic Reinforcement Learning

**arXiv:** [2602.10090v3](https://arxiv.org/abs/2602.10090v3) · 2026-02-10 · cs.AI
**Authors:** Zhaoyang Wang, Canwen Xu, Boyi Liu, Yite Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in large language model (LLM) have empowered autonomous agents to perform multi-turn interactions with tools and environments. However, scaling such agent training is limited by the lack of diverse and reliable environments. In this paper, we propose Agent World Model (AWM), a fully synthetic environment generation pipeline. Using this pipeline, we scale to 1,000 environments covering everyday scenarios, in which agents can interact with rich toolsets and obtain high-quality observations. Notably, these environments are code-driven and backed by databases, providing more reliable and consistent state transitions than environments simulated by LLMs. Moreover, they enable more efficient agent interaction compared with collecting trajectories from realistic environments. To demonstrate the effectiveness of this resource, we perform large-scale reinforcement learning for multi-turn tool-use agents. Thanks to the fully executable environments and accessible database states, we can also design reliable reward functions. Experiments on three benchmarks show that training exclusively in synthetic environments, rather than benchmark-specific ones, yields strong out-of-distribution generalization. The code is available at https://github.com/Snowflake-Labs/agent-world-model.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.10090v3)
