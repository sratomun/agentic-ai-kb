---
type: source
source_type: arxiv
title: "AutoSearch: Adaptive Search Depth for Efficient Agentic RAG via Reinforcement Learning"
authors: Jingbo Sun, Wenyue Chong, Songjun Tu, Qichao Zhang et al.
url: https://arxiv.org/abs/2604.17337v1
date: 2026-04-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# AutoSearch: Adaptive Search Depth for Efficient Agentic RAG via Reinforcement Learning

**arXiv:** [2604.17337v1](https://arxiv.org/abs/2604.17337v1) · 2026-04-19 · cs.AI
**Authors:** Jingbo Sun, Wenyue Chong, Songjun Tu, Qichao Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic retrieval-augmented generation (RAG) systems enable large language models (LLMs) to solve complex tasks through multi-step interaction with external retrieval tools. However, such multi-step interaction often involves redundant search steps, incurring substantial computational cost and latency. Prior work limits search depth (i.e., the number of search steps) to reduce cost, but this often leads to underexploration of complex questions. To address this, we first investigate how search depth affects accuracy and find a minimal sufficient search depth that defines an accuracy-efficiency trade-off, jointly determined by question complexity and the agent's capability. Furthermore, we propose AutoSearch, a reinforcement learning (RL) framework that evaluates each search step via self-generated intermediate answers. By a self-answering mechanism, AutoSearch identifies the minimal sufficient search depth and promotes efficient search by rewarding its attainment while penalizing over-searching. In addition, reward mechanisms are introduced to stabilize search behavior and improve answer quality on complex questions. Extensive experiments on multiple benchmarks show that AutoSearch achieves a superior accuracy-efficiency trade-off, alleviating over-searching while preserving search quality.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17337v1)
