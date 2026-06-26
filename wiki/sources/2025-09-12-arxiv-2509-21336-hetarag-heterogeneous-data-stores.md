---
type: source
source_type: arxiv
depth: abstract
title: "HetaRAG: Hybrid Deep Retrieval-Augmented Generation across Heterogeneous Data Stores"
authors: Guohang Yan et al. (Shanghai AI Lab)
url: https://arxiv.org/abs/2509.21336
date: 2025-09-12
venue: arXiv 2025
tags: [mediated-semantic-architecture, agentic-rag, knowledge-graph, arxiv, mediated-architecture-corpus]
---

# HetaRAG: Hybrid Deep Retrieval-Augmented Generation across Heterogeneous Data Stores

**arXiv:** [2509.21336](https://arxiv.org/abs/2509.21336) · 2025-09-12 · arXiv 2025
**Authors:** Guohang Yan et al. (Shanghai AI Lab)

> Abstract-tier note (extended-search corpus). Part of the mediated-semantic-architecture thread (2026-06-23).

## Abstract
Retrieval-augmented generation (RAG) has become a dominant paradigm for mitigating knowledge hallucination and staleness in large language models (LLMs) while preserving data security. By retrieving relevant evidence from private, domain-specific corpora and injecting it into carefully engineered prompts, RAG delivers trustworthy responses without the prohibitive cost of fine-tuning. Traditional retrieval-augmented generation (RAG) systems are text-only and often rely on a single storage backend, most commonly a vector database. In practice, this monolithic design suffers from unavoidable trade-offs: vector search captures semantic similarity yet loses global context; knowledge graphs excel at relational precision but struggle with recall; full-text indexes are fast and exact yet semantically blind; and relational engines such as MySQL provide strong transactional guarantees but no semantic understanding. We argue that these heterogeneous retrieval paradigms are complementary, and propose a principled fusion scheme to orchestrate them synergistically, mitigating the weaknesses of any single modality. In this work we introduce HetaRAG, a hybrid, deep-retrieval augmented generation framework that orchestrates cross-modal evidence from heterogeneous data stores. We plan to design a system that unifies vector indices, knowledge graphs, full-text engines, and structured databases into a single retrieval plane, dynamically routing and fusing evidence to maximize recall, precision, and contextual fidelity.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[agentic-rag|Agentic RAG]] · [[knowledge-graph|Knowledge graph]]
