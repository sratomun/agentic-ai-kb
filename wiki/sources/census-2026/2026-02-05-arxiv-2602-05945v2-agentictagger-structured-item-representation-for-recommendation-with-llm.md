---
type: source
source_type: arxiv
title: "AgenticTagger: Structured Item Representation for Recommendation with LLM Agents"
authors: Zhouhang Xie, Bo Peng, Zhankui He, Ziqi Chen et al.
url: https://arxiv.org/abs/2602.05945v2
date: 2026-02-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.IR
tags: [recommendation-agents, multi-agent-systems, arxiv, auto-ingested]
---

# AgenticTagger: Structured Item Representation for Recommendation with LLM Agents

**arXiv:** [2602.05945v2](https://arxiv.org/abs/2602.05945v2) · 2026-02-05 · cs.IR
**Authors:** Zhouhang Xie, Bo Peng, Zhankui He, Ziqi Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
High-quality representations are a core requirement for effective recommendation. In this work, we study the problem of LLM-based descriptor generation, i.e., keyphrase-like natural language item representation generation frameworks with minimal constraints on downstream applications. We propose AgenticTagger, a framework that queries LLMs for representing items with sequences of text descriptors. However, open-ended generation provides little control over the generation space, leading to high cardinality, low-performance descriptors that render downstream modeling challenging. To this end, AgenticTagger features two core stages: (1) a vocabulary-building stage in which a set of hierarchical, low-cardinality, and high-quality descriptors is identified, and (2) a vocabulary-assignment stage in which LLMs assign in-vocabulary descriptors to items. To effectively and efficiently ground vocabulary in the item corpus of interest, we design a multi-agent reflection mechanism in which an architect LLM iteratively refines the vocabulary guided by parallelized feedback from annotator LLMs that validate the vocabulary against item data. Experiments on public and private data show AgenticTagger brings consistent improvements across diverse recommendation scenarios, including generative and term-based retrieval, ranking, and controllability-oriented, critique-based recommendation.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.05945v2)
