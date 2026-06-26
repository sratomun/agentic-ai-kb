---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Comprehensive Survey in LLM(-Agent) Full Stack Safety: Data, Training and Deployment"
authors: Kun Wang, Guibin Zhang, Zhenhong Zhou, Jiahao Wu et al.
url: https://arxiv.org/abs/2504.15585v4
date: 2025-04-22
citationCount: 126
influentialCitationCount: 4
velocity: 9.0
ingested: 2026-06-22
tags: [agent-reliability, agent-security, agentic-ai, arxiv, 2025, cited]
---

# A Comprehensive Survey in LLM(-Agent) Full Stack Safety: Data, Training and Deployment

**arXiv [2504.15585v4](https://arxiv.org/abs/2504.15585v4)** · 2025-04-22 · **126 citations** (4 influential · 9.0/mo) · Kun Wang, Guibin Zhang, Zhenhong Zhou, Jiahao Wu et al.

## Abstract
The remarkable success of Large Language Models (LLMs) has illuminated a promising pathway toward achieving Artificial General Intelligence for both academic and industrial communities, owing to their unprecedented performance across various applications. As LLMs continue to gain prominence in both research and commercial domains, their security and safety implications have become a growing concern, not only for researchers and corporations but also for every nation. Currently, existing surveys on LLM safety primarily focus on specific stages of the LLM lifecycle, e.g., deployment phase or fine-tuning phase, lacking a comprehensive understanding of the entire "lifechain" of LLMs. To address this gap, this paper introduces, for the first time, the concept of "full-stack" safety to systematically consider safety issues throughout the entire process of LLM training, deployment, and eventual commercialization. Compared to the off-the-shelf LLM safety surveys, our work demonstrates several distinctive advantages: (I) Comprehensive Perspective. We define the complete LLM lifecycle as encompassing data preparation, pre-training, post-training, deployment and final commercialization. To our knowledge, this represents the first safety survey to encompass the entire lifecycle of LLMs. (II) Extensive Literature Support. Our research is grounded in an exhaustive review of over 800+ papers, ensuring comprehensive coverage and systematic organization of security issues within a more holistic understanding. (III) Unique Insights. Through systematic literature analysis, we have developed reliable roadmaps and perspectives for each chapter. Our work identifies promising research directions, including safety in data generation, alignment techniques, model editing, and LLM-based agent systems. These insights provide valuable guidance for researchers pursuing future work in this field.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Data Safety 2.1 Pretraining Data Safety 2.2 Fine-tuning Data Safety 2.3 Alignment Data Safety 2.4 Safety in Data Generation 2.5 Roadmap Perspective 2.5.1 Reliable Data Distillation 2.5.2 Novel Data Generation Paradigms 2.5.3 Advanced Data Poisoning Depoisoning 3 Pre-training Safety 3.1 Data Filtering for Pretrain Safety 3.1.1 Heuristic based Filtering 3.1.2 Model based Filtering 3.1.3 Blackbox Filtering 3.2 Augmenting Training Data for Pre-training Safety 3.3 Roadmap Perspective 4 Post-training Safety 4.1 Attacks in Post-training 4.1.1 Toxic Data Construction Phase 4.1.2 Fine-tuning Phase 4.2 Defenses in Post-training 4.2.1 Alignment 4.2.2 Downstream Fine-tuning 4.2.3 Safety Recovery 4.2.4 Safety Location 4.2.5 Open-Weight LLMs Safeguard 4.3 Evaluation 4.3.1 Evaluation Metrics 4.3.2 Evaluation Benchmarks 4.4 Roadmap Perspective 4.4.1 From Low-Level to High-Level Safety Deceptive Alignment Reward Hacking 4.4.2 Provably Safe AI System 4.4.3 Beyond Fine-tuning, Systematic Saf…

**Method / approach.** methods to efficiently update the model’s knowledge or parameters, thus effectively ensuring the model’s usability during deployment. In the deployment phase, we delineate the safety of large models into: (1) pure LLM models, which do not incorporate additional modules; and (2) LLM-based agents, which are augmented with tools, memory, and other modules. This framework encompasses the entire cycle of model parameter training, convergence, and solidification. How to provide a clearer taxonomy and literature review? Contribution 2. After a comprehensive evaluation of over 800 pieces of literature, we develop a full-stack taxonomic framework that nearly covers the entire LLM lifecycle, offering systematic insights into the safety of LLMs throughout their “lifespan”. We provide a more reliable correlation analysis between each phase of the LLM timeline and other relevant sections, aiding readers in understanding the safety issues of LLMs while also clarifying the research stage of ea…

**Results.** Evaluation 4.3.1 Evaluation Metrics 4.3.2 Evaluation Benchmarks 4.4 Roadmap Perspective 4.4.1 From Low-Level to High-Level Safety Deceptive Alignment Reward Hacking 4.4.2 Provably Safe AI System 4.4.3 Beyond Fine-tuning, Systematic Safety 5 Safety in Model Editing Unlearning 5.1 Safety in Model Editing 5.2 Safety in Unlearning 5.3 Roadmap Perspective 5.3.1 Model Editing 5.3.2 Unlearning 6 LLM(-Agent) Deployment Safety 6.1 Deployment Safety 6.1.1 Attack in Deployment 6.1.2 Defensive Mechanisms in Deployment 6.1.3 Evaluation and Benchmarks in Deployment 6.2 Single-agent Safety 6.2.1 Definition of Agent 6.2.2 Tool Safety 6.2.3 Memory Safety 6.2.4 Attack 6.2.5 Defense 6.2.6 Environment Safety 6.3 Multi-agent Safety 6.3.1 Attack 6.3.2 Defense 6.4 Agent Communication Safety 6.4.1 Attack 6.4.2 Defense 6.5 Agent Safety Evaluation 6.5.1 Attack-Speci…

**Conclusion.** Conclusion \useunder \ul A Comprehensive Survey in LLM(-Agent) Full Stack Safety: Data, Training and Deployment Kun Wang Kun Wang is with Nanyang Technological University ( wang.kun@ntu.edu.sg ), Guibin Zhang is with National University of Singapore ( guibinz@outlook.com ), Jiahao Wu is with The Hong Kong Polytechnic University ( jiahao.wu@connect.polyu.hk ), Zhenhong Zhou is with A*STAR ( ydyjyazzh@gmail.com ), Yang Liu is with Nanyang Technological University ( yangliu@ntu.edu.sg ). * denotes equal contribution and † † \dagger † denotes the corresponding authors. Nanyang Technological University Squirrel AI Learning Guibin Zhang National University of Singapore Zhenhong Zhou † † \dagger † A*STAR Jiahao Wu † †…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.15585v4.md` · `raw/arxiv/2504.15585v4.fulltext.md`
