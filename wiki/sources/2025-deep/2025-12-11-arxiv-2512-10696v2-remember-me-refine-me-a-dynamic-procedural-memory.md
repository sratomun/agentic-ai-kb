---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Remember Me, Refine Me: A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution"
authors: Zouying Cao, Jiaji Deng, Li Yu, Weikang Zhou et al.
url: https://arxiv.org/abs/2512.10696v2
date: 2025-12-11
citationCount: 39
influentialCitationCount: 7
velocity: 6.15
ingested: 2026-06-22
tags: [agent-reliability, self-evolving-agents, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Remember Me, Refine Me: A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution

**arXiv [2512.10696v2](https://arxiv.org/abs/2512.10696v2)** · 2025-12-11 · **39 citations** (7 influential · 6.15/mo) · Zouying Cao, Jiaji Deng, Li Yu, Weikang Zhou et al.

## Abstract
Procedural memory enables large language model (LLM) agents to internalize "how-to" knowledge, theoretically reducing redundant trial-and-error. However, existing frameworks predominantly suffer from a "passive accumulation" paradigm, treating memory as a static append-only archive. To bridge the gap between static storage and dynamic reasoning, we propose $\textbf{ReMe}$ ($\textit{Remember Me, Refine Me}$), a comprehensive framework for experience-driven agent evolution. ReMe innovates across the memory lifecycle via three mechanisms: 1) $\textit{multi-faceted distillation}$, which extracts fine-grained experiences by recognizing success patterns, analyzing failure triggers and generating comparative insights; 2) $\textit{context-adaptive reuse}$, which tailors historical insights to new contexts via scenario-aware indexing; and 3) $\textit{utility-based refinement}$, which autonomously adds valid memories and prunes outdated ones to maintain a compact, high-quality experience pool. Extensive experiments on BFCL-V3 and AppWorld demonstrate that ReMe establishes a new state-of-the-art in agent memory system. Crucially, we observe a significant memory-scaling effect: Qwen3-8B equipped with ReMe outperforms larger, memoryless Qwen3-14B, suggesting that self-evolving memory provides a computation-efficient pathway for lifelong learning. We release our code and the $\texttt{reme.library}$ dataset to facilitate further research.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 Methodology 3.1 Overview of ReMe 3.2 Experience Acquisition 3.3 Experience Reuse 3.4 Experience Refinement 4 Experiments 4.1 Experimental Settings Datasets. Metrics. Baselines. Implementation Details. 4.2 Main Results 4.3 Ablation Studies Granularity Ablations. Component Ablations. Retrieval Key Ablations. 4.4 More Analysis Agent Gains More with Stronger LLM summ \textbf{LLM}_{\textbf{summ}} . Effect of Retrieved Experience Number. Computational Overheads. Error Analysis. 5 Conclusion References A Use of AI Assistants B Experimental Details B.1 Datasets and Evaluation Metrics BFCL-V3 AppWorld B.2 Baseline Details LangMem A-Mem B.3 Model Configuration B.4 Implementation Details B.4.1 For Experience Acquisition B.4.2 For Experience Retrieval C Experience Examples D Detailed Experimental Results D.1 Generalizability across Different Models D.2 Results on Larger-scale Benchmark D.3 Retrieval Key Analysis E Case Study License: arXiv.org…

**Method / approach.** Methodology 3.1 Overview of ReMe 3.2 Experience Acquisition 3.3 Experience Reuse 3.4 Experience Refinement 4 Experiments 4.1 Experimental Settings Datasets. Metrics. Baselines. Implementation Details. 4.2 Main Results 4.3 Ablation Studies Granularity Ablations. Component Ablations. Retrieval Key Ablations. 4.4 More Analysis Agent Gains More with Stronger LLM summ \textbf{LLM}_{\textbf{summ}} . Effect of Retrieved Experience Number. Computational Overheads. Error Analysis. 5 Conclusion References A Use of AI Assistants B Experimental Details B.1 Datasets and Evaluation Metrics BFCL-V3 AppWorld B.2 Baseline Details LangMem A-Mem B.3 Model Configuration B.4 Implementation Details B.4.1 For Experience Acquisition B.4.2 For Experience Retrieval C Experience Examples D Detailed Experimental Results D.1 Generalizability across Different Models D.2 Results on Larger-scale Benchmark D…

**Results.** Experiments 4.1 Experimental Settings Datasets. Metrics. Baselines. Implementation Details. 4.2 Main Results 4.3 Ablation Studies Granularity Ablations. Component Ablations. Retrieval Key Ablations. 4.4 More Analysis Agent Gains More with Stronger LLM summ \textbf{LLM}_{\textbf{summ}} . Effect of Retrieved Experience Number. Computational Overheads. Error Analysis. 5 Conclusion References A Use of AI Assistants B Experimental Details B.1 Datasets and Evaluation Metrics BFCL-V3 AppWorld B.2 Baseline Details LangMem A-Mem B.3 Model Configuration B.4 Implementation Details B.4.1 For Experience Acquisition B.4.2 For Experience Retrieval C Experience Examples D Detailed Experimental Results D.1 Generalizability across Different Models D.2 Results on Larger-scale Benchmark D.3 Retrieval Key Analysis E Case Study License: arXiv.org perpetual…

**Conclusion.** Conclusion References A Use of AI Assistants B Experimental Details B.1 Datasets and Evaluation Metrics BFCL-V3 AppWorld B.2 Baseline Details LangMem A-Mem B.3 Model Configuration B.4 Implementation Details B.4.1 For Experience Acquisition B.4.2 For Experience Retrieval C Experience Examples D Detailed Experimental Results D.1 Generalizability across Different Models D.2 Results on Larger-scale Benchmark D.3 Retrieval Key Analysis E Case Study License: arXiv.org perpetual non-exclusive license arXiv:2512.10696v2 [cs.AI] 15 Apr 2026 Remember Me, Refine Me : A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution Zouying Cao 1,3, , Jiaji Deng 2 , Li Yu 2…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[bfcl]] · [[qwen]]
- **Raw:** `raw/arxiv/2512.10696v2.md` · `raw/arxiv/2512.10696v2.fulltext.md`
