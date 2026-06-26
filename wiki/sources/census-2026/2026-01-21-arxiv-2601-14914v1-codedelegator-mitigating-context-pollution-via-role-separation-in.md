---
type: source
source_type: arxiv
title: "CodeDelegator: Mitigating Context Pollution via Role Separation in Code-as-Action Agents"
authors: Tianxiang Fei, Cheng Chen, Yue Pan, Mao Zheng et al.
url: https://arxiv.org/abs/2601.14914v1
date: 2026-01-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [human-agent-interaction, agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# CodeDelegator: Mitigating Context Pollution via Role Separation in Code-as-Action Agents

**arXiv:** [2601.14914v1](https://arxiv.org/abs/2601.14914v1) · 2026-01-21 · cs.CL
**Authors:** Tianxiang Fei, Cheng Chen, Yue Pan, Mao Zheng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in large language models (LLMs) allow agents to represent actions as executable code, offering greater expressivity than traditional tool-calling. However, real-world tasks often demand both strategic planning and detailed implementation. Using a single agent for both leads to context pollution from debugging traces and intermediate failures, impairing long-horizon performance. We propose CodeDelegator, a multi-agent framework that separates planning from implementation via role specialization. A persistent Delegator maintains strategic oversight by decomposing tasks, writing specifications, and monitoring progress without executing code. For each sub-task, a new Coder agent is instantiated with a clean context containing only its specification, shielding it from prior failures. To coordinate between agents, we introduce Ephemeral-Persistent State Separation (EPSS), which isolates each Coder's execution state while preserving global coherence, preventing debugging traces from polluting the Delegator's context. Experiments on various benchmarks demonstrate the effectiveness of CodeDelegator across diverse scenarios.

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.14914v1)
