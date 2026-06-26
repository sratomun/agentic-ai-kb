---
type: source
source_type: arxiv
title: "Lang2MLIP: End-to-End Language-to-Machine Learning Interatomic Potential Development with Autonomous Agentic Workflows"
authors: Wenwen Li, Yuki Orimo, Nontawat Charoenphakdee
url: https://arxiv.org/abs/2605.14527v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.LG
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# Lang2MLIP: End-to-End Language-to-Machine Learning Interatomic Potential Development with Autonomous Agentic Workflows

**arXiv:** [2605.14527v1](https://arxiv.org/abs/2605.14527v1) · 2026-05-14 · cs.LG
**Authors:** Wenwen Li, Yuki Orimo, Nontawat Charoenphakdee

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Developing machine learning interatomic potentials (MLIPs) for complex materials systems remains challenging because it requires expertise in atomistic simulations, machine learning, and workflow design, as well as iterative active learning procedures. Existing automated pipelines typically assume a fixed sequence of stages or depend on domain experts, which limits their adaptability to heterogeneous materials systems where the optimal curriculum is not known in advance. To lower the barrier to developing MLIPs for non-experts, we propose Lang2MLIP, a multi-agent framework that takes natural-language input and formulates end-to-end MLIP development as a sequential decision-making problem solved by large language models (LLMs). At each step, a decision-making agent observes the current dataset, model, evaluation results, and execution log, and then automatically selects an appropriate action to improve the model. This removes the need for a predefined pipeline and enables the agent to self-correct by revisiting earlier subsystems when new failures arise. We evaluate this approach on a solid electrolyte interphase (SEI) system with multiple components and interfaces. These results suggest that LLM-based multi-agent systems are a promising direction for automating MLIP development and making it more accessible to non-experts.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14527v1)
