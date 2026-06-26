---
type: source
source_type: arxiv
title: "Beyond RAG for Cyber Threat Intelligence: A Systematic Evaluation of Graph-Based and Agentic Retrieval"
authors: Dzenan Hamzic, Florian Skopik, Max Landauer, Markus Wurzenberger et al.
url: https://arxiv.org/abs/2604.11419v1
date: 2026-04-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [knowledge-graph, agent-reliability, agent-security, agentic-rag, arxiv, auto-ingested]
---

# Beyond RAG for Cyber Threat Intelligence: A Systematic Evaluation of Graph-Based and Agentic Retrieval

**arXiv:** [2604.11419v1](https://arxiv.org/abs/2604.11419v1) · 2026-04-13 · cs.AI
**Authors:** Dzenan Hamzic, Florian Skopik, Max Landauer, Markus Wurzenberger et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cyber threat intelligence (CTI) analysts must answer complex questions over large collections of narrative security reports. Retrieval-augmented generation (RAG) systems help language models access external knowledge, but traditional vector retrieval often struggles with queries that require reasoning over relationships between entities such as threat actors, malware, and vulnerabilities. This limitation arises because relevant evidence is often distributed across multiple text fragments and documents. Knowledge graphs address this challenge by enabling structured multi-hop reasoning through explicit representations of entities and relationships. However, multiple retrieval paradigms, including graph-based, agentic, and hybrid approaches, have emerged with different assumptions and failure modes. It remains unclear how these approaches compare in realistic CTI settings and when graph grounding improves performance. We present a systematic evaluation of four RAG architectures for CTI analysis: standard vector retrieval, graph-based retrieval over a CTI knowledge graph, an agentic variant that repairs failed graph queries, and a hybrid approach combining graph queries with text retrieval. We evaluate these systems on 3,300 CTI question-answer pairs spanning factual lookups, multi-hop relational queries, analyst-style synthesis questions, and unanswerable cases. Results show that graph grounding improves performance on structured factual queries. The hybrid graph-text approach improves answer quality by up to 35 percent on multi-hop questions compared to vector RAG, while maintaining more reliable performance than graph-only systems.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.11419v1)
