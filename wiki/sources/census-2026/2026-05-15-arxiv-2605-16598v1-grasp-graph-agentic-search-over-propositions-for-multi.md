---
type: source
source_type: arxiv
title: "GRASP: Graph Agentic Search over Propositions for Multi-hop Question Answering"
authors: Stockton Jenkins, Ramya Korlakai Vinayak, Junjie Hu
url: https://arxiv.org/abs/2605.16598v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.MA
tags: [knowledge-graph, multi-agent-systems, arxiv, auto-ingested]
---

# GRASP: Graph Agentic Search over Propositions for Multi-hop Question Answering

**arXiv:** [2605.16598v1](https://arxiv.org/abs/2605.16598v1) · 2026-05-15 · cs.MA
**Authors:** Stockton Jenkins, Ramya Korlakai Vinayak, Junjie Hu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic retrieval improves multi-hop question answering by giving language models autonomy to iteratively gather evidence. Recent work augments these systems with knowledge graphs for structured traversal, but this combination introduces significant cost: expensive graph construction at index time and compounding token usage at inference time. We introduce Graph Agentic Search over Propositions (GRASP), an agentic system that simultaneously optimizes for high accuracy and minimal token usage in multi-hop question answering. Rather than executing a rigid, singular query, GRASP actively coordinates its retrieval strategy by decomposing multi-hop queries into dependency-aware plans. This enables GRASP to dynamically scale the number of sub-agents according to the complexity of the problem. Each sub-agent resolves its single-hop query by exploring a novel three-layer hierarchical graph of entities, propositions, and passages, using the entity layer for targeted traversal and the proposition layer for high-recall passage retrieval via reciprocal-rank voting. We evaluate GRASP on MuSiQue, 2WikiMultihopQA, and HotpotQA under two settings: open-corpus retrieval and extended context reasoning (LongBench). GRASP achieves the highest QA accuracy in the open retrieval setting on MuSiQue and 2Wiki while using 40-50 percent fewer tokens than IRCoT+HippoRAG2. Furthermore, GRASP leads on EM and F1 across all three datasets in the LongBench setting while using 30 percent fewer tokens than the next most accurate method. Finally, we introduce success economy - the amortized token cost per correct answer, weighted by difficulty - and advocate for efficiency-aware evaluation as a standard practice for agentic QA.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16598v1)
