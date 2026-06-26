---
type: source
source_type: arxiv
title: "ToolTree: Efficient LLM Agent Tool Planning via Dual-Feedback Monte Carlo Tree Search and Bidirectional Pruning"
authors: Shuo Yang, Soyeon Caren Han, Yihao Ding, Shuhe Wang et al.
url: https://arxiv.org/abs/2603.12740v1
date: 2026-03-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# ToolTree: Efficient LLM Agent Tool Planning via Dual-Feedback Monte Carlo Tree Search and Bidirectional Pruning

**arXiv:** [2603.12740v1](https://arxiv.org/abs/2603.12740v1) · 2026-03-13 · cs.AI
**Authors:** Shuo Yang, Soyeon Caren Han, Yihao Ding, Shuhe Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) agents are increasingly applied to complex, multi-step tasks that require interaction with diverse external tools across various domains. However, current LLM agent tool planning methods typically rely on greedy, reactive tool selection strategies that lack foresight and fail to account for inter-tool dependencies. In this paper, we present ToolTree, a novel Monte Carlo tree search-inspired planning paradigm for tool planning. ToolTree explores possible tool usage trajectories using a dual-stage LLM evaluation and bidirectional pruning mechanism that enables the agent to make informed, adaptive decisions over extended tool-use sequences while pruning less promising branches before and after the tool execution. Empirical evaluations across both open-set and closed-set tool planning tasks on 4 benchmarks demonstrate that ToolTree consistently improves performance while keeping the highest efficiency, achieving an average gain of around 10\% compared to the state-of-the-art planning paradigm.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.12740v1)
