---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MMSearch-R1: Incentivizing LMMs to Search"
authors: Jinming Wu, Zihao Deng, Wei Li, Yiding Liu et al.
url: https://arxiv.org/abs/2506.20670v1
date: 2025-06-25
citationCount: 82
influentialCitationCount: 18
velocity: 6.9
ingested: 2026-06-22
tags: [agentic-rl, agentic-rag, arxiv, 2025, cited]
---

# MMSearch-R1: Incentivizing LMMs to Search

**arXiv [2506.20670v1](https://arxiv.org/abs/2506.20670v1)** · 2025-06-25 · **82 citations** (18 influential · 6.9/mo) · Jinming Wu, Zihao Deng, Wei Li, Yiding Liu et al.

## Abstract
Robust deployment of large multimodal models (LMMs) in real-world scenarios requires access to external knowledge sources, given the complexity and dynamic nature of real-world information. Existing approaches such as retrieval-augmented generation (RAG) and prompt engineered search agents rely on rigid pipelines, often leading to inefficient or excessive search behaviors. We present MMSearch-R1, the first end-to-end reinforcement learning framework that enables LMMs to perform on-demand, multi-turn search in real-world Internet environments. Our framework integrates both image and text search tools, allowing the model to reason about when and how to invoke them guided by an outcome-based reward with a search penalty. To support training, We collect a multimodal search VQA dataset through a semi-automated pipeline that covers diverse visual and textual knowledge needs and curate a search-balanced subset with both search-required and search-free samples, which proves essential for shaping efficient and on-demand search behavior. Extensive experiments on knowledge-intensive and info-seeking VQA tasks show that our model not only outperforms RAG-based baselines of the same model size, but also matches the performance of a larger RAG-based model while reducing search calls by over 30%. We further analyze key empirical findings to offer actionable insights for advancing research in multimodal search.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Building Iterative Multimodal Search-Integrated RL Framework 2.1 Group Relative Policy Optimization (GRPO) 2.2 Multimodal Search Tools 2.3 Rollout with Multi-turn Multimodal Search 2.4 Reward Modeling 3 Curating Search-balanced VQA Datasets 3.1 Training Dataset Construction 3.2 Test Dataset Annotation 4 Experiments 4.1 Setups 4.2 Findings Finding 1: RL training enables models to better recognize the boundaries of their knowledge and perform on-demand search more effectively. Finding 2: RL training enhances the model’s ability to generate effective text queries and summarize retrieved information. Finding 3: RL improves the model’s ability to utilize its internal knowledge. Finding 4: RL achieves greater performance improvements and exhibits higher data efficiency compared to supervised SFT. Finding 5: Training with balanced data and a search penalty in the reward effectively guide the model to perform on-demand search. 5 Conclusion A Related Work A.1 Large Multimodal Models (LMMs) A.2 Large Models with Extern…

**Method / approach.** methods follow a fixed retrieve-then-generate workflow grounded in static knowledge bases, often resulting in over-retrieval, high computational cost, and the unrealistic assumption that all required information is already present in the corpus. Such a controlled setting fails to capture the dynamic and unpredictable nature of real-world scenarios, rendering these systems vulnerable in practical deployments. On the other hand, prompt-engineered agents interact with real-world search engines, but the model parameters are not optimized through learning. As a result, the models do not truly learn how to interact effectively with search tools or adapt their behavior to open world environments. This motivates the development of methods that teach models to search on demand and interact effectively with search tools, ensuring practical usability in dynamic real-world settings. Recent advances, such as OpenAI’s o series rl/openai-o1 ; openai-o3_o4_mini_syscard and DeepSeek-R1 rl/deepseek-…

**Results.** Experiments 4.1 Setups 4.2 Findings Finding 1: RL training enables models to better recognize the boundaries of their knowledge and perform on-demand search more effectively. Finding 2: RL training enhances the model’s ability to generate effective text queries and summarize retrieved information. Finding 3: RL improves the model’s ability to utilize its internal knowledge. Finding 4: RL achieves greater performance improvements and exhibits higher data efficiency compared to supervised SFT. Finding 5: Training with balanced data and a search penalty in the reward effectively guide the model to perform on-demand search. 5 Conclusion A Related Work A.1 Large Multimodal Models (LMMs) A.2 Large Models with External Knowledge Access A.2.1 Retrieval-Augmented Generation (RAG) A.2.2 Search-Augmented Approaches A.3 Reinforcement Learning-powered Search Agents B Group Relative Policy Optimization (…

**Conclusion.** Conclusion A Related Work A.1 Large Multimodal Models (LMMs) A.2 Large Models with External Knowledge Access A.2.1 Retrieval-Augmented Generation (RAG) A.2.2 Search-Augmented Approaches A.3 Reinforcement Learning-powered Search Agents B Group Relative Policy Optimization (GRPO) Algorithm C Multimodal Search Tools D Prompts D.1 Prompts for FVQA-auto-ac VQA Generation D.2 Prompts for RL Training D.3 Prompts for Webpage Summarization Model D.4 Prompt for Direct Answer Baseline D.5 Prompts for RAG Workflow Baseline D.6 Prompts for LLM-as-Judge Evaluation E Details of Benchmark Datasets F Details of Experimental Implementation F.1 RL Training Setting F.2 SFT Training Setting F.3 Evaluati…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]]
- **Raw:** `raw/arxiv/2506.20670v1.md` · `raw/arxiv/2506.20670v1.fulltext.md`
