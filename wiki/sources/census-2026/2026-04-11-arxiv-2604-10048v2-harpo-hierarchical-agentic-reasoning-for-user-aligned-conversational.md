---
type: source
source_type: arxiv
title: "HARPO: Hierarchical Agentic Reasoning for User-Aligned Conversational Recommendation"
authors: Subham Raj, Aman Vaibhav Jha, Mayank Anand, Sriparna Saha
url: https://arxiv.org/abs/2604.10048v2
date: 2026-04-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.IR
tags: [recommendation-agents, multi-agent-systems, arxiv, auto-ingested]
---

# HARPO: Hierarchical Agentic Reasoning for User-Aligned Conversational Recommendation

**arXiv:** [2604.10048v2](https://arxiv.org/abs/2604.10048v2) · 2026-04-11 · cs.IR
**Authors:** Subham Raj, Aman Vaibhav Jha, Mayank Anand, Sriparna Saha

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Conversational recommender systems (CRSs) operate under incremental preference revelation, requiring recommendation decisions under uncertainty. While recent LLM-based approaches achieve strong performance on proxy metrics such as Recall@K and BLEU, they often fail to deliver high-quality, user-aligned recommendations in practice, as they optimize intermediate objectives like retrieval accuracy or fluent generation rather than recommendation quality itself. We propose HARPO (Hierarchical Agentic Reasoning with Preference Optimization), an agentic framework that reframes conversational recommendation as a structured decision-making process optimized for multi-dimensional recommendation quality. HARPO integrates (i) hierarchical preference learning that decomposes recommendation quality into interpretable dimensions (relevance, diversity, satisfaction, and engagement) with context-dependent weighting; (ii) deliberative tree-search reasoning guided by a learned value network evaluating candidate paths on predicted quality; and (iii) domain-agnostic reasoning abstractions through Virtual Tool Operations and multi-agent refinement. We evaluate HARPO on ReDial, INSPIRED, and MUSE, demonstrating consistent improvements over strong baselines on recommendation-centric metrics while maintaining competitive response quality.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10048v2)
