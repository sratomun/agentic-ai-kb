---
type: source
source_type: arxiv
depth: abstract
title: "Multi-Agent GraphRAG: A Text-to-Cypher Framework for Labeled Property Graphs"
authors: Anton Gusarov et al.
url: https://arxiv.org/abs/2511.08274
date: 2025-11-11
venue: arXiv 2025
tags: [text-to-cypher, knowledge-graph, agentic-rag, arxiv, text-to-cypher-corpus]
---

# Multi-Agent GraphRAG: A Text-to-Cypher Framework for Labeled Property Graphs

**arXiv:** [2511.08274](https://arxiv.org/abs/2511.08274) · 2025-11-11 · arXiv 2025
**Authors:** Anton Gusarov et al.

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
While Retrieval-Augmented Generation (RAG) methods commonly draw information from unstructured documents, the emerging paradigm of GraphRAG aims to leverage structured data such as knowledge graphs. Most existing GraphRAG efforts focus on Resource Description Framework (RDF) knowledge graphs, relying on triple representations and SPARQL queries. However, the potential of Cypher and Labeled Property Graph (LPG) databases to serve as scalable and effective reasoning engines within GraphRAG pipelines remains underexplored in current research literature. To fill this gap, we propose Multi-Agent GraphRAG, a modular LLM agentic system for text-to-Cypher query generation serving as a natural language interface to LPG-based graph data. Our proof-of-concept system features an LLM-based workflow for automated Cypher queries generation and execution, using Memgraph as the graph database backend. Iterative content-aware correction and normalization, reinforced by an aggregated feedback loop, ensures both semantic and syntactic refinement of generated queries. We evaluate our system on the CypherBench graph dataset covering several general domains with diverse types of queries. In addition, we demonstrate performance of the proposed workflow on a property graph derived from the IFC (Industry Foundation Classes) data, representing a digital twin of a building. This highlights how such an approach can bridge AI with real-world applications at scale, enabling industrial digital automation use cases.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[knowledge-graph|Knowledge graph]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[cypher]] · [[cypherbench]]
