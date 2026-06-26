---
type: source
source_type: arxiv
title: "KAIJU: An Executive Kernel for Intent-Gated Execution of LLM Agents"
authors: Cormac Guerin, Frank Guerin
url: https://arxiv.org/abs/2604.02375v1
date: 2026-03-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.SE
tags: [agent-security, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# KAIJU: An Executive Kernel for Intent-Gated Execution of LLM Agents

**arXiv:** [2604.02375v1](https://arxiv.org/abs/2604.02375v1) · 2026-03-31 · cs.SE
**Authors:** Cormac Guerin, Frank Guerin

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-calling autonomous agents based on large language models using ReAct exhibit three limitations: serial latency, quadratic context growth, and vulnerability to prompt injection and hallucination. Recent work moves towards separating planning from execution but in each case the model remains coupled to the execution mechanics. We introduce a system-level abstraction for LLM agents which decouples the execution of agent workflows from the LLM reasoning layer. We define two first-class abstractions: (1) Intent-Gated Execution (IGX), a security paradigm that enforces intent at execution, and (2) an Executive Kernel that manages scheduling, tool dispatch, dependency resolution, failures and security. In KAIJU, the LLM plans upfront, optimistically scheduling tools in parallel with dependency-aware parameter injection. Tools are authorised via IGX based on four independent variables: scope, intent, impact, and clearance (external approval). KAIJU supports three adaptive execution modes (Reflect, nReflect, and Orchestrator), providing progressively finer-grained execution control apt for complex investigation and deep analysis or research. Empirical evaluation against a ReAct baseline shows that KAIJU has a latency penalty on simple queries due to planning overhead, convergence at moderate complexity, and a structural advantage on computational queries requiring parallel data gathering. Beyond latency, the separation enforces behavioural guarantees that ReAct cannot match through prompting alone. Code available at https://github.com/compdeep/kaiju

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.02375v1)
