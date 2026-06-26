---
type: source
source_type: arxiv
title: "Harmonizing Real-Time Constraints and Long-Horizon Reasoning: An Asynchronous Agentic Framework for Dynamic Scheduling"
authors: Shijie Cao, Yuan Yuan, Jing Liu
url: https://arxiv.org/abs/2605.29262v1
date: 2026-05-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [coding-agents, agentic-rl, agent-security, agent-memory, arxiv, auto-ingested]
---

# Harmonizing Real-Time Constraints and Long-Horizon Reasoning: An Asynchronous Agentic Framework for Dynamic Scheduling

**arXiv:** [2605.29262v1](https://arxiv.org/abs/2605.29262v1) · 2026-05-28 · cs.AI
**Authors:** Shijie Cao, Yuan Yuan, Jing Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The Dynamic Flexible Job Shop Scheduling Problem (DFJSP) necessitates a trade-off between instant reaction to stochastic disturbances and global optimization of production goals. Conventional priority rules are insufficiently flexible to handle complex disruptions, whereas learning-based approaches often compromise interpretability or fail to generalize across problem scales. Although Large Language Models (LLMs) offer advanced reasoning capabilities to bridge this gap, their substantial inference latency is incompatible with the millisecond-level decision cycles of industrial control systems. To resolve this conflict, we introduce RACE-Sched, an asynchronous agent-based framework that decouples policy execution from logical reasoning via a dual-stream architecture. The Reactive Stream executes low-latency symbolic heuristics to enable real-time dispatching, while the parallel Deliberative Stream leverages an LLM to synthesize, validate, and evolve these rules. Candidate rules undergo rigorous testing in a sandbox and are deployed via atomic updates, ensuring safety without blocking the control loop. Additionally, a semantic rule repository indexes validated heuristics for retrieval-based initialization which enhances transferability across problem scales. Extensive evaluations on GEN-Bench, MK-Bench, and JMS-Bench demonstrate that RACE-Sched outperforms leading Deep Reinforcement Learning and other LLM-based baselines. This approach harmonizes real-time constraints with long-horizon reasoning to achieve superior solution quality and robust adaptation to dynamic events.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.29262v1)
