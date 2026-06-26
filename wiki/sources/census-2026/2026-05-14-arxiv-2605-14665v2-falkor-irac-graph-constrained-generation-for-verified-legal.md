---
type: source
source_type: arxiv
title: "Falkor-IRAC: Graph-Constrained Generation for Verified Legal Reasoning in Indian Judicial AI"
authors: Joy Bose
url: https://arxiv.org/abs/2605.14665v2
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, agentic-rag, arxiv, auto-ingested]
---

# Falkor-IRAC: Graph-Constrained Generation for Verified Legal Reasoning in Indian Judicial AI

**arXiv:** [2605.14665v2](https://arxiv.org/abs/2605.14665v2) · 2026-05-14 · cs.AI
**Authors:** Joy Bose

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Legal reasoning is not semantic similarity search. A court judgment encodes constrained symbolic reasoning: precedent propagation, procedural state transitions, and statute-bound inference. These are properties that vector-based retrieval-augmented generation (RAG) cannot faithfully represent. Hallucinated precedents, outdated statute citations, and unsupported reasoning chains remain persistent failure modes in LLM-based legal AI, with real consequences for access to justice in high-caseload jurisdictions such as India. This paper presents Falkor-IRAC, a graph-constrained generation framework for Indian legal AI that grounds generation in structured reasoning over an IRAC (Issue, Rule, Analysis, Conclusion) knowledge graph. Judgments from the Supreme Court and High Courts of India are ingested as IRAC node structures enriched with procedural state transitions, precedent relationships, and statutory references, stored in FalkorDB for low-latency agentic traversal. At inference time, LLM-generated answers are accepted only if a valid supporting path can be traced through the graph, a check performed by a falsifiability oracle called the Verifier Agent. The system also detects doctrinal conflicts as a first-class output rather than silently resolving them. Falkor-IRAC is evaluated using graph-native metrics: citation grounding accuracy, path validity rate, hallucinated precedent rate, and conflict detection rate. These metrics are argued to be more appropriate for legal reasoning evaluation than BLEU and ROUGE. On a proof-of-concept corpus of 51 Supreme Court judgments, the Verifier Agent correctly validated citations on completed queries and correctly rejected fabricated citations. Evaluation against vector-only RAG baselines is left for future work. The companion InIRAC dataset, 500+ structured Indian court judgments with IRAC annotations, is released alongside this paper.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14665v2)
