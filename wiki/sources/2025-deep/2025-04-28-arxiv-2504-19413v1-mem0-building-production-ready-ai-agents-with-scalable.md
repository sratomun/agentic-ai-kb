---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory"
authors: Prateek Chhikara, Dev Khant, Saket Aryan, Taranjeet Singh et al.
url: https://arxiv.org/abs/2504.19413v1
date: 2025-04-28
citationCount: 412
influentialCitationCount: 79
velocity: 29.86
ingested: 2026-06-22
tags: [knowledge-graph, agent-reliability, agentic-rag, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory

**arXiv [2504.19413v1](https://arxiv.org/abs/2504.19413v1)** · 2025-04-28 · **412 citations** (79 influential · 29.86/mo) · Prateek Chhikara, Dev Khant, Saket Aryan, Taranjeet Singh et al.

**Significance:** The reference for production agent memory at scale — a touchstone for 'agents that remember across sessions'.

## Abstract
Large Language Models (LLMs) have demonstrated remarkable prowess in generating contextually coherent responses, yet their fixed context windows pose fundamental challenges for maintaining consistency over prolonged multi-session dialogues. We introduce Mem0, a scalable memory-centric architecture that addresses this issue by dynamically extracting, consolidating, and retrieving salient information from ongoing conversations. Building on this foundation, we further propose an enhanced variant that leverages graph-based memory representations to capture complex relational structures among conversational elements. Through comprehensive evaluations on LOCOMO benchmark, we systematically compare our approaches against six baseline categories: (i) established memory-augmented systems, (ii) retrieval-augmented generation (RAG) with varying chunk sizes and k-values, (iii) a full-context approach that processes the entire conversation history, (iv) an open-source memory solution, (v) a proprietary model system, and (vi) a dedicated memory management platform. Empirical results show that our methods consistently outperform all existing memory systems across four question categories: single-hop, temporal, multi-hop, and open-domain. Notably, Mem0 achieves 26% relative improvements in the LLM-as-a-Judge metric over OpenAI, while Mem0 with graph memory achieves around 2% higher overall score than the base configuration. Beyond accuracy gains, we also markedly reduce computational overhead compared to full-context method. In particular, Mem0 attains a 91% lower p95 latency and saves more than 90% token cost, offering a compelling balance between advanced reasoning capabilities and practical deployment constraints. Our findings highlight critical role of structured, persistent memory mechanisms for long-term conversational coherence, paving the way for more reliable and efficient LLM-driven AI agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Proposed Methods 2.1 Mem0 2.2 Mem0 g superscript Mem0 𝑔 \texttt{Mem0}^{\tiny g} Mem0 start_POSTSUPERSCRIPT italic_g end_POSTSUPERSCRIPT 3 Experimental Setup 3.1 Dataset 3.2 Evaluation Metrics (1) Performance Metrics (2) Deployment Metrics 3.3 Baselines Established LOCOMO Benchmarks Open-Source Memory Solutions Retrieval-Augmented Generation (RAG) Full-Context Processing Proprietary Models Memory Providers 4 Evaluation Results, Analysis and Discussion. 4.1 Performance Comparison Across Memory-Enabled Systems Single-Hop Question Performance Multi-Hop Question Performance Open-Domain Performance Temporal Reasoning Performance 4.2 Cross-Category Analysis 4.3 Performance Comparison of Mem0 and Mem0 g superscript Mem0 𝑔 \texttt{Mem0}^{\tiny g} Mem0 start_POSTSUPERSCRIPT italic_g end_POSTSUPERSCRIPT Against RAG Approaches and Full-Context Model 4.4 Latency Analysis 4.5 Memory System Overhead: Token Analysis and Construction Time 5 Conclusion and Future Work 6 Acknowledgments A Prompts B Algorithm…

**Method / approach.** Methods 2.1 Mem0 2.2 Mem0 g superscript Mem0 𝑔 \texttt{Mem0}^{\tiny g} Mem0 start_POSTSUPERSCRIPT italic_g end_POSTSUPERSCRIPT 3 Experimental Setup 3.1 Dataset 3.2 Evaluation Metrics (1) Performance Metrics (2) Deployment Metrics 3.3 Baselines Established LOCOMO Benchmarks Open-Source Memory Solutions Retrieval-Augmented Generation (RAG) Full-Context Processing Proprietary Models Memory Providers 4 Evaluation Results, Analysis and Discussion. 4.1 Performance Comparison Across Memory-Enabled Systems Single-Hop Question Performance Multi-Hop Question Performance Open-Domain Performance Temporal Reasoning Performance 4.2 Cross-Category Analysis 4.3 Performance Comparison of Mem0 and Mem0 g superscript Mem0 𝑔 \texttt{Mem0}^{\tiny g} Mem0 start_POSTSUPERSCRIPT italic_g end_POSTSUPERSCRIPT Against RAG Approaches and Full-Context Model 4.4 Latency Analysis 4.5 Memory System Overhead: Token Analysis and Construction Time 5…

**Results.** Experimental Setup 3.1 Dataset 3.2 Evaluation Metrics (1) Performance Metrics (2) Deployment Metrics 3.3 Baselines Established LOCOMO Benchmarks Open-Source Memory Solutions Retrieval-Augmented Generation (RAG) Full-Context Processing Proprietary Models Memory Providers 4 Evaluation Results, Analysis and Discussion. 4.1 Performance Comparison Across Memory-Enabled Systems Single-Hop Question Performance Multi-Hop Question Performance Open-Domain Performance Temporal Reasoning Performance 4.2 Cross-Category Analysis 4.3 Performance Comparison of Mem0 and Mem0 g superscript Mem0 𝑔 \texttt{Mem0}^{\tiny g} Mem0 start_POSTSUPERSCRIPT italic_g end_POSTSUPERSCRIPT Against RAG Approaches and Full-Context Model 4.4 Latency Analysis 4.5 Memory System Overhead: Token Analysis and Construction Time 5 Conclusion and Future Work 6 Acknowledgments A Prompts B Algorithm C Selected B…

**Conclusion.** Conclusion and Future Work 6 Acknowledgments A Prompts B Algorithm C Selected Baselines LoCoMo ReadAgent MemoryBank MemGPT A-Mem Mem0 : Building Production - Ready AI Agents with Scalable Long - Term Memory Prateek Chhikara Dev Khant Saket Aryan Taranjeet Singh and Deshraj Yadav research@mem0.ai Abstract Large Language Models (LLMs) have demonstrated remarkable prowess in generating contextually coherent responses, yet their fixed context windows pose fundamental challenges for maintaining consistency over prolonged multi-session dialogues. We introduce Mem0 , a scalable memory-centric architecture that addresses this issue by dynamically extracting, consolidating, and retrieving salient inf…

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mem0]]
- **Raw:** `raw/arxiv/2504.19413v1.md` · `raw/arxiv/2504.19413v1.fulltext.md`
