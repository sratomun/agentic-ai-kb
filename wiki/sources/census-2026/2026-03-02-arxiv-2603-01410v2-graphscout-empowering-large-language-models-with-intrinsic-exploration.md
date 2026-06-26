---
type: source
source_type: arxiv
title: "GraphScout: Empowering Large Language Models with Intrinsic Exploration Ability for Agentic Graph Reasoning"
authors: Yuchen Ying, Weiqi Jiang, Tongya Zheng, Yu Wang et al.
url: https://arxiv.org/abs/2603.01410v2
date: 2026-03-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [knowledge-graph, agent-reliability, agentic-rag, arxiv, auto-ingested]
---

# GraphScout: Empowering Large Language Models with Intrinsic Exploration Ability for Agentic Graph Reasoning

**arXiv:** [2603.01410v2](https://arxiv.org/abs/2603.01410v2) · 2026-03-02 · cs.AI
**Authors:** Yuchen Ying, Weiqi Jiang, Tongya Zheng, Yu Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Knowledge graphs provide structured and reliable information for many real-world applications, motivating increasing interest in combining large language models (LLMs) with graph-based retrieval to improve factual grounding. Recent Graph-based Retrieval-Augmented Generation (GraphRAG) methods therefore introduce iterative interaction between LLMs and knowledge graphs to enhance reasoning capability. However, existing approaches typically depend on manually designed guidance and interact with knowledge graphs through a limited set of predefined tools, which substantially constrains graph exploration. To address these limitations, we propose GraphScout, a training-centric agentic graph reasoning framework equipped with more flexible graph exploration tools. GraphScout enables models to autonomously interact with knowledge graphs to synthesize structured training data which are then used to post-train LLMs, thereby internalizing agentic graph reasoning ability without laborious manual annotation or task curation. Extensive experiments across five knowledge-graph domains show that a small model (e.g., Qwen3-4B) augmented with GraphScout outperforms baseline methods built on leading LLMs (e.g., Qwen-Max) by an average of 16.7\% while requiring significantly fewer inference tokens. Moreover, GraphScout exhibits robust cross-domain transfer performance. Our code will be made publicly available~\footnote{https://github.com/Ying-Yuchen/_GraphScout_}.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]] · [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01410v2)
