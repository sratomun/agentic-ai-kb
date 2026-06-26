---
type: source
source_type: arxiv
title: "From CRUD to Autonomous Agents: Formal Validation and Zero-Trust Security for Semantic Gateways in AI-Native Enterprise Systems"
authors: Ignacio Peyrano
url: https://arxiv.org/abs/2604.25555v1
date: 2026-04-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CR
tags: [coding-agents, human-agent-interaction, agent-security, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# From CRUD to Autonomous Agents: Formal Validation and Zero-Trust Security for Semantic Gateways in AI-Native Enterprise Systems

**arXiv:** [2604.25555v1](https://arxiv.org/abs/2604.25555v1) · 2026-04-28 · cs.CR
**Authors:** Ignacio Peyrano

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enterprise software engineering is shifting away from deterministic CRUD/REST architectures toward AI-native systems where large language models act as cognitive orchestrators. This transition introduces a critical security tension: probabilistic LLMs weaken classical mechanisms for validation, access control, and formal testing. This paper proposes the design, formal validation, and empirical evaluation of a Semantic Gateway governed by the Model Context Protocol (MCP). The gateway reframes the enterprise API as a semantic surface where tools are dynamically discovered, authorized, and executed based on intent and policy enforcement. The central contribution rests on a paradigm shift: autonomous agents must not be validated as traditional software nor as simple API consumers, but as stochastic state-transition systems whose behavior must be abstracted, fuzzed, and audited through enabled-tool graphs. The architecture introduces a three-layer Zero-Trust security model comprising a pre-inference Semantic Firewall, deterministic Tool-Level RBAC, and out-of-band Cryptographic Human-in-the-Loop approval. Enabledness-Preserving Abstractions (EPAs) and greybox semantic fuzzing--originally developed for blockchain smart contract verification--are adapted to audit agent behavior in enterprise environments. Results demonstrate an 84.2% reduction in incidental code. Across 500,000 multi-turn fuzzing sequences, the methodology achieved a 100% discovery rate of hidden unauthorized state transitions, proving that dynamic formal verification is strictly necessary for secure agentic deployment.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.25555v1)
