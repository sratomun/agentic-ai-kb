---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebWalker: Benchmarking LLMs in Web Traversal"
authors: Jialong Wu, Wenbiao Yin, Yong Jiang, Zhenglin Wang et al.
url: https://arxiv.org/abs/2501.07572v3
date: 2025-01-13
citationCount: 146
influentialCitationCount: 16
velocity: 8.47
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# WebWalker: Benchmarking LLMs in Web Traversal

**arXiv [2501.07572v3](https://arxiv.org/abs/2501.07572v3)** · 2025-01-13 · **146 citations** (16 influential · 8.47/mo) · Jialong Wu, Wenbiao Yin, Yong Jiang, Zhenglin Wang et al.

## Abstract
Retrieval-augmented generation (RAG) demonstrates remarkable performance across tasks in open-domain question-answering. However, traditional search engines may retrieve shallow content, limiting the ability of LLMs to handle complex, multi-layered information. To address it, we introduce WebWalkerQA, a benchmark designed to assess the ability of LLMs to perform web traversal. It evaluates the capacity of LLMs to traverse a website's subpages to extract high-quality data systematically. We propose WebWalker, which is a multi-agent framework that mimics human-like web navigation through an explore-critic paradigm. Extensive experimental results show that WebWalkerQA is challenging and demonstrates the effectiveness of RAG combined with WebWalker, through the horizontal and vertical integration in real-world scenarios.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large Language Models (LLMs) have demonstrated impressive capabilities across a wide range of natural language processing tasks (Ouyang et al., 2022; OpenAI, 2022a). While their knowledge base remains static post-training, integrating external search engines via retrieval-augmented generation (RAG) allows LLMs to retrieve up-to-date information from the web, enhancing their utility in dynamic, knowledgeintensive scenarios (Lewis et al., 2020). However, traditional online search engines, e.g., Google or Bing, perform horizontal searches of queries and may not effectively trace the deeper content embedded within websites. Interacting with the web pages and digging through them can effectively address this issue. Previous works related to web pages focus on addressing action-based requests, such as Mind2Web (Deng et al., 2023) and WebArena (Zhou et al., 2024a); these HTML-based instruction-action benchmarks face challenges such as excessively noisy information and overly long inputs, which can significantly hinder performance due to limitations in long-context understandin…

**Method / approach.** method with LLM and human participation, we obtain 680 questionanswer pairs for WebWalkerQA. The annotated case is shown in Figure 8. We will provide comprehensive statistics on WebWalkerQA, categorized by type, domain, and language. Type WebWalkerQA contains two types of data: multi-source and single-source QAs. SingleSingle-source QAs Multi-source QAs source QAs are labeled as single_sourcei , where i ∈ [2, 4], denoting the depth of the corresponding subEasy Medium Hard Easy Medium Hard page. Similarly, Multi-source QAs are labeled as 80 140 120 80 140 120 multi_sourcei , where i ∈ [2, 8], representing the sum of the depths of the two associated subpages2 . In Table 2: Dataset statistics on data difficulty level. other words, answering this query requires reading both pages simultaneously. Difficulty Level We categorize the questions into three difficulty levels: easy, medium, and hard, based on the value of i. Specifically, single_source2 , single_source3 , and single_source4 corre…

**Results.** experimental results show that WebWalkerQA is challenging and demonstrates the effectiveness of RAG combined with WebWalker, through the horizontal and vertical integration in real-world scenarios. 1 Introduction Large Language Models (LLMs) have demonstrated impressive capabilities across a wide range of natural language processing tasks (Ouyang et al., 2022; OpenAI, 2022a). While their knowledge base remains static post-training, integrating external search engines via retrieval-augmented generation (RAG) allows LLMs to retrieve up-to-date information from the web, enhancing their utility in dynamic, knowledgeintensive scenarios (Lewis et al., 2020). However, traditional online search engines, e.g., Google or Bing, perform horizontal searches of queries and may not effectively trace the deeper content embedded within websites. Interacting with the web pages and digging through them can effectively address this issue. Previous works…

**Conclusion.** Conclusion We introduce WebWalkerQA, a benchmark for evaluating LLMs’ web traversal abilities in complex, multistep information-seeking tasks. We also proposed WebWalker, a multi-agent framework that mimics human-like web navigation, combining exploration and critique. Experiments show that WebWalkerQA effectively challenges RAG systems, and combining RAG with WebWalker improves web navigation performance. Our work highlights the importance of deep, vertical exploration in web-based tasks, paving the way for more scalable and reliable LLM-based information retrieval integrated with RAG. 10 References Tamer Abuelsaad, Deepak Akkil, Prasenjit Dey, Ashish Jagmohan, Aditya Vempaty, and Ravi Kokku. Agent-e: From autonomous web navigation to…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2501.07572v3.md` · `raw/arxiv/2501.07572v3.fulltext.md`
