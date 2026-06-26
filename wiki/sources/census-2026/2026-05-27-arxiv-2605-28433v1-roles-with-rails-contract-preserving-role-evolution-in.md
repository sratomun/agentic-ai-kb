---
type: source
source_type: arxiv
title: "Roles with Rails: Contract-Preserving Role Evolution in Multi-Agent Structured Reasoning"
authors: Ling-Yue Ge, Lan-Zhe Guo
url: https://arxiv.org/abs/2605.28433v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [self-evolving-agents, agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Roles with Rails: Contract-Preserving Role Evolution in Multi-Agent Structured Reasoning

**arXiv:** [2605.28433v1](https://arxiv.org/abs/2605.28433v1) · 2026-05-27 · cs.CL
**Authors:** Ling-Yue Ge, Lan-Zhe Guo

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Role-based LLM multi-agent systems need adaptive role pools, yet adapting such systems is not merely a matter of prompt optimization: roles often carry structural obligations, including capability coverage, message compatibility, validation, final-answer aggregation, and parser-compatible output protocols. Existing systems either fix the role inventory and lose adaptivity, or allow unconstrained generation to induce role drift, removing structurally necessary roles and breaking answer contracts. We formulate this as contract-preserving role evolution, requiring every committed edit to preserve five structural contracts (capability, communication, validation, aggregation, output protocol). We instantiate this formulation in SERO, a Self-Evolving Role Orchestration framework that evolves a typed role-card pool through credit-guided retrieval, a credit-ranked communication DAG with a protected terminal aggregator and conditional validator repair, and a contextual-bandit controller whose LLM-proposed edits are committed only when they preserve the contracts and improve task score. Experiments on real-world reasoning benchmarks across three LLM backbones confirm the value of contract-preserving role evolution.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28433v1)
