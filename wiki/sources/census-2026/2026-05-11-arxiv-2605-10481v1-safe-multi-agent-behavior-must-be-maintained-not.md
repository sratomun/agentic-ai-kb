---
type: source
source_type: arxiv
title: "Safe Multi-Agent Behavior Must Be Maintained, Not Merely Asserted: Constraint Drift in LLM-Based Multi-Agent Systems"
authors: Tianxiao Li, Yixing Ma, Haiquan Wen, Zhenglin Huang et al.
url: https://arxiv.org/abs/2605.10481v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.MA
tags: [agentic-rl, agent-security, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Safe Multi-Agent Behavior Must Be Maintained, Not Merely Asserted: Constraint Drift in LLM-Based Multi-Agent Systems

**arXiv:** [2605.10481v1](https://arxiv.org/abs/2605.10481v1) · 2026-05-11 · cs.MA
**Authors:** Tianxiao Li, Yixing Ma, Haiquan Wen, Zhenglin Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern LLM based agents are no longer passive text generators. They read repositories, call tools, browse the web, execute code, maintain memory, communicate with other agents, and act through long horizon workflows. This shift moves the unit of safety. A system may produce a compliant final answer while leaking private information through an internal message, delegating authority beyond its original scope, calling an external tool with sensitive context, or losing the evidence needed to reconstruct why an action was allowed. We argue that many emerging failures in LLM-based multi-agent systems share a common structure: safety critical constraints do not remain operative throughout the trajectory. We call this phenomenon constraint drift: the loss, distortion, weakening, or relaxation of constraints as they pass through memory, delegation, communication, tool use, audit, and optimization. The position taken here is that safe multi-agent behavior must be maintained, not merely asserted. Prompts, guardrails, tool schemas, access control, and final output checks are necessary, but they are insufficient unless constraints remain fresh, inherited, enforceable, and auditable across execution. We propose Constraint State Governance as a research paradigm for LLM-based multi-agent systems. In this paradigm, safety-critical constraints are maintained as explicit execution state, while constraint-native reinforcement learning improves utility only within maintained safety boundaries. The goal is not to freeze agentic systems under rigid rules, but to make safety operational across the trajectories through which modern agents actually act.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10481v1)
