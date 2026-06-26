---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Systematic Review of Key Retrieval-Augmented Generation (RAG) Systems: Progress, Gaps, and Future Directions"
authors: Agada Joseph Oche, Ademola Glory Folashade, Tirthankar Ghosal, Arpan Biswas
url: https://arxiv.org/abs/2507.18910v1
date: 2025-07-25
citationCount: 48
influentialCitationCount: 0
velocity: 4.4
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agentic-rag, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# A Systematic Review of Key Retrieval-Augmented Generation (RAG) Systems: Progress, Gaps, and Future Directions

**arXiv [2507.18910v1](https://arxiv.org/abs/2507.18910v1)** · 2025-07-25 · **48 citations** (0 influential · 4.4/mo) · Agada Joseph Oche, Ademola Glory Folashade, Tirthankar Ghosal, Arpan Biswas

## Abstract
Retrieval-Augmented Generation (RAG) represents a major advancement in natural language processing (NLP), combining large language models (LLMs) with information retrieval systems to enhance factual grounding, accuracy, and contextual relevance. This paper presents a comprehensive systematic review of RAG, tracing its evolution from early developments in open domain question answering to recent state-of-the-art implementations across diverse applications. The review begins by outlining the motivations behind RAG, particularly its ability to mitigate hallucinations and outdated knowledge in parametric models. Core technical components-retrieval mechanisms, sequence-to-sequence generation models, and fusion strategies are examined in detail. A year-by-year analysis highlights key milestones and research trends, providing insight into RAG's rapid growth. The paper further explores the deployment of RAG in enterprise systems, addressing practical challenges related to retrieval of proprietary data, security, and scalability. A comparative evaluation of RAG implementations is conducted, benchmarking performance on retrieval accuracy, generation fluency, latency, and computational efficiency. Persistent challenges such as retrieval quality, privacy concerns, and integration overhead are critically assessed. Finally, the review highlights emerging solutions, including hybrid retrieval approaches, privacy-preserving techniques, optimized fusion strategies, and agentic RAG architectures. These innovations point toward a future of more reliable, efficient, and context-aware knowledge-intensive NLP systems.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Background and Motivation 1.2 Scope and Objectives 1.3 Paper Organization 2 Methodology 2.1 Search Strategy Keywords and Databases. Initial Screening. 2.2 Inclusion and Exclusion Criteria 2.2.1 Inclusion Criteria 2.2.2 Exclusion Criteria 2.3 Data Extraction Synthesis Process. Ensuring Reliability. 3 Foundations of RAG 3.1 Definition and Key Concepts Retrieval-Augmented Generation (RAG) Chunking, Embedding, and (Re)ranking 3.2 Technical Components of RAG Retriever Module (Dense Passage Retrieval). Generator Module (Conditional Seq2Seq Model). Fusion Mechanisms and Answer Aggregation. Training and Optimization. 3.3 Historical Context Execution Flow of a RAG System. 4 Year-by-Year Progress in RAG 4.1 Initial Proposals and Early Research (2017–2019) 4.2 Major Milestones (2020–2024) 2020 — Birth of RAG. Dense neural retrieval. End-to-end retriever–generator architectures. Retrieval-aware pre-training. Applications beyond QA. Impact and open questions. 2021 — Improving Generati…

**Method / approach.** Methodology 2.1 Search Strategy Keywords and Databases. Initial Screening. 2.2 Inclusion and Exclusion Criteria 2.2.1 Inclusion Criteria 2.2.2 Exclusion Criteria 2.3 Data Extraction Synthesis Process. Ensuring Reliability. 3 Foundations of RAG 3.1 Definition and Key Concepts Retrieval-Augmented Generation (RAG) Chunking, Embedding, and (Re)ranking 3.2 Technical Components of RAG Retriever Module (Dense Passage Retrieval). Generator Module (Conditional Seq2Seq Model). Fusion Mechanisms and Answer Aggregation. Training and Optimization. 3.3 Historical Context Execution Flow of a RAG System. 4 Year-by-Year Progress in RAG 4.1 Initial Proposals and Early Research (2017–2019) 4.2 Major Milestones (2020–2024) 2020 — Birth of RAG. Dense neural retrieval. End-to-end retriever–generator architectures. Retrieval-aware pre-training. Applications beyond QA. Impact and open questions. 2021 — Improving Generation…

**Results.** experimented with learnable fusion weights or iterative retrieval-generation cycles, but the core idea is the same: the model must reconcile possibly conflicting or complementary information from multiple documents to produce a single, coherent answer. The choice of fusion affects the system’s ability to handle conflicting evidence and the credit assignment during training (i.e., which document gets “credit” for a correct answer). RAG’s probabilistic fusion provides a principled way to train the retriever and generator together by marginalizing, whereas direct concatenation treats the problem in a single forward pass of a generator (often fine for tasks where evidence is mostly additive or when using very large generators). Fusion strategies continue to be an active area of research, but they all serve the goal of effectively utilizing multiple retrieved pieces of text to improve answer completeness and correctness. Training and O…

**Conclusion.** Conclusion A Systematic Review of Key Retrieval-Augmented Generation (RAG) Systems: Progress, Gaps, and Future Directions Agada Joseph Oche Corresponding author: joe88data1@gmail.com Bredesen Center for Interdisciplinary Research, University of Tennessee, Knoxville, USA, 37996 Ademola Glory Folashade gloryademola112@gmail.com Bredesen Center for Interdisciplinary Research, University of Tennessee, Knoxville, USA, 37996 Tirthankar Ghosal National Center for Computational Sciences, Oak Ridge National Laboratory, Oak Ridge, USA, 37830 Arpan Biswas University of Tennessee-Oak Ridge Innovation Institute, University of Tennessee, Knoxville, USA, 37996 (July 25, 2025 ) Abstract Retrieval-Augmented Generation (RAG)…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.18910v1.md` · `raw/arxiv/2507.18910v1.fulltext.md`
