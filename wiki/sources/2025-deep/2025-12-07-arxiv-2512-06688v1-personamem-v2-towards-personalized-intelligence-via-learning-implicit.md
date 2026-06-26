---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PersonaMem-v2: Towards Personalized Intelligence via Learning Implicit User Personas and Agentic Memory"
authors: Bowen Jiang, Yuan Yuan, Maohao Shen, Zhuoqun Hao et al.
url: https://arxiv.org/abs/2512.06688v1
date: 2025-12-07
citationCount: 47
influentialCitationCount: 8
velocity: 7.26
ingested: 2026-06-22
tags: [agent-memory, agentic-ai, arxiv, 2025, cited]
---

# PersonaMem-v2: Towards Personalized Intelligence via Learning Implicit User Personas and Agentic Memory

**arXiv [2512.06688v1](https://arxiv.org/abs/2512.06688v1)** · 2025-12-07 · **47 citations** (8 influential · 7.26/mo) · Bowen Jiang, Yuan Yuan, Maohao Shen, Zhuoqun Hao et al.

## Abstract
Personalization is one of the next milestones in advancing AI capability and alignment. We introduce PersonaMem-v2, the state-of-the-art dataset for LLM personalization that simulates 1,000 realistic user-chatbot interactions on 300+ scenarios, 20,000+ user preferences, and 128k-token context windows, where most user preferences are implicitly revealed to reflect real-world interactions. Using this data, we investigate how reinforcement fine-tuning enables a model to improve its long-context reasoning capabilities for user understanding and personalization. We also develop a framework for training an agentic memory system, which maintains a single, human-readable memory that grows with each user over time. In our experiments, frontier LLMs still struggle with implicit personalization, achieving only 37-48% accuracy. While they support long context windows, reasoning remains the bottleneck for implicit personalization tasks. Using reinforcement fine-tuning, we successfully train Qwen3-4B to outperforms GPT-5, reaching 53% accuracy in implicit personalization. Moreover, our agentic memory framework achieves state-of-the-art 55% accuracy while using 16x fewer input tokens, relying on a 2k-token memory instead of full 32k conversation histories. These results underscore the impact of our dataset and demonstrate agentic memory as a scalable path toward real-world personalized intelligence.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Overview of PersonaMem-v2: Implicit Personas 2.1 Comprehensive User Personas 2.2 Multi-Session Realistic Conversation Histories 2.3 User Privacy-Aware Design 2.4 In-Situ User Queries 2.5 Ensuring High Quality of Data 3 Towards Personalized Intelligence 3.1 RL with Long-Context Reasoning 3.2 RL with Agentic Memory: Toward Scalable Personalization 4 Experimental Results 4.1 Benchmarking Frontier LLMs in Personalization 4.1.1 Frontier LLMs still struggle to infer implicit user preferences 4.1.2 Reasoning, not long-context capabilities, drives success in implicit personalization 4.1.3 Implicit personalization varies systematically across preference types 4.2 Training Long-context Reasoning for Personalization 4.2.1 Reinforcement learning incentives reasoning toward personalization 4.2.2 Hybrid reward signals unlock better RL toward personalization 4.3 Training Agentic Memory for Personalization 4.3.1 Agentic memory delivers state-of-the-art performance with unmatched efficiency 4.3.2 Human-readable memory enables tra…

**Method / approach.** methods such as RLHF (Ouyang et al. , 2022 ) and DPO (Rafailov et al. , 2023 ) form the foundation of preference-based fine-tuning but primarily capture population-level rather than individual user preferences. Building on this, P-RLHF (Li et al. , 2024 ) learns compact representations of personal preferences. Optimization-focused studies (Khaki et al. , 2024 ; Tajwar et al. , 2024 ) emphasize using model-generated, on-policy data to achieve more robust preference learning. Feedback-based methods (Bu et al. , 2025 ; Zhu et al. , 2025 ; Shi et al. , 2024 ) refine responses during generation. In this work, we further explore reinforcement fine-tuning with verifiable rewards (Liu et al. , 2025b ; Guo et al. , 2025 ) , leveraging our high-quality, comprehensively annotated data to provide verification signals. 5.2 The Landscape of Existing Personalization Benchmarks Despite algorithmic efforts, high-quality personalization data that better mimic real-world scenarios is essenti…

**Results.** Experimental Results 4.1 Benchmarking Frontier LLMs in Personalization 4.1.1 Frontier LLMs still struggle to infer implicit user preferences 4.1.2 Reasoning, not long-context capabilities, drives success in implicit personalization 4.1.3 Implicit personalization varies systematically across preference types 4.2 Training Long-context Reasoning for Personalization 4.2.1 Reinforcement learning incentives reasoning toward personalization 4.2.2 Hybrid reward signals unlock better RL toward personalization 4.3 Training Agentic Memory for Personalization 4.3.1 Agentic memory delivers state-of-the-art performance with unmatched efficiency 4.3.2 Human-readable memory enables transparency and user control 5 Related Work 5.1 Personalization Techniques: Retrieval, Memory, and Alignment 5.2 The Landscape of Existing Personalization Benchmarks 6 Conclusion and Future Work References License: arXiv.org per…

**Conclusion.** Conclusion and Future Work References License: arXiv.org perpetual non-exclusive license arXiv:2512.06688v1 [cs.CL] 07 Dec 2025 PersonaMem-v2 : Towards Personalized Intelligence via Learning Implicit User Personas and Agentic Memory Bowen Jiang 1 , Yuan Yuan 1 , Maohao Shen 2 , Zhuoqun Hao 1 , Zhangchen Xu 3 , Zichen Chen 4 , Ziyi Liu 6 , Anvesh R. Vijjini 7 , Jiashu He 1 , Hanchao Yu 5 , Radha Poovendran 3 , Gregory Wornell 2 , Lyle Ungar 1 , Dan Roth 1 , Sihao Chen 8 , Camillo J. Taylor 1 1 1 footnotemark: 1 University of Pennsylvania 1 , Massachusetts Institute of Technology 2 , University of Washington 3 , University of California Santa Barbara 4 , Meta 5 , University of Southern California 6 , University of Nort…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2512.06688v1.md` · `raw/arxiv/2512.06688v1.fulltext.md`
