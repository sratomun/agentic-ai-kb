---
type: source
source_type: arxiv
title: "Drift-Bench: Diagnosing Cooperative Breakdowns in LLM Agents under Input Faults via Multi-Turn Interaction"
authors: Han Bao, Zheyuan Zhang, Pengcheng Jing, Zhengqing Yuan et al.
url: https://arxiv.org/abs/2602.02455v1
date: 2026-02-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, agent-reliability, agent-security, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# Drift-Bench: Diagnosing Cooperative Breakdowns in LLM Agents under Input Faults via Multi-Turn Interaction

**arXiv:** [2602.02455v1](https://arxiv.org/abs/2602.02455v1) · 2026-02-02 · cs.AI
**Authors:** Han Bao, Zheyuan Zhang, Pengcheng Jing, Zhengqing Yuan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As Large Language Models transition to autonomous agents, user inputs frequently violate cooperative assumptions (e.g., implicit intent, missing parameters, false presuppositions, or ambiguous expressions), creating execution risks that text-only evaluations do not capture. Existing benchmarks typically assume well-specified instructions or restrict evaluation to text-only, single-turn clarification, and thus do not measure multi-turn disambiguation under grounded execution risk. We introduce \textbf{Drift-Bench}, the first diagnostic benchmark that evaluates agentic pragmatics under input faults through multi-turn clarification across state-oriented and service-oriented execution environments. Grounded in classical theories of communication, \textbf{Drift-Bench} provides a unified taxonomy of cooperative breakdowns and employs a persona-driven user simulator with the \textbf{Rise} evaluation protocol. Experiments show substantial performance drops under these faults, with clarification effectiveness varying across user personas and fault types. \MethodName bridges clarification research and agent safety evaluation, enabling systematic diagnosis of failures that can lead to unsafe executions.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.02455v1)
