---
type: source
source_type: arxiv
title: "MPAC: A Multi-Principal Agent Coordination Protocol for Interoperable Multi-Agent Collaboration"
authors: Kaiyang Qian, Xinmin Fang, Zhengxiong Li
url: https://arxiv.org/abs/2604.09744v1
date: 2026-04-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.MA
tags: [coding-agents, agent-economies, human-agent-interaction, agent-security, agent-protocols, arxiv, auto-ingested]
---

# MPAC: A Multi-Principal Agent Coordination Protocol for Interoperable Multi-Agent Collaboration

**arXiv:** [2604.09744v1](https://arxiv.org/abs/2604.09744v1) · 2026-04-10 · cs.MA
**Authors:** Kaiyang Qian, Xinmin Fang, Zhengxiong Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The AI agent ecosystem has converged on two protocols: the Model Context Protocol (MCP) for tool invocation and Agent-to-Agent (A2A) for single-principal task delegation. Both assume a single controlling principal, meaning one person or organization that owns every agent. When independent principals' agents must coordinate over shared state, such as engineers' coding agents editing the same repository, family members planning a shared trip, or agents from different organizations negotiating a joint decision, neither protocol applies, and coordination collapses to ad-hoc chat, manual merging, or silent overwrites. We present MPAC (Multi-Principal Agent Coordination Protocol), an application-layer protocol that fills this gap with explicit coordination semantics across five layers: Session, Intent, Operation, Conflict, and Governance. MPAC makes intent declaration a precondition for action, represents conflicts as first-class structured objects, and supports human-in-the-loop arbitration through a pluggable governance layer. The specification defines 21 message types, three state machines with normative transition tables, Lamport-clock causal watermarking, two execution models, three security profiles, and optimistic concurrency control on shared state. We release two interoperable reference implementations in Python and TypeScript with 223 tests, a JSON Schema suite, and seven live multi-agent demos. A controlled three-agent code review benchmark shows a 95 percent reduction in coordination overhead and a 4.8 times wall-clock speedup versus a serialized human-mediated baseline, with per-agent decision time preserved. The speedup comes from eliminating coordination waits, not compressing model calls. Specification, implementations, and demos are open source.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-economies|Agent economies]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]] · [[a2a-protocol]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09744v1)
