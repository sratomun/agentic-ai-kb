---
type: source
source_type: arxiv
title: "Knowledge-Graph Paths as Intermediate Supervision for Self-Evolving Search Agents"
authors: Huyu Wu, Jun Liu, Xiaochi Wei, Yan Gao et al.
url: https://arxiv.org/abs/2605.05702v1
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, self-evolving-agents, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Knowledge-Graph Paths as Intermediate Supervision for Self-Evolving Search Agents

**arXiv:** [2605.05702v1](https://arxiv.org/abs/2605.05702v1) · 2026-05-07 · cs.AI
**Authors:** Huyu Wu, Jun Liu, Xiaochi Wei, Yan Gao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Self-evolving search agents reduce reliance on human-written training questions by generating and solving their own search tasks. We build on Search Self-Play (SSP), a representative Proposer and Solver framework in which questions are generated and answered via multi-step search and reasoning. In practice, however, SSP faces two bottlenecks: the Proposer constructs questions from isolated answer entities without relational context, yielding many invalid or unverifiable questions in early self-play training, while the Solver receives only a binary outcome reward that discards useful signal from partially on-track search trajectories. We address both bottlenecks by reusing knowledge-graph paths as construction-derived intermediate supervision for both question construction and reward shaping. First, we ground question construction in LLM-guided knowledge-graph subgraphs, providing relational context for the Proposer. Second, we observe that constructing and solving a multi-hop question can involve overlapping intermediate entities: the factual bridges used to formulate the question may provide approximate waypoints for answering it. Exploiting this overlap, we introduce Waypoint Coverage Reward (WCR), which grants graded partial credit to incorrect Solver trajectories according to their coverage of entities on the construction path, while preserving full reward for correct answers. Across seven QA benchmarks and nine model configurations, our approach improves the average score over standard SSP in all configurations, including notable gains on multi-hop QA tasks. These results suggest that knowledge-graph paths can be reused as lightweight intermediate supervision, providing both relational guidance and process feedback without additional task-specific human annotations or manually labeled process steps.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.05702v1)
