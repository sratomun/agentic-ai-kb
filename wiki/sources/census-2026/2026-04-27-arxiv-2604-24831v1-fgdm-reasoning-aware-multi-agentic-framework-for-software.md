---
type: source
source_type: arxiv
title: "FGDM: Reasoning Aware Multi-Agentic Framework for Software Bug Detection using Chain of Thought and Tree of Thought Prompting"
authors: Srita Padmanabhuni, Bhargavi Karuturi, Jerusha Karen Indupalli, Santhan Reddy Chilla et al.
url: https://arxiv.org/abs/2604.24831v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.SE
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# FGDM: Reasoning Aware Multi-Agentic Framework for Software Bug Detection using Chain of Thought and Tree of Thought Prompting

**arXiv:** [2604.24831v1](https://arxiv.org/abs/2604.24831v1) · 2026-04-27 · cs.SE
**Authors:** Srita Padmanabhuni, Bhargavi Karuturi, Jerusha Karen Indupalli, Santhan Reddy Chilla et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deep Learning methods are becoming prominent in automated software bug detection; however, they lack the global understanding of the given code. Consequently, their performance tends to degrade, especially when they are applied to large interconnected code bases or complex modular programs. Recently, Large Language Models (LLMs) have proven to be effective at capturing dependencies among multiple interconnected modules in the codebase. This motivated us to propose the Flow-Graph-Driven Multi-Agent Framework (FGDM), which is composed of four agents that operate in a sequential manner. The framework converts the received code to a flow graph, identifies the erroneous segments, and further generates the repaired code. All the employed agents utilize Chain-of-Thought (COT) and Tree-of-Thoughts (TOT) prompts. Additionally, we also integrated with the FAISS vector database to retrieve similar previous bugs and their repairs. We demonstrated the efficacy of the proposed framework over 100 programs from several projects, including Ansible, Black, FastAPI, Keras, Luigi, Matplotlib, Pandas, Scrapy, SpaCy, and Tornado in both C and Python programs. Our experiments demonstrate that the FGDM outperforms the extant approaches and yielded reductions with a mean of 24.33 and 8.37 in Levenshtein distance and similarities of 0.951 and 0.974 in cosine similarity for Python and C, respectively.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.24831v1)
