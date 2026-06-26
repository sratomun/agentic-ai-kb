---
type: source
source_type: arxiv
title: "H-Mem: A Novel Memory Mechanism for Evolving and Retrieving Agent Memory via a Hybrid Structure"
authors: Jiawei Yu, Yixiang Fang, Xilin Liu, Yuchi Ma
url: https://arxiv.org/abs/2605.15701v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.CL
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# H-Mem: A Novel Memory Mechanism for Evolving and Retrieving Agent Memory via a Hybrid Structure

**arXiv:** [2605.15701v1](https://arxiv.org/abs/2605.15701v1) · 2026-05-15 · cs.CL
**Authors:** Jiawei Yu, Yixiang Fang, Xilin Liu, Yuchi Ma

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Memory data are ubiquitous in Large Language Model (LLM)-based agents (e.g., OpenClaw and Manus). A few recent works have attempted to exploit agents'memory for improving their performance on the question-answering (QA) task, but they lack a principled mechanism for effectively modeling how memory data evolves over time and retrieving memory data effectively, leading to poor performance in memory utilization. To fill this gap, we present H-Mem, a novel memory mechanism via a hybrid structure that can not only effectively model the evolution of agent memory over a long period of time, but also provide an efficient memory retrieval approach. Particularly, H-Mem builds a temporal and semantic tree structure that allows the short-term memory data to evolve progressively into long-term memory data, where the latter provides summarized information about the former, while simultaneously constructing a knowledge graph to capture the relationships between entities in memory. Moreover, it offers an effective memory retrieval approach by exploiting the hybrid structure of the tree and graph structures. Extensive experiments on three agent memory benchmarks show that H-Mem achieves state-of-the-art performance on the QA task.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15701v1)
