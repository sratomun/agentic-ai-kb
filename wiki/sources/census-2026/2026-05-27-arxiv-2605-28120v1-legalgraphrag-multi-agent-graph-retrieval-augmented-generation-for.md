---
type: source
source_type: arxiv
title: "LegalGraphRAG: Multi-Agent Graph Retrieval-Augmented Generation for Reliable Legal Reasoning"
authors: Zerui Chen, Qinggang Zhang, Zhishang Xiang, Zhimin Wei et al.
url: https://arxiv.org/abs/2605.28120v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [knowledge-graph, agent-reliability, agentic-rag, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# LegalGraphRAG: Multi-Agent Graph Retrieval-Augmented Generation for Reliable Legal Reasoning

**arXiv:** [2605.28120v1](https://arxiv.org/abs/2605.28120v1) · 2026-05-27 · cs.CL
**Authors:** Zerui Chen, Qinggang Zhang, Zhishang Xiang, Zhimin Wei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph-based Retrieval-Augmented Generation (GraphRAG) advances flat document retrieval by structuring knowledge as relational graphs, enabling more coherent and effective reasoning. However, applying it to specific domains like legal reasoning faces critical challenges. (i) Legal corpora are heterogeneous, containing multi-granular knowledge from cases, articles and interpretations. A flat knowledge graph cannot adequately differentiate between factual details, applied rules, and abstract principles, limiting accurate retrieval. (ii) Reliable legal judgment demands transparent, evidence-based reasoning. Traditional RAG passes retrieved context directly to an LLM without verification, resulting in opaque, error-prone reasoning. To this end, we propose LegalGraphRAG, a framework designed for reliable legal reasoning. Our approach introduces two core components: a hierarchical legal graph that hierarchically organizes legal sources to enable retrieval at appropriate abstraction levels, and a multi-agent system for reliable legal reasoning, where a Researcher retrieves candidate evidence, an Auditor rigorously verifies its validity against source documents, and an Adjudicator synthesizes the set of verified evidence to render a final judgment. Extensive experiments show that LegalGraphRAG achieves the state-of-the-art performance, outperforming existing GraphRAG baselines in accurate and trustworthy legal analysis. Our code, datasets and implementation details are available at https://github.com/XMUDeepLIT/LegalGraphRAG.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28120v1)
