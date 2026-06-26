---
type: source
source_type: arxiv
title: "Agentic Retrieval-Augmented Generation for Financial Document Question Answering"
authors: Yang Shu, Yingmin Liu, Zequn Xie
url: https://arxiv.org/abs/2605.05409v1
date: 2026-05-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [finance-agents, agent-reliability, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Agentic Retrieval-Augmented Generation for Financial Document Question Answering

**arXiv:** [2605.05409v1](https://arxiv.org/abs/2605.05409v1) · 2026-05-06 · cs.AI
**Authors:** Yang Shu, Yingmin Liu, Zequn Xie

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Financial document question answering (QA) demands complex multi-step numerical reasoning over heterogeneous evidence--structured tables, textual narratives, and footnotes--scattered across corporate filings. Existing retrieval-augmented generation (RAG) approaches adopt a single-pass retrieve-then-generate paradigm that struggles with the compositional reasoning chains prevalent in financial analysis. We propose FinAgent-RAG, an agentic RAG framework that orchestrates iterative retrieval-reasoning loops with self-verification, specifically engineered for the precision requirements of financial numerical reasoning. The framework integrates three domain-specific innovations: (1) a Contrastive Financial Retriever trained with hard negative mining to distinguish semantically similar but numerically distinct financial passages, (2) a Program-of-Thought reasoning module that generates executable Python code for precise arithmetic rather than relying on error-prone LLM-based mental computation, and (3) an Adaptive Strategy Router that dynamically allocates computational resources based on question complexity, reducing API costs by 41.3% on FinQA while preserving accuracy. Extensive experiments on three benchmark datasets--FinQA, ConvFinQA, and TAT-QA--demonstrate that FinAgent-RAG achieves 76.81%, 78.46%, and 74.96% execution accuracy respectively, outperforming the strongest baseline by 5.62--9.32 percentage points. Ablation studies, cross-backbone evaluation with four LLMs, and deployment cost analysis confirm the framework's robustness and practical viability for financial institutions.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.05409v1)
