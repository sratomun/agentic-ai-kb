---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Process vs. Outcome Reward: Which is Better for Agentic RAG Reinforcement Learning"
authors: Wenlin Zhang, Xiangyang Li, Kuicai Dong, Yichao Wang et al.
url: https://arxiv.org/abs/2505.14069v3
date: 2025-05-20
citationCount: 67
influentialCitationCount: 6
velocity: 5.12
ingested: 2026-06-22
tags: [agentic-rl, agentic-rag, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Process vs. Outcome Reward: Which is Better for Agentic RAG Reinforcement Learning

**arXiv [2505.14069v3](https://arxiv.org/abs/2505.14069v3)** · 2025-05-20 · **67 citations** (6 influential · 5.12/mo) · Wenlin Zhang, Xiangyang Li, Kuicai Dong, Yichao Wang et al.

## Abstract
Retrieval-augmented generation (RAG) enhances the text generation capabilities of large language models (LLMs) by integrating external knowledge and up-to-date information. However, traditional RAG systems are limited by static workflows and lack the adaptability required for multistep reasoning and complex task management. To address these limitations, agentic RAG systems (e.g., DeepResearch) have been proposed, enabling dynamic retrieval strategies, iterative context refinement, and adaptive workflows for handling complex search queries beyond the capabilities of conventional RAG. Recent advances, such as Search-R1, have demonstrated promising gains using outcome-based reinforcement learning, where the correctness of the final answer serves as the reward signal. Nevertheless, such outcome-supervised agentic RAG methods face challenges including low exploration efficiency, gradient conflict, and sparse reward signals. To overcome these challenges, we propose to utilize fine-grained, process-level rewards to improve training stability, reduce computational costs, and enhance efficiency. Specifically, we introduce a novel method ReasonRAG that automatically constructs RAG-ProGuide, a high-quality dataset providing process-level rewards for (i) query generation, (ii) evidence extraction, and (iii) answer generation, thereby enhancing model inherent capabilities via process-supervised reinforcement learning. With the process-level policy optimization, the proposed framework empowers LLMs to autonomously invoke search, generate queries, extract relevant evidence, and produce final answers. Compared to existing approaches such as Search-R1 and traditional RAG systems, ReasonRAG, leveraging RAG-ProGuide, achieves superior performance on five benchmark datasets using only 5k training instances, significantly fewer than the 90k training instances required by Search-R1.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 ReasonRAG Framework 2.1 Framework Overview 2.2 Process-Supervised Data Generation 2.2.1 Shortest Path Reward Estimation (SPRE) 2.2.2 Monte Carlo Tree Search (MCTS) for Process-level Exploration 2.2.3 RAG-ProGuide Dataset Construction. Dataset Statistics. 2.3 Process-Supervised Preference Optimization 2.4 Agentic RAG Inference 3 Experiments 3.1 Experimental Setup 3.2 Main Results 3.3 Training Efficiency 3.4 Effectiveness of Different Optimization Strategies 3.5 Impact of Search on Performance Performance vs. Retrieval Steps. Performance vs. Number of Retrieved Documents. 4 Related Works Prompt-Based Agentic RAG. RL-Based Agentic RAG. 5 Conclusion A Monte Carlo Tree Search for Process-level Reward B Process Evaluation C Case Study D Evaluation Dataset Details Evaluation Datasets. Evaluation Details. E Implementation Details E.1 Implementation Details of ReasonRAG E.2 Implementation Details of Baselines F Prompt Instructions G License Agreement H Limitations I Societal Im…

**Method / approach.** methods face challenges including low exploration efficiency, gradient conflict, and sparse reward signals. To overcome these challenges, we propose to utilize fine-grained, process-level rewards to improve training stability, reduce computational costs, and enhance efficiency. Specifically, we introduce a novel method ReasonRAG that automatically constructs RAG-ProGuide , a high-quality dataset providing process-level rewards for (i) query generation, (ii) evidence extraction, and (iii) answer generation, thereby enhancing model inherent capabilities via process-supervised reinforcement learning. With the process-level policy optimization, the proposed framework empowers LLMs to autonomously invoke search, generate queries, extract relevant evidence, and produce final answers. Compared to existing approaches such as Search-R1 and traditional RAG systems, ReasonRAG , leveraging RAG-ProGuide , achieves superior performance on five benchmark datasets using only 5k training instances, si…

**Results.** Experiments 3.1 Experimental Setup 3.2 Main Results 3.3 Training Efficiency 3.4 Effectiveness of Different Optimization Strategies 3.5 Impact of Search on Performance Performance vs. Retrieval Steps. Performance vs. Number of Retrieved Documents. 4 Related Works Prompt-Based Agentic RAG. RL-Based Agentic RAG. 5 Conclusion A Monte Carlo Tree Search for Process-level Reward B Process Evaluation C Case Study D Evaluation Dataset Details Evaluation Datasets. Evaluation Details. E Implementation Details E.1 Implementation Details of ReasonRAG E.2 Implementation Details of Baselines F Prompt Instructions G License Agreement H Limitations I Societal Impacts Process vs. Outcome Reward: Which is Better for Agentic RAG Reinforcement Learning Wenlin Zhang 1,∗ , Xiangyang Li 2,∗ , Kuicai Dong 2, , Yichao Wang 2,† , Pengyue Jia 1 , Xiaopeng Li 1 , Yingyi Zhang 1 , Derong Xu 1…

**Conclusion.** Conclusion A Monte Carlo Tree Search for Process-level Reward B Process Evaluation C Case Study D Evaluation Dataset Details Evaluation Datasets. Evaluation Details. E Implementation Details E.1 Implementation Details of ReasonRAG E.2 Implementation Details of Baselines F Prompt Instructions G License Agreement H Limitations I Societal Impacts Process vs. Outcome Reward: Which is Better for Agentic RAG Reinforcement Learning Wenlin Zhang 1,∗ , Xiangyang Li 2,∗ , Kuicai Dong 2, , Yichao Wang 2,† , Pengyue Jia 1 , Xiaopeng Li 1 , Yingyi Zhang 1 , Derong Xu 1 , Zhaocheng Du 2 , Huifeng Guo 2 , Ruiming Tang 2 , Xiangyu Zhao 1, 1 City University of Hong Kong, Hong Kong, 2 Noah’s Ark Lab, Huawei, Chi…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.14069v3.md` · `raw/arxiv/2505.14069v3.fulltext.md`
