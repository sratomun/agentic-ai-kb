---
type: source
source_type: arxiv
title: "DataFactory: Collaborative Multi-Agent Framework for Advanced Table Question Answering"
authors: Tong Wang, Chi Jin, Yongkang Chen, Huan Deng et al.
url: https://arxiv.org/abs/2603.09152v1
date: 2026-03-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [knowledge-graph, agent-reliability, multi-agent-systems, arxiv, auto-ingested]
---

# DataFactory: Collaborative Multi-Agent Framework for Advanced Table Question Answering

**arXiv:** [2603.09152v1](https://arxiv.org/abs/2603.09152v1) · 2026-03-10 · cs.AI
**Authors:** Tong Wang, Chi Jin, Yongkang Chen, Huan Deng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Table Question Answering (TableQA) enables natural language interaction with structured tabular data. However, existing large language model (LLM) approaches face critical limitations: context length constraints that restrict data handling capabilities, hallucination issues that compromise answer reliability, and single-agent architectures that struggle with complex reasoning scenarios involving semantic relationships and multi-hop logic. This paper introduces DataFactory, a multi-agent framework that addresses these limitations through specialized team coordination and automated knowledge transformation. The framework comprises a Data Leader employing the ReAct paradigm for reasoning orchestration, together with dedicated Database and Knowledge Graph teams, enabling the systematic decomposition of complex queries into structured and relational reasoning tasks. We formalize automated data-to-knowledge graph transformation via the mapping function T:D x S x R -> G, and implement natural language-based consultation that - unlike fixed workflow multi-agent systems - enables flexible inter-agent deliberation and adaptive planning to improve coordination robustness. We also apply context engineering strategies that integrate historical patterns and domain knowledge to reduce hallucinations and improve query accuracy. Across TabFact, WikiTableQuestions, and FeTaQA, using eight LLMs from five providers, results show consistent gains. Our approach improves accuracy by 20.2% (TabFact) and 23.9% (WikiTQ) over baselines, with significant effects (Cohen's d > 1). Team coordination also outperforms single-team variants (+5.5% TabFact, +14.4% WikiTQ, +17.1% FeTaQA ROUGE-2). The framework offers design guidelines for multi-agent collaboration and a practical platform for enterprise data analysis through integrated structured querying and graph-based knowledge representation.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.09152v1)
