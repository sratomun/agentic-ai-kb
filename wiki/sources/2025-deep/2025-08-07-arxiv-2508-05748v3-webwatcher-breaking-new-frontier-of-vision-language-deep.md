---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebWatcher: Breaking New Frontier of Vision-Language Deep Research Agent"
authors: Xinyu Geng, Peng Xia, Zhen Zhang, Xinyu Wang et al.
url: https://arxiv.org/abs/2508.05748v3
date: 2025-08-07
citationCount: 83
influentialCitationCount: 15
velocity: 7.92
ingested: 2026-06-22
tags: [computer-use-agents, science-agents, agentic-rl, agentic-rag, agent-evaluation, arxiv, 2025, cited]
---

# WebWatcher: Breaking New Frontier of Vision-Language Deep Research Agent

**arXiv [2508.05748v3](https://arxiv.org/abs/2508.05748v3)** · 2025-08-07 · **83 citations** (15 influential · 7.92/mo) · Xinyu Geng, Peng Xia, Zhen Zhang, Xinyu Wang et al.

## Abstract
Web agents such as Deep Research have demonstrated superhuman cognitive abilities, capable of solving highly challenging information-seeking problems. However, most research remains primarily text-centric, overlooking visual information in the real world. This makes multimodal Deep Research highly challenging, as such agents require much stronger reasoning abilities in perception, logic, knowledge, and the use of more sophisticated tools compared to text-based agents. To address this limitation, we introduce WebWatcher, a multi-modal Agent for Deep Research equipped with enhanced visual-language reasoning capabilities. It leverages high-quality synthetic multimodal trajectories for efficient cold start training, utilizes various tools for deep reasoning, and further enhances generalization through reinforcement learning. To better evaluate the capabilities of multimodal agents, we propose BrowseComp-VL, a benchmark with BrowseComp-style that requires complex information retrieval involving both visual and textual information. Experimental results show that WebWatcher significantly outperforms proprietary baseline, RAG workflow and open-source agents in four challenging VQA benchmarks, which paves the way for solving complex multimodal information-seeking tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction Deep research agents represents a new frontier in Artificial Intelligence (AI), where Large Language Models (LLMs) go beyond static prompts to plan multi-step tasks: issuing search queries, reading documents, browsing the web, and refining answers through iterative reasoning (OpenAI, 2025a; Google, 2024; Perplexity, 2025). Many open-source, text-only web agents for deep research (Li et al., 2025b;a; Wu et al., 2025a; Zheng et al., 2025) have demonstrated superhuman abilities to interact with intricate information environments, achieving remarkable performance on high-difficulty benchmarks such as BrowseComp (Wei et al., 2025a) and Humanity’s Last Exam (HLE) (Phan et al., 2025). However, most advances to date remain primarily text-centric, neglecting the rich visual information omnipresent in realworld scenarios. Many research-centric and everyday tasks such as interpreting scientific diagrams (Hu et al., 2024), analyzing graphics (Wang et al., 2024b), or navigating visually rich web interfaces (Hong et al., 2024), demand integrated vision-language reasoning (Dong et al.…

**Method / approach.** methodology, emphasizing high data quality, multi-step multimodal reasoning, and robust compatibility with web-based agent paradigms. 2.1 Data Overview Our dataset BrowseComp-VL is designed for advanced multi-modal reasoning agents operating in real-world web environments. Each example comprises a factual image, an associated question requiring cross-modal reasoning, and auxiliary metadata about the underlying entities and relations. As shown in Fig.3, BrowseComp-VL is organized into 5 major domains comprising 17 fine-grained subfields, which is detailed in Appendix B. The major domains include Entertainment, Humanities, Technology, Natural Science and Other. Additionally, we define two difficulty levels to encourage a spectrum of reasoning abilities: • Level 1: Questions require multi-hop reasoning but still reference explicit entities. While the answers can be obtained through iterative retrieval steps, the reasoning process remains nontrivial due to the need for integrating info…

**Results.** Experimental results show that WebWatcher significantly outperforms proprietary baseline, RAG workflow and open-source agents in four challenging VQA benchmarks, which paves the way for solving complex multimodal information-seeking tasks. Humanity's Last Exam(HLE)-VL BrowseComp-VL (BC-VL, Average) 13.6 9.8 9 9.2 30 25 20 15 10 5 0 8.6 6 4.3 3 W her atc ebW 32B GPT-4o 41.3 W her atc ebW 7 -VL- n2.5 Qwe 2B Clau .7 de-3 W LiveVQA 58.7 50 40 30 20 10 0 ash l .5-f ini2 Gem 35.7 32B 5-fl ni2. i Gem ash VL-7 2.5- n Qwe 34.0 2B 13.4 -4o GPT 32B GPT-4o .7 de-3 11.5 lash .5-f ini2 Gem 72B -VL- n2.5 Qwe 11.2 .7 de-3 Clau MMSearch 55.3 50 40 30 20 10 0 30.3 Clau her atc ebW 13.0 43.9 32.7 Pass@1 0 27.0 Pass@1 Pass@1 12 Pass@1 arXiv:2508.05748v3 [cs.IR] 1 Sep 2025 Abstract W her atc ebW 32B ash 5-fl ni2. i Gem 29.2 .7 de-3 Clau 2B VL-7 2.5- n Qwe 24.1 -4o GPT Fi…

**Conclusion.** Conclusion In this work, we explore the underdeveloped landscape of multimodal DeepResearch by designing a unified framework WebWatcher that combines complex vision-language reasoning and multi-tool interaction. We present BrowseComp-VL, a challenging dataset tailored for in-depth multimodal reasoning and strategic planning, and introduce a scalable pipeline to transform complex textual QA examples into VQA. To equip agents with robust tool-use capabilities, we further develop an automated trajectory generation pipeline grounded in action-observation traces, enabling high-quality supervision for cold start and GRPO. Finally, we enhance evaluation through a test-time scaling strategy. WebWatcher establishes a strong foundation for future mu…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[science-agents|Science agents]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2508.05748v3.md` · `raw/arxiv/2508.05748v3.fulltext.md`
