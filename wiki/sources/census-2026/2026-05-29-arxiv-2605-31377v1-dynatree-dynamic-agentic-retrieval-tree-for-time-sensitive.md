---
type: source
source_type: arxiv
title: "DynaTree: Dynamic Agentic Retrieval Tree for Time-Sensitive News Retrieval"
authors: Siyuan Qi, Xinyuan Wang, Yingxuan Yang, Haochuan Guo et al.
url: https://arxiv.org/abs/2605.31377v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.IR
tags: [agentic-rag, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# DynaTree: Dynamic Agentic Retrieval Tree for Time-Sensitive News Retrieval

**arXiv:** [2605.31377v1](https://arxiv.org/abs/2605.31377v1) · 2026-05-29 · cs.IR
**Authors:** Siyuan Qi, Xinyuan Wang, Yingxuan Yang, Haochuan Guo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Retrieval-Augmented Generation improves retrieval by integrating planning, tool use, and iterative reasoning, but existing agentic RAG methods often couple semantic expansion with retrieval decisions in short-horizon inference loops, leading to high inference cost and limited suitability for time-sensitive news retrieval. We propose DynaTree, a two-stage framework for efficient and adaptive news retrieval. In the offline stage, DynaTree uses coordinated agents to construct a reusable retrieval tree that materializes the semantic space of a query topic. In the online stage, DynaTree performs lightweight daily subtree selection over a time-localized evaluation proxy, without further agentic reasoning, tree modification, or retraining. Experiments on a multi-day Syft news benchmark and multiple BEIR datasets show that DynaTree achieves strong recall and ranking performance, consistently outperforming standard RAG and prior agentic baselines. We further deploy DynaTree in the Syft production system and evaluate it through online A/B testing from Jan. 28 to Feb. 6, 2026. The dynamically adapted variant improves survival rate from 0.32-0.53 to 0.59-0.73 over a fixed offline-selected subtree and outperforms existing production recallers on every evaluation day. These results show that persistent, structure-aware semantic expansion can translate offline agentic reasoning into practical improvements in coverage, freshness, and relevance for real-world news retrieval.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.31377v1)
