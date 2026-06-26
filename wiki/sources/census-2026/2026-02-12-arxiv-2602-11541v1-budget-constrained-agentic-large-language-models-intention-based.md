---
type: source
source_type: arxiv
title: "Budget-Constrained Agentic Large Language Models: Intention-Based Planning for Costly Tool Use"
authors: Hanbing Liu, Chunhao Tian, Nan An, Ziyuan Wang et al.
url: https://arxiv.org/abs/2602.11541v1
date: 2026-02-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, arxiv, auto-ingested]
---

# Budget-Constrained Agentic Large Language Models: Intention-Based Planning for Costly Tool Use

**arXiv:** [2602.11541v1](https://arxiv.org/abs/2602.11541v1) · 2026-02-12 · cs.AI
**Authors:** Hanbing Liu, Chunhao Tian, Nan An, Ziyuan Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We study budget-constrained tool-augmented agents, where a large language model must solve multi-step tasks by invoking external tools under a strict monetary budget. We formalize this setting as sequential decision making in context space with priced and stochastic tool executions, making direct planning intractable due to massive state-action spaces, high variance of outcomes and prohibitive exploration cost. To address these challenges, we propose INTENT, an inference-time planning framework that leverages an intention-aware hierarchical world model to anticipate future tool usage, risk-calibrated cost, and guide decisions online. Across cost-augmented StableToolBench, INTENT strictly enforces hard budget feasibility while substantially improving task success over baselines, and remains robust under dynamic market shifts such as tool price changes and varying budgets.

## Graph
- **Concepts:** [[tool-use|Tool use]]
- **Entities:** [[toolbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.11541v1)
