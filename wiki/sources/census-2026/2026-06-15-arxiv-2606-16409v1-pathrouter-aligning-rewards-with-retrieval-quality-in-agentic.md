---
type: source
source_type: arxiv
title: "PathRouter: Aligning Rewards with Retrieval Quality in Agentic Graph Retrieval-Augmented Generation"
authors: Bo Wang, Heyan Huang, Yaolin Li, Wei Tang et al.
url: https://arxiv.org/abs/2606.16409v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# PathRouter: Aligning Rewards with Retrieval Quality in Agentic Graph Retrieval-Augmented Generation

**arXiv:** [2606.16409v1](https://arxiv.org/abs/2606.16409v1) · 2026-06-15 · cs.CL
**Authors:** Bo Wang, Heyan Huang, Yaolin Li, Wei Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic GraphRAG trains language-model agents to iteratively retrieve and reason over graph-structured evidence, enabling more accurate and context-aware decision-making by efficiently navigating complex information networks. However, outcome-only reinforcement learning suffers from \textit{\textbf{answer-path reward aliasing}}, where correct answers may come from shortcuts rather than useful evidence paths. It also exhibits \textit{\textbf{search-update ambiguity}}, as scalar trajectory-level feedback does not indicate which retrieval actions to adjust. To mitigate these shortcomings, we present PathRouter, a path-aware training framework for agentic GraphRAG. PathRouter jointly evaluates each trajectory along answer correctness and evidence-path overlap, yielding four trajectory categories with differentiated GRPO advantage scaling that suppresses shortcut reinforcement while preserving evidence-seeking behavior. For evidence-poor trajectories, a frozen gold-evidence teacher provides token-level KL guidance on reasoning and search-query tokens, excluding answer tokens to avoid direct response imitation. Experiments on six QA benchmarks across three model sizes show that PathRouter consistently improves answer F1 and evidence-path overlap, achieving average F1 gains of 3.1 on 3B and 4.9 on 7B models compared to a strong baseline.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.16409v1)
