---
type: source
source_type: arxiv
title: "GraphRAG for Engineering Diagrams: ChatP&ID Enables LLM Interaction with P&IDs"
authors: Achmad Anggawirya Alimin, Artur M. Schweidtmann
url: https://arxiv.org/abs/2603.22528v1
date: 2026-03-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.IR
tags: [knowledge-graph, agent-reliability, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# GraphRAG for Engineering Diagrams: ChatP&ID Enables LLM Interaction with P&IDs

**arXiv:** [2603.22528v1](https://arxiv.org/abs/2603.22528v1) · 2026-03-23 · cs.IR
**Authors:** Achmad Anggawirya Alimin, Artur M. Schweidtmann

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) combined with Retrieval-Augmented Generation (RAG) and knowledge graphs offer new opportunities for interacting with engineering diagrams such as Piping and Instrumentation Diagrams (P&IDs). However, directly processing raw images or smart P&ID files with LLMs is often costly, inefficient, and prone to hallucinations. This work introduces ChatP&ID, an agentic framework that enables grounded and cost-effective natural-language interaction with P&IDs using Graph Retrieval-Augmented Generation (GraphRAG), a paradigm we refer to as GraphRAG for engineering diagrams. Smart P&IDs encoded in the DEXPI standard are transformed into structured knowledge graphs, which serve as the basis for graph-based retrieval and reasoning by LLM agents. This approach enables reliable querying of engineering diagrams while significantly reducing computational cost. Benchmarking across commercial LLM APIs (OpenAI, Anthropic) demonstrates that graph-based representations improve accuracy by 18% over raw image inputs and reduce token costs by 85% compared to directly ingesting smart P&ID files. While small open-source models still struggle to interpret knowledge graph formats and structured engineering data, integrating them with VectorRAG and PathRAG improves response accuracy by up to 40%. Notably, GPT-5-mini combined with ContextRAG achieves 91% accuracy at a cost of only $0.004 per task. The resulting ChatP&ID interface enables intuitive natural-language interaction with complex engineering diagrams and lays the groundwork for AI-assisted process engineering tasks such as Hazard and Operability Studies (HAZOP) and multi-agent analysis.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]] · [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.22528v1)
