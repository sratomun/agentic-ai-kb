---
type: source
source_type: arxiv
title: "An Agentic Approach to Metadata Reasoning"
authors: Jiani Zhang, Sercan O. Arik, Cosmin Arad, Fatma Ozcan et al.
url: https://arxiv.org/abs/2604.20144v1
date: 2026-04-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.DB
tags: [agent-evaluation, arxiv, auto-ingested]
---

# An Agentic Approach to Metadata Reasoning

**arXiv:** [2604.20144v1](https://arxiv.org/abs/2604.20144v1) · 2026-04-22 · cs.DB
**Authors:** Jiani Zhang, Sercan O. Arik, Cosmin Arad, Fatma Ozcan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As LLM-driven autonomous agents evolve to perform complex, multi-step tasks that require integrating multiple datasets, the problem of discovering relevant data sources becomes a key bottleneck. Beyond the challenge posed by the sheer volume of available data sources, data-source selection is difficult because the semantics of data are extremely nuanced and require considering many aspects of the data. To address this, we introduce the Metadata Reasoner, an agentic approach to metadata reasoning, designed to identify a small set of data sources that are both sufficient and minimal for a given analytical task. The Metadata Reasoner leverages a table-search engine to retrieve candidate tables, and then autonomously consults various aspects of the available metadata to determine whether the candidates fit the requirements of the task. We demonstrate the effectiveness of the Metadata Reasoner through a series of empirical studies. Evaluated on the real-world KramaBench datasets for data selection, our approach achieves an average F1-score of 83.16%, outperforming state-of-the-art baselines by a substantial margin of 32 percentage points. Furthermore, evaluations on a newly-created synthetic benchmark based on the BIRD data lake reveal that the Metadata Reasoner is highly robust against redundant and low-quality tables that may be in the data lake. In this noisy environment, it maintains an average of 85.5% F1-score for selecting the right datasets and demonstrates a 99% success rate in avoiding low-quality data.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.20144v1)
