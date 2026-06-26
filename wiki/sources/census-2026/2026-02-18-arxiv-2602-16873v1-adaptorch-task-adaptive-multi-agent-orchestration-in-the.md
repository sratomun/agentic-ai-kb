---
type: source
source_type: arxiv
title: "AdaptOrch: Task-Adaptive Multi-Agent Orchestration in the Era of LLM Performance Convergence"
authors: Geunbin Yu
url: https://arxiv.org/abs/2602.16873v1
date: 2026-02-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.MA
tags: [coding-agents, agent-protocols, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AdaptOrch: Task-Adaptive Multi-Agent Orchestration in the Era of LLM Performance Convergence

**arXiv:** [2602.16873v1](https://arxiv.org/abs/2602.16873v1) · 2026-02-18 · cs.MA
**Authors:** Geunbin Yu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As large language models from diverse providers converge toward comparable benchmark performance, the traditional paradigm of selecting a single best model per task yields diminishing returns. We argue that orchestration topology -- the structural composition of how multiple agents are coordinated, parallelized, and synthesized -- now dominates system-level performance over individual model capability. We present AdaptOrch, a formal framework for task-adaptive multi-agent orchestration that dynamically selects among four canonical topologies (parallel, sequential, hierarchical, and hybrid) based on task dependency graphs and empirically derived domain characteristics. Our framework introduces three key contributions: (1) a Performance Convergence Scaling Law, formalizing conditions under which orchestration selection outweighs model selection; (2) a Topology Routing Algorithm that maps task decomposition DAGs to optimal orchestration patterns in O(|V| + |E|) time; and (3) an Adaptive Synthesis Protocol with provable termination guarantees and heuristic consistency scoring for parallel agent outputs. We validate AdaptOrch across coding (SWE-bench), reasoning (GPQA), and retrieval-augmented generation tasks, demonstrating that topology-aware orchestration achieves 12-23% improvement over static single-topology baselines, even when using identical underlying models. Our results establish orchestration design as a first-class optimization target independent of model scaling.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-protocols|Agent protocols]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[swe-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16873v1)
