---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments"
authors: Yuxiang Zheng, Dayuan Fu, Xiangkun Hu, Xiaojie Cai et al.
url: https://arxiv.org/abs/2504.03160v4
date: 2025-04-04
citationCount: 220
influentialCitationCount: 14
velocity: 15.08
ingested: 2026-06-22
tags: [computer-use-agents, science-agents, agentic-rl, agentic-rag, multi-agent-systems, arxiv, 2025, cited]
---

# DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments

**arXiv [2504.03160v4](https://arxiv.org/abs/2504.03160v4)** · 2025-04-04 · **220 citations** (14 influential · 15.08/mo) · Yuxiang Zheng, Dayuan Fu, Xiangkun Hu, Xiaojie Cai et al.

## Abstract
Large Language Models (LLMs) equipped with web search capabilities have demonstrated impressive potential for deep research tasks. However, current approaches predominantly rely on either manually engineered prompts (prompt engineering-based) with brittle performance or reinforcement learning within controlled Retrieval-Augmented Generation (RAG) environments (RAG-based) that fail to capture the complexities of real-world interaction. In this paper, we introduce DeepResearcher, the first comprehensive framework for end-to-end training of LLM-based deep research agents through scaling reinforcement learning (RL) in real-world environments with authentic web search interactions. Unlike RAG-based approaches that assume all necessary information exists within a fixed corpus, our method trains agents to navigate the noisy, unstructured, and dynamic nature of the open web. We implement a specialized multi-agent architecture where browsing agents extract relevant information from various webpage structures and overcoming significant technical challenges. Extensive experiments on open-domain research tasks demonstrate that DeepResearcher achieves substantial improvements of up to 28.9 points over prompt engineering-based baselines and up to 7.2 points over RAG-based RL agents. Our qualitative analysis reveals emergent cognitive behaviors from end-to-end RL training, including the ability to formulate plans, cross-validate information from multiple sources, engage in self-reflection to redirect research, and maintain honesty when unable to find definitive answers. Our results highlight that end-to-end training in real-world web environments is not merely an implementation detail but a fundamental requirement for developing robust research capabilities aligned with real-world applications. We release DeepResearcher at https://github.com/GAIR-NLP/DeepResearcher.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Prompt-Based Search Agents 2.2 Training-Based Search Agents Supervised Fine-Tuning (SFT) Reinforcement Learning (RL) 2.3 Training Environments Local RAG Environments Real-World Web Search Environments 3 Methodology 3.1 Deep Research Trajectory Reasoning Web Search Tool Web Browsing Agent Answering 3.2 Addressing Challenges in Dynamic Real-World Web Environments Challenge I: High-concurrency requests at a single moment Challenge II: Managing Web Crawling and API Limitations Challenge III: Optimizing Information Extraction via a Multi-Agent Approach 3.3 RL Training Framework GRPO Masking Observations 3.4 Reward 4 Beyond Memorization: Curating Search-Dependent Training Data 4.1 Leveraging Open Domain QA Data 4.2 The Issue of Data Contamination 4.3 Data Cleaning and Contamination Detection Low-Quality Question Filtering Contamination Detection 5 Experiments 5.1 Experimental Setups 5.1.1 Model and Hyperparameters 5.2 Evaluation and Results 5.2.1 Benchmarks…

**Method / approach.** Methodology 3.1 Deep Research Trajectory Reasoning Web Search Tool Web Browsing Agent Answering 3.2 Addressing Challenges in Dynamic Real-World Web Environments Challenge I: High-concurrency requests at a single moment Challenge II: Managing Web Crawling and API Limitations Challenge III: Optimizing Information Extraction via a Multi-Agent Approach 3.3 RL Training Framework GRPO Masking Observations 3.4 Reward 4 Beyond Memorization: Curating Search-Dependent Training Data 4.1 Leveraging Open Domain QA Data 4.2 The Issue of Data Contamination 4.3 Data Cleaning and Contamination Detection Low-Quality Question Filtering Contamination Detection 5 Experiments 5.1 Experimental Setups 5.1.1 Model and Hyperparameters 5.2 Evaluation and Results 5.2.1 Benchmarks 5.2.2 Baselines 5.2.3 Evaluation Metrics Rule-based Metrics Model-based Evaluation 5.2.4 Main Results DeepResearcher outperforms the baselines wi…

**Results.** Experiments 5.1 Experimental Setups 5.1.1 Model and Hyperparameters 5.2 Evaluation and Results 5.2.1 Benchmarks 5.2.2 Baselines 5.2.3 Evaluation Metrics Rule-based Metrics Model-based Evaluation 5.2.4 Main Results DeepResearcher outperforms the baselines within training domains. DeepResearcher demonstrates exceptional generalization to novel domains. Importance of Real-World Environment in Training 6 Analysis 6.1 Training Dynamics 6.2 Case Study 7 Conclusion A Prompts A.1 Prompt for Question Quality Level Evaluation A.2 Prompt for Model’s Answer Quality Level Evaluation A.3 Prompt for Research Plan on Question Answering B Training Scaling Result \mdfdefinestyle mystylerightline=true, innerleftmargin=10, innerrightmargin=10, outerlinewidth=3pt, topline=false, rightline=true, bottomline=false, skipabove=skipbelow= showstringspaces = false, keywords = false,true, alsolet…

**Conclusion.** Conclusion A Prompts A.1 Prompt for Question Quality Level Evaluation A.2 Prompt for Model’s Answer Quality Level Evaluation A.3 Prompt for Research Plan on Question Answering B Training Scaling Result \mdfdefinestyle mystylerightline=true, innerleftmargin=10, innerrightmargin=10, outerlinewidth=3pt, topline=false, rightline=true, bottomline=false, skipabove=skipbelow= showstringspaces = false, keywords = false,true, alsoletter = 0123456789., morestring = [s]””, stringstyle = , MoreSelectCharTable = \lst@DefSaveDef ‘: \colon@json \processColon@json , basicstyle = , keywordstyle = , DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments Yuxiang Zheng 1,2,3 Dayuan Fu 2,3∗ Xian…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[science-agents|Science agents]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Raw:** `raw/arxiv/2504.03160v4.md` · `raw/arxiv/2504.03160v4.fulltext.md`
