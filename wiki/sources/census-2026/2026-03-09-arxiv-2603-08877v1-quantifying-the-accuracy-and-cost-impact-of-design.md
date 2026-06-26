---
type: source
source_type: arxiv
title: "Quantifying the Accuracy and Cost Impact of Design Decisions in Budget-Constrained Agentic LLM Search"
authors: Kyle McCleary, James Ghawaly
url: https://arxiv.org/abs/2603.08877v1
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rag, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Quantifying the Accuracy and Cost Impact of Design Decisions in Budget-Constrained Agentic LLM Search

**arXiv:** [2603.08877v1](https://arxiv.org/abs/2603.08877v1) · 2026-03-09 · cs.AI
**Authors:** Kyle McCleary, James Ghawaly

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Retrieval-Augmented Generation (RAG) systems combine iterative search, planning prompts, and retrieval backends, but deployed settings impose explicit budgets on tool calls and completion tokens. We present a controlled measurement study of how search depth, retrieval strategy, and completion budget affect accuracy and cost under fixed constraints. Using Budget-Constrained Agentic Search (BCAS), a model-agnostic evaluation harness that surfaces remaining budget and gates tool use, we run comparisons across six LLMs and three question-answering benchmarks. Across models and datasets, accuracy improves with additional searches up to a small cap, hybrid lexical and dense retrieval with lightweight re-ranking produces the largest average gains in our ablation grid, and larger completion budgets are most helpful on HotpotQA-style synthesis. These results provide practical guidance for configuring budgeted agentic retrieval pipelines and are accompanied by reproducible prompts and evaluation settings.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08877v1)
