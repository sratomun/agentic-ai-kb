---
type: source
source_type: arxiv
title: "Beyond Single-Shot: Multi-step Tool Retrieval via Query Planning"
authors: Wei Fang, James Glass
url: https://arxiv.org/abs/2601.07782v1
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# Beyond Single-Shot: Multi-step Tool Retrieval via Query Planning

**arXiv:** [2601.07782v1](https://arxiv.org/abs/2601.07782v1) · 2026-01-12 · cs.CL
**Authors:** Wei Fang, James Glass

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM agents operating over massive, dynamic tool libraries rely on effective retrieval, yet standard single-shot dense retrievers struggle with complex requests. These failures primarily stem from the disconnect between abstract user goals and technical documentation, and the limited capacity of fixed-size embeddings to model combinatorial tool compositions. To address these challenges, we propose TOOLQP, a lightweight framework that models retrieval as iterative query planning. Instead of single-shot matching, TOOLQP decomposes instructions into sub-tasks and dynamically generates queries to interact with the retriever, effectively bridging the semantic gap by targeting the specific sub-tasks required for composition. We train TOOLQP using synthetic query trajectories followed by optimization via Reinforcement Learning with Verifiable Rewards (RLVR). Experiments demonstrate that TOOLQP achieves state-of-the-art performance, exhibiting superior zero-shot generalization, robustness across diverse retrievers, and significant improvements in downstream agentic execution.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.07782v1)
