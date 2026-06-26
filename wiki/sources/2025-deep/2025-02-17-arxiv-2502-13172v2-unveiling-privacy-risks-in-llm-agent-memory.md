---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Unveiling Privacy Risks in LLM Agent Memory"
authors: Bo Wang, Weiyi He, Shenglai Zeng, Zhen Xiang et al.
url: https://arxiv.org/abs/2502.13172v2
date: 2025-02-17
citationCount: 85
influentialCitationCount: 5
velocity: 5.28
ingested: 2026-06-22
tags: [agent-security, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Unveiling Privacy Risks in LLM Agent Memory

**arXiv [2502.13172v2](https://arxiv.org/abs/2502.13172v2)** · 2025-02-17 · **85 citations** (5 influential · 5.28/mo) · Bo Wang, Weiyi He, Shenglai Zeng, Zhen Xiang et al.

## Abstract
Large Language Model (LLM) agents have become increasingly prevalent across various real-world applications. They enhance decision-making by storing private user-agent interactions in the memory module for demonstrations, introducing new privacy risks for LLM agents. In this work, we systematically investigate the vulnerability of LLM agents to our proposed Memory EXTRaction Attack (MEXTRA) under a black-box setting. To extract private information from memory, we propose an effective attacking prompt design and an automated prompt generation method based on different levels of knowledge about the LLM agent. Experiments on two representative agents demonstrate the effectiveness of MEXTRA. Moreover, we explore key factors influencing memory leakage from both the agent designer's and the attacker's perspectives. Our findings highlight the urgent need for effective memory safeguards in LLM agent design and deployment.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background and Threat Model 2.1 Agent Workflow 2.2 Threat model Attacker Objective. Attacker Capability. 3 Paradigm of Attack Design 3.1 Attacking Prompt Design 3.2 Automated Diverse Prompts Generation 4 RQ1: LLM Agent Memory Extraction 4.1 Experiments Setup Agent Setup. Metrics. Baseline. 4.2 Attacking Results The attacking prompt design and automated generation instruction are essential for revealing privacy risk. 5 RQ2: Impact of Memory Module Configuration 5.1 Memory Module Configuration 5.2 Results Analysis Scoring Function. Embedding Model. Memory Size. Retrieval Depth. Backbone. 6 RQ3: Impact of Prompting Strategies 6.1 Experiment Settings 6.2 Results Analysis The number of attacking prompts. Prompt generation instructions. 7 Related Work LLM Agent with Memory. Privacy Risk in RAG. Prompt Injection Attack. 8 Conclusion A Instructions for Prompts Generation A.1 Basic Instruction A.2 Advanced Instruction Advanced Instruction for Edit Distance. Ad…

**Method / approach.** method based on different levels of knowledge about the LLM agent. Experiments on two representative agents demonstrate the effectiveness of MEXTRA. Moreover, we explore key factors influencing memory leakage from both the agent designer’s and the attacker’s perspectives. Our findings highlight the urgent need for effective memory safeguards in LLM agent design and deployment. 1 Introduction Large Language Models (LLMs) have demonstrated revolutionary capabilities in language understanding, reasoning, and generation (OpenAI, 2023 ; Zhao et al., 2023 ) . Building on these advances, LLM agents use LLMs and supplement with additional functionalities to perform more complex tasks (Xi et al., 2023 ) . Its typical pipeline consists of the following key steps: taking user instruction, gathering environment information, retrieving relevant knowledge and past experiences, giving an action solution based on the above information, and finally executing the solution Wang et al. ( 2024a )…

**Results.** Experiments Setup Agent Setup. Metrics. Baseline. 4.2 Attacking Results The attacking prompt design and automated generation instruction are essential for revealing privacy risk. 5 RQ2: Impact of Memory Module Configuration 5.1 Memory Module Configuration 5.2 Results Analysis Scoring Function. Embedding Model. Memory Size. Retrieval Depth. Backbone. 6 RQ3: Impact of Prompting Strategies 6.1 Experiment Settings 6.2 Results Analysis The number of attacking prompts. Prompt generation instructions. 7 Related Work LLM Agent with Memory. Privacy Risk in RAG. Prompt Injection Attack. 8 Conclusion A Instructions for Prompts Generation A.1 Basic Instruction A.2 Advanced Instruction Advanced Instruction for Edit Distance. Advanced Instruction for Cosine Similarity. A.3 Instructions for Baselines B More Details about Experiments B.1 Experiment Setup…

**Conclusion.** Conclusion A Instructions for Prompts Generation A.1 Basic Instruction A.2 Advanced Instruction Advanced Instruction for Edit Distance. Advanced Instruction for Cosine Similarity. A.3 Instructions for Baselines B More Details about Experiments B.1 Experiment Setup Agent Setup. Memory Setup. Embedding Model Setup. Attacks Setting. B.2 More Experiments Case study. Overlap Analysis. Experiments on QA-Agent C Discussion about Potential Mitigation Unveiling Privacy Risks in LLM Agent Memory Bo Wang 1 , Weiyi He 1 , Shenglai Zeng 1 , Zhen Xiang 2 , Yue Xing 1 , Jiliang Tang 1 , Pengfei He 1 🖂 1 Michigan State University, 2 University of Georgia {wangbo9,heweiyi,zengshe1,xingyue1,tangjil…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.13172v2.md` · `raw/arxiv/2502.13172v2.fulltext.md`
