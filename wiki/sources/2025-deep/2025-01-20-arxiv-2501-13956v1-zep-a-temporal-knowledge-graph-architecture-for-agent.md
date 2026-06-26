---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Zep: A Temporal Knowledge Graph Architecture for Agent Memory"
authors: Preston Rasmussen, Pavlo Paliychuk, Travis Beauvais, Jack Ryan et al.
url: https://arxiv.org/abs/2501.13956v1
date: 2025-01-20
citationCount: 213
influentialCitationCount: 33
velocity: 12.52
ingested: 2026-06-22
tags: [knowledge-graph, agentic-rag, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Zep: A Temporal Knowledge Graph Architecture for Agent Memory

**arXiv [2501.13956v1](https://arxiv.org/abs/2501.13956v1)** · 2025-01-20 · **213 citations** (33 influential · 12.52/mo) · Preston Rasmussen, Pavlo Paliychuk, Travis Beauvais, Jack Ryan et al.

## Abstract
We introduce Zep, a novel memory layer service for AI agents that outperforms the current state-of-the-art system, MemGPT, in the Deep Memory Retrieval (DMR) benchmark. Additionally, Zep excels in more comprehensive and challenging evaluations than DMR that better reflect real-world enterprise use cases. While existing retrieval-augmented generation (RAG) frameworks for large language model (LLM)-based agents are limited to static document retrieval, enterprise applications demand dynamic knowledge integration from diverse sources including ongoing conversations and business data. Zep addresses this fundamental limitation through its core component Graphiti -- a temporally-aware knowledge graph engine that dynamically synthesizes both unstructured conversational data and structured business data while maintaining historical relationships. In the DMR benchmark, which the MemGPT team established as their primary evaluation metric, Zep demonstrates superior performance (94.8% vs 93.4%). Beyond DMR, Zep's capabilities are further validated through the more challenging LongMemEval benchmark, which better reflects enterprise use cases through complex temporal reasoning tasks. In this evaluation, Zep achieves substantial results with accuracy improvements of up to 18.5% while simultaneously reducing response latency by 90% compared to baseline implementations. These results are particularly pronounced in enterprise-critical tasks such as cross-session information synthesis and long-term context maintenance, demonstrating Zep's effectiveness for deployment in real-world applications.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Knowledge Graph Construction 2.1 Episodes 2.2 Semantic Entities and Facts 2.2.1 Entities 2.2.2 Facts 2.2.3 Temporal Extraction and Edge Invalidation 2.3 Communities 3 Memory Retrieval 3.1 Search 3.2 Reranker 4 Experiments 4.1 Choice of models 4.2 Deep Memory Retrieval (DMR) 4.3 LongMemEval (LME) 4.3.1 LongMemEval and MemGPT 4.3.2 LongMemEval results 5 Conclusion 6 Appendix 6.1 Graph Construction Prompts 6.1.1 Entity Extraction 6.1.2 Entity Resolution 6.1.3 Fact Extraction 6.1.4 Fact Resolution 6.1.5 Temporal Extraction Zep: A Temporal Knowledge Graph Architecture for Agent Memory Preston Rasmussen Zep AI preston@getzep.com Pavlo Paliychuk Zep AI paul@getzep.com Travis Beauvais Zep AI travis@getzep.com Jack Ryan Zep AI jack@getzep.com Daniel Chalef Zep AI daniel@getzep.com Abstract We introduce Zep, a novel memory layer service for AI agents that outperforms the current state-of-the-art system, MemGPT, in the Deep Memory Retrieval (DMR) benchmark. Additionally,…

**Method / approach.** methods differ substantially from GraphRAG’s map-reduce approach [ 4 ] . To support our retrieval methodology, we generate community names containing key terms and relevant subjects from the community summaries. These names are embedded and stored to enable cosine similarity searches. 3 Memory Retrieval The memory retrieval system in Zep provides powerful, complex, and highly configurable functionality. At a high level, the Zep graph search API implements a function f : S → S : 𝑓 → 𝑆 𝑆 f:S\to S italic_f : italic_S → italic_S that accepts a text-string query α ∈ S 𝛼 𝑆 \alpha\in S italic_α ∈ italic_S as input and returns a text-string context β ∈ S 𝛽 𝑆 \beta\in S italic_β ∈ italic_S as output. The output β 𝛽 \beta italic_β contains formatted data from nodes and edges required for an LLM agent to generate an accurate response to query α 𝛼 \alpha italic_α . The process f ⁢ ( α ) → β → 𝑓 𝛼 𝛽 f(\alpha)\to\beta italic_f ( italic_α ) → italic_β comprises three distinct steps: •…

**Results.** Experiments 4.1 Choice of models 4.2 Deep Memory Retrieval (DMR) 4.3 LongMemEval (LME) 4.3.1 LongMemEval and MemGPT 4.3.2 LongMemEval results 5 Conclusion 6 Appendix 6.1 Graph Construction Prompts 6.1.1 Entity Extraction 6.1.2 Entity Resolution 6.1.3 Fact Extraction 6.1.4 Fact Resolution 6.1.5 Temporal Extraction Zep: A Temporal Knowledge Graph Architecture for Agent Memory Preston Rasmussen Zep AI preston@getzep.com Pavlo Paliychuk Zep AI paul@getzep.com Travis Beauvais Zep AI travis@getzep.com Jack Ryan Zep AI jack@getzep.com Daniel Chalef Zep AI daniel@getzep.com Abstract We introduce Zep, a novel memory layer service for AI agents that outperforms the current state-of-the-art system, MemGPT, in the Deep Memory Retrieval (DMR) benchmark. Additionally, Zep excels in more comprehensive and challenging evaluations than DMR that better reflect real-world enterpris…

**Conclusion.** Conclusion 6 Appendix 6.1 Graph Construction Prompts 6.1.1 Entity Extraction 6.1.2 Entity Resolution 6.1.3 Fact Extraction 6.1.4 Fact Resolution 6.1.5 Temporal Extraction Zep: A Temporal Knowledge Graph Architecture for Agent Memory Preston Rasmussen Zep AI preston@getzep.com Pavlo Paliychuk Zep AI paul@getzep.com Travis Beauvais Zep AI travis@getzep.com Jack Ryan Zep AI jack@getzep.com Daniel Chalef Zep AI daniel@getzep.com Abstract We introduce Zep, a novel memory layer service for AI agents that outperforms the current state-of-the-art system, MemGPT, in the Deep Memory Retrieval (DMR) benchmark. Additionally, Zep excels in more comprehensive and challenging evaluations than DMR tha…

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2501.13956v1.md` · `raw/arxiv/2501.13956v1.fulltext.md`
