---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "CLAG: Adaptive Memory Organization via Agent-Driven Clustering for Small Language Model Agents"
authors: Taeyun Roh et al.
url: https://arxiv.org/abs/2603.15421v2
date: 2026-03-16
score: 7
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, agent-memory, reasoning-models, agentic-rag, coding-agents]
---

# CLAG: Adaptive Memory Organization via Agent-Driven Clustering for Small Language Model Agents

**arXiv:** [2603.15421v2](https://arxiv.org/abs/2603.15421v2) · 2026-03-16 · cs.CL
**Authors:** Taeyun Roh et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model agents heavily rely on external memory to support knowledge reuse and complex reasoning tasks. Yet most memory systems store experiences in a single global retrieval pool which can gradually dilute or corrupt stored knowledge. This problem is especially pronounced for small language models (SLMs), which are highly vulnerable to irrelevant context. We introduce CLAG, a CLustering-based AGentic memory framework where an SLM agent actively organizes memory by clustering. CLAG employs an SLM-driven router to assign incoming memories to semantically coherent clusters and autonomously generates cluster-specific profiles, including topic summaries and descriptive tags, to establish each cluster as a self-contained functional unit. By performing localized evolution within these structured neighborhoods, CLAG effectively reduces cross-topic interference and enhances internal memory density. During retrieval, the framework utilizes a two-stage process that first filters relevant clusters via their profiles, thereby excluding distractors and reducing the search space. Experiments on multiple QA datasets with three SLM backbones show that CLAG consistently improves answer quality and robustness over prior memory systems for agents, remaining lightweight and efficient.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[reasoning-models]] · [[agentic-rag]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.15421v2)
