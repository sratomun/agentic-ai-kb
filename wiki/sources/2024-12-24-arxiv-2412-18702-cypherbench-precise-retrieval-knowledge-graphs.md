---
type: source
source_type: arxiv
depth: abstract
title: "CypherBench: Towards Precise Retrieval over Full-scale Modern Knowledge Graphs in the LLM Era"
authors: Yanlin Feng, Simone Papicchio, Sajjadur Rahman (Megagon Labs)
url: https://arxiv.org/abs/2412.18702
date: 2024-12-24
venue: ACL 2025
tags: [text-to-cypher, knowledge-graph, agentic-rag, arxiv, text-to-cypher-corpus]
---

# CypherBench: Towards Precise Retrieval over Full-scale Modern Knowledge Graphs in the LLM Era

**arXiv:** [2412.18702](https://arxiv.org/abs/2412.18702) · 2024-12-24 · ACL 2025
**Authors:** Yanlin Feng, Simone Papicchio, Sajjadur Rahman (Megagon Labs)

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
Retrieval from graph data is crucial for augmenting large language models (LLM) with both open-domain knowledge and private enterprise data, and it is also a key component in the recent GraphRAG system (edge et al., 2024). Despite decades of research on knowledge graphs and knowledge base question answering, leading LLM frameworks (e.g. Langchain and LlamaIndex) have only minimal support for retrieval from modern encyclopedic knowledge graphs like Wikidata. In this paper, we analyze the root cause and suggest that modern RDF knowledge graphs (e.g. Wikidata, Freebase) are less efficient for LLMs due to overly large schemas that far exceed the typical LLM context window, use of resource identifiers, overlapping relation types and lack of normalization. As a solution, we propose property graph views on top of the underlying RDF graph that can be efficiently queried by LLMs using Cypher. We instantiated this idea on Wikidata and introduced CypherBench, the first benchmark with 11 large-scale, multi-domain property graphs with 7.8 million entities and over 10,000 questions.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[knowledge-graph|Knowledge graph]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[cypherbench]] · [[cypher]]
