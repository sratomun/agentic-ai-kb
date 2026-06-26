---
type: source
source_type: arxiv
title: "Towards Reliable ML Feature Engineering via Planning in Constrained-Topology of LLM Agents"
authors: Himanshu Thakur, Anusha Kamath, Anurag Muthyala, Dhwani Sanmukhani et al.
url: https://arxiv.org/abs/2601.10820v1
date: 2026-01-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.LG
tags: [recommendation-agents, coding-agents, human-agent-interaction, agent-reliability, multi-agent-systems, arxiv, auto-ingested]
---

# Towards Reliable ML Feature Engineering via Planning in Constrained-Topology of LLM Agents

**arXiv:** [2601.10820v1](https://arxiv.org/abs/2601.10820v1) · 2026-01-15 · cs.LG
**Authors:** Himanshu Thakur, Anusha Kamath, Anurag Muthyala, Dhwani Sanmukhani et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in code generation models have unlocked unprecedented opportunities for automating feature engineering, yet their adoption in real-world ML teams remains constrained by critical challenges: (i) the scarcity of datasets capturing the iterative and complex coding processes of production-level feature engineering, (ii) limited integration and personalization of widely used coding agents, such as CoPilot and Devin, with a team's unique tools, codebases, workflows, and practices, and (iii) suboptimal human-AI collaboration due to poorly timed or insufficient feedback. We address these challenges with a planner-guided, constrained-topology multi-agent framework that generates code for repositories in a multi-step fashion. The LLM-powered planner leverages a team's environment, represented as a graph, to orchestrate calls to available agents, generate context-aware prompts, and use downstream failures to retroactively correct upstream artifacts. It can request human intervention at critical steps, ensuring generated code is reliable, maintainable, and aligned with team expectations. On a novel in-house dataset, our approach achieves 38% and 150% improvement in the evaluation metric over manually crafted and unplanned workflows respectively. In practice, when building features for recommendation models serving over 120 million users, our approach has delivered real-world impact by reducing feature engineering cycles from three weeks to a single day.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[coding-agents|Coding agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[devin]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.10820v1)
