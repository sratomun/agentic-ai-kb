---
type: source
source_type: arxiv
depth: abstract
title: "Federation of Agents: A Semantics-Aware Communication Fabric for Large-Scale Agentic AI"
authors: Lorenzo Giusti et al.
url: https://arxiv.org/abs/2509.20175
date: 2025-09-24
venue: arXiv 2025
tags: [mediated-semantic-architecture, multi-agent-systems, intent-routing, arxiv, mediated-architecture-corpus]
---

# Federation of Agents: A Semantics-Aware Communication Fabric for Large-Scale Agentic AI

**arXiv:** [2509.20175](https://arxiv.org/abs/2509.20175) · 2025-09-24 · arXiv 2025
**Authors:** Lorenzo Giusti et al.

> Abstract-tier note (extended-search corpus). Part of the mediated-semantic-architecture thread (2026-06-23).

## Abstract
We present Federation of Agents (FoA), a distributed orchestration framework that transforms static multi-agent coordination into dynamic, capability-driven collaboration. FoA introduces Versioned Capability Vectors (VCVs): machine-readable profiles that make agent capabilities searchable through semantic embeddings, enabling agents to advertise their capabilities, cost, and limitations. Our architecture combines three key innovations: (1) semantic routing that matches tasks to agents over sharded HNSW indices while enforcing operational constraints through cost-biased optimization, (2) dynamic task decomposition where compatible agents collaboratively break down complex tasks into DAGs of subtasks through consensus-based merging, and (3) smart clustering that groups agents working on similar subtasks into collaborative channels for k-round refinement before synthesis. Built on top of MQTT's publish-subscribe semantics for scalable message passing, FoA achieves sub-linear complexity through hierarchical capability matching and efficient index maintenance. Evaluation on HealthBench shows 13x improvements over single-model baselines, with clustering-enhanced collaboration particularly effective for complex reasoning tasks requiring multiple perspectives. The system scales horizontally while maintaining consistent performance, demonstrating that semantic orchestration with structured collaboration can unlock the collective intelligence of heterogeneous federations of AI agents.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[multi-agent-systems|Multi-agent systems]] · [[intent-routing|Intent routing]]
