---
type: source
source_type: arxiv
title: "CaveAgent: Transforming LLMs into Stateful Runtime Operators"
authors: Maohao Ran, Zhenglin Wan, Cooper Lin, Yanting Zhang et al.
url: https://arxiv.org/abs/2601.01569v3
date: 2026-01-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [coding-agents, agentic-rl, agent-protocols, agent-skills, agent-memory, arxiv, auto-ingested]
---

# CaveAgent: Transforming LLMs into Stateful Runtime Operators

**arXiv:** [2601.01569v3](https://arxiv.org/abs/2601.01569v3) · 2026-01-04 · cs.AI
**Authors:** Maohao Ran, Zhenglin Wan, Cooper Lin, Yanting Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents are increasingly capable of complex task execution, yet current agentic systems remain constrained by text-centric paradigms that struggle with long-horizon tasks due to fragile multi-turn dependencies and context drift. We present CaveAgent, a framework that shifts tool use from ``LLM-as-Text-Generator'' to ``LLM-as-Runtime-Operator.'' CaveAgent introduces a dual-stream architecture that inverts the conventional paradigm: rather than treating the LLM's text context as the primary workspace with tools as auxiliary, CaveAgent elevates the persistent Python runtime as the central locus of state, with a lightweight semantic stream serving as its orchestrator. Beyond leveraging code generation to resolve interdependent sub-tasks (e.g., loops, conditionals) in a single step, CaveAgent introduces \textit{Stateful Runtime Management}: it injects, manipulates, and retrieves complex Python objects (e.g., DataFrames, database connections) that persist across turns, unlike existing code-based approaches that remain text-bound. CaveAgent further provides a runtime-integrated skill management system that extends the Agent Skills open standard, enabling ecosystem interoperability through executable skill injections. This persistence mechanism serves as a high-fidelity external memory that reduces context drift in multi-turn interactions and preserves processed data for downstream applications without information loss. Evaluations show consistent improvement across challenging benchmarks, enabling CaveAgent to handle data scales that cause context overflow in both JSON-based and code-based agents. The accessible runtime state further provides programmatically verifiable feedback, enabling automated evaluation and reward signal generation without human annotation and establishing a structural foundation for future research in Reinforcement Learning with Verifiable Rewards (RLVR).

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.01569v3)
