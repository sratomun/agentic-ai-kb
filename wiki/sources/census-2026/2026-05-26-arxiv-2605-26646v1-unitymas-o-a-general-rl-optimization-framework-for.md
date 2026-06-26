---
type: source
source_type: arxiv
title: "UnityMAS-O: A General RL Optimization Framework for LLM-Based Multi-Agent Systems"
authors: Yiqun Chen, Wei Yang, Erhan Zhang, Shijie Wang et al.
url: https://arxiv.org/abs/2605.26646v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, agentic-rl, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# UnityMAS-O: A General RL Optimization Framework for LLM-Based Multi-Agent Systems

**arXiv:** [2605.26646v1](https://arxiv.org/abs/2605.26646v1) · 2026-05-26 · cs.AI
**Authors:** Yiqun Chen, Wei Yang, Erhan Zhang, Shijie Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based multi-agent systems decompose complex tasks into interacting roles, but most remain manually orchestrated by prompts, tools, and control rules, while agents are rarely optimized through a unified reinforcement learning interface. Existing RL post-training frameworks mainly target single-policy optimization and lack abstractions for user-defined multi-agent workflows, structured interaction, role-specific credit assignment, and configurable parameter sharing. We present UnityMAS-O, a general RL optimization framework for LLM-based multi-agent systems. UnityMAS-O treats the complete workflow as the optimization unit, rather than a single response or policy trajectory. It represents workflows through four first-class objects: logical agent roles, graph trajectories, user-defined rewards, and agent--model mappings. This decouples logical agents from physical model parameters, supporting full sharing, full separation, and partial sharing, with rewards assigned at role, turn, and trajectory levels. UnityMAS-O extends verl with a Ray-based star-topology runtime. A central controller executes workflows, invokes tools, records structured trajectories, and assembles rewards; model-local worker groups handle rollout, buffering, advantage computation, and distributed PPO-style updates. Users can define agents, workflows, model mappings, and rewards without rewriting the optimization infrastructure. We instantiate UnityMAS-O on retrieval-augmented QA, iterative agentic search, and reflective code generation. Across Natural Questions, HotpotQA, and held-out code tasks, multi-agent RL improves manually specified workflows after optimization, with especially large gains for smaller models and strict code all-passed metrics. These results show that UnityMAS-O can serve as a reusable substrate for converting diverse LLM-based multi-agent workflows into trainable multi-agent RL systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[ppo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26646v1)
