---
type: source
source_type: arxiv
title: "HyEvo: Self-Evolving Hybrid Agentic Workflows for Efficient Reasoning"
authors: Beibei Xu, Yutong Ye, Chuyun Shen, Yingbo Zhou et al.
url: https://arxiv.org/abs/2603.19639v1
date: 2026-03-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [self-evolving-agents, agent-evaluation, arxiv, auto-ingested]
---

# HyEvo: Self-Evolving Hybrid Agentic Workflows for Efficient Reasoning

**arXiv:** [2603.19639v1](https://arxiv.org/abs/2603.19639v1) · 2026-03-20 · cs.AI
**Authors:** Beibei Xu, Yutong Ye, Chuyun Shen, Yingbo Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Although agentic workflows have demonstrated strong potential for solving complex tasks, existing automated generation methods remain inefficient and underperform, as they rely on predefined operator libraries and homogeneous LLM-only workflows in which all task-level computation is performed through probabilistic inference. To address these limitations, we propose HyEvo, an automated workflow-generation framework that leverages heterogeneous atomic synthesis. HyEvo integrates probabilistic LLM nodes for semantic reasoning with deterministic code nodes for rule-based execution, offloading predictable operations from LLM inference and reducing inference cost and execution latency. To efficiently navigate the hybrid search space, HyEvo employs an LLM-driven multi-island evolutionary strategy with a reflect-then-generate mechanism, iteratively refining both workflow topology and node logic via execution feedback. Comprehensive experiments show that HyEvo consistently outperforms existing methods across diverse reasoning and coding benchmarks, while reducing inference cost and execution latency by up to 19$\times$ and 16$\times$, respectively, compared to the state-of-the-art open-source baseline.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.19639v1)
