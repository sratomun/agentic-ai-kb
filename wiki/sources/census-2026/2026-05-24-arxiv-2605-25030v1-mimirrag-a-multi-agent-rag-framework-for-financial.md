---
type: source
source_type: arxiv
title: "MimirRAG: A Multi-Agent RAG Framework for Financial Data Retrieval with Metadata Integration"
authors: Magnus Samuelsen, Wilmer Nyström, Somnath Mazumdar, Mansoor Hussain et al.
url: https://arxiv.org/abs/2605.25030v1
date: 2026-05-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.LG
tags: [finance-agents, agent-reliability, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MimirRAG: A Multi-Agent RAG Framework for Financial Data Retrieval with Metadata Integration

**arXiv:** [2605.25030v1](https://arxiv.org/abs/2605.25030v1) · 2026-05-24 · cs.LG
**Authors:** Magnus Samuelsen, Wilmer Nyström, Somnath Mazumdar, Mansoor Hussain et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-augmented generation (RAG) systems offer a promising approach to reduce hallucinations and improve answer accuracy in large language models (LLMs), a requirement for reliable, financial analysis where answers must be grounded in verifiable evidence from filings rather than generated from model priors. However, designing RAG systems that extract meaningful insights from mixed financial documents and integrate into analyst workflows remains challenging. This paper introduces MimirRAG (Metadata-Integrated Multi-Agent Information Retrieval), a multi-agent RAG system developed iteratively to address these challenges. MimirRAG features a modular pipeline encompassing structure-preserving parsing of PDF filings, table-aware chunking, metadata extraction, agent-based retrieval with query planning and hybrid search, validation, and context-aware generation with numerical reasoning support. Our ablation study identifies three key technical enablers for effective financial RAG: metadata integration, table-aware chunking, and an agentic workflow. MimirRAG was evaluated quantitatively using FinanceBench and qualitatively through expert validation with four financial analysts. The system achieved 89.3% accuracy on FinanceBench, outperforming the original benchmark baselines. Expert feedback highlighted that successful deployment also requires calibrated trust, comprehensive data integration, and user personalization. We conclude that combining multi-agent RAG architecture with human-centric design principles can improve the extraction of meaningful insights in financial analysis.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.25030v1)
