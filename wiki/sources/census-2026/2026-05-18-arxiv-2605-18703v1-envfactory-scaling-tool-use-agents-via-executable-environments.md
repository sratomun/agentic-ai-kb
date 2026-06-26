---
type: source
source_type: arxiv
title: "EnvFactory: Scaling Tool-Use Agents via Executable Environments Synthesis and Robust RL"
authors: Minrui Xu, Zilin Wang, Mengyi DENG, Zhiwei Li et al.
url: https://arxiv.org/abs/2605.18703v1
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agentic-rl, agent-protocols, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# EnvFactory: Scaling Tool-Use Agents via Executable Environments Synthesis and Robust RL

**arXiv:** [2605.18703v1](https://arxiv.org/abs/2605.18703v1) · 2026-05-18 · cs.CL
**Authors:** Minrui Xu, Zilin Wang, Mengyi DENG, Zhiwei Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Equipping LLMs with tool-use capabilities via Agentic Reinforcement Learning (Agentic RL) is bottlenecked by two challenges: the lack of scalable, robust execution environments and the scarcity of realistic training data that captures implicit human reasoning. Existing approaches depend on costly real-world APIs, hallucination-prone LLM simulators, or synthetic environments that are often single-turn or depend on pre-collected documents. Moreover, synthetic trajectories are frequently over-specified, resembling instruction sequences rather than natural human intents, reducing their effectiveness for RL training. We introduce EnvFactory, a fully automated framework that addresses both challenges. EnvFactory autonomously explores and verifies stateful, executable tool environments from authentic resources, and synthesizes natural multi-turn trajectories through topology-aware sampling and calibrated refinement, producing grounded queries with implicit intents. Using only 85 verified environments across 7 domains, EnvFactory generates 2,575 SFT and RL trajectories. Despite using significantly fewer environments than prior work, which are often 5 times more, EnvFactory achieves superior training efficiency and downstream performance, improving Qwen3-series models by up to +15% on BFCLv3, +8.6% on MCP-Atlas, and +6% on conversational benchmarks including $τ^2$-Bench and VitaBench. By fully automating both environment construction and trajectory synthesis, EnvFactory provides a scalable, extensible, and robust foundation for Agentic RL.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.18703v1)
