---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "APIGen-MT: Agentic Pipeline for Multi-Turn Data Generation via Simulated Agent-Human Interplay"
authors: Akshara Prabhakar, Zuxin Liu, Ming Zhu, Jianguo Zhang et al.
url: https://arxiv.org/abs/2504.03601v4
date: 2025-04-04
citationCount: 130
influentialCitationCount: 20
velocity: 8.91
ingested: 2026-06-22
tags: [human-agent-interaction, agent-reliability, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# APIGen-MT: Agentic Pipeline for Multi-Turn Data Generation via Simulated Agent-Human Interplay

**arXiv [2504.03601v4](https://arxiv.org/abs/2504.03601v4)** · 2025-04-04 · **130 citations** (20 influential · 8.91/mo) · Akshara Prabhakar, Zuxin Liu, Ming Zhu, Jianguo Zhang et al.

## Abstract
Training effective AI agents for multi-turn interactions requires high-quality data that captures realistic human-agent dynamics, yet such data is scarce and expensive to collect manually. We introduce APIGen-MT, a two-phase framework that generates verifiable and diverse multi-turn agent data. In the first phase, our agentic pipeline produces detailed task blueprints with ground-truth actions, leveraging a committee of LLM reviewers and iterative feedback loops. These blueprints are then transformed into complete interaction trajectories through simulated human-agent interplay. We train a family of models -- the xLAM-2-fc-r series with sizes ranging from 1B to 70B parameters. Our models outperform frontier models such as GPT-4o and Claude 3.5 on $τ$-bench and BFCL benchmarks, with the smaller models surpassing their larger counterparts, particularly in multi-turn settings, while maintaining superior consistency across multiple trials. Comprehensive experiments demonstrate that our verified blueprint-to-details approach yields high-quality training data, enabling the development of more reliable, efficient, and capable agents. We open-source 5K synthetic data trajectories and the trained xLAM-2-fc-r models to advance research in AI agents. Models at https://huggingface.co/collections/Salesforce/xlam-2-67ef5be12949d8dcdae354c4; Dataset at https://huggingface.co/datasets/Salesforce/APIGen-MT-5k and Website at https://apigen-mt.github.io

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 APIGen-MT Method for Synthesizing High-Quality Multi-Turn Data 3.1 Multi-Turn Interaction Problem Formulation 3.2 APIGen-MT Framework Overview 3.2.1 Phase 1: Task Configuration and Groundtruth Generation 3.2.2 Phase 2: Human-Agent-Environment Interaction Trajectory Collection 4 A Case Study of APIGen-MT on τ 𝜏 \tau italic_τ -bench 4.1 Phase 1 Implementation: Task Configuration Generation and Validation 4.1.1 API Dependency Graph and Context Samplers API Graph Modeling. Specialized Context Samplers. 4.1.2 Multi-Stage Validation for τ 𝜏 \tau italic_τ -bench Stage 1: Action Validation. Stage 2: Alignment Validation. Stage 3: Final Semantic Review Refinement. 4.1.3 Reverse Task Recombination for Complex Task Construction 4.2 Phase 2: Simulated Human-Agent Interplay and Trajectory Collection 4.3 Data Collection Statistics 5 Experiments 5.1 Experimental Setup 5.2 Experiment Results BFCL v3 Results. 𝝉 𝝉 \boldsymbol{\tau} bold_italic_τ -bench Results. 5.3 Consistency Stability Experiment…

**Method / approach.** methods for knowledge distillation in agent training. However, these approaches primarily focus on single-turn interactions, failing to capture the complexity of real-world agent usage, where multiple turns are often required. Other efforts like [ 51 , 50 , 11 ] , while incorporating multi-turn aspects, lack human-agent interplay–crucial for realistic data generation. The verification and synthesis of high-quality multi-turn trajectories containing both linguistic diversity and grounded actions remains largely unsolved, creating a significant barrier to advancing agent capabilities. To address these limitations, we introduce APIGen-MT , an agentic data synthesis pipeline for generating high-quality multi-turn agent data. It operates in two main steps: first, a data agent generates a detailed and verified task "blueprint", and second, this blueprint guides the generation of realistic multi-turn interactions through simulated agent-human interplay ( Subsection 4.2 ). The blueprint ge…

**Results.** Experiments 5.1 Experimental Setup 5.2 Experiment Results BFCL v3 Results. 𝝉 𝝉 \boldsymbol{\tau} bold_italic_τ -bench Results. 5.3 Consistency Stability Experiments 5.4 In-Depth Analysis of Model Behavior 6 Discussion A Benchmarks Description B Prompts APIGen-MT : A gentic PI peline for M ulti- T urn Data Gen eration via Simulated Agent-Human Interplay Akshara Prabhakar Zuxin Liu 1 1 footnotemark: 1 Ming Zhu Jianguo Zhang 2 2 footnotemark: 2 Tulika Awalgaonkar 2 2 footnotemark: 2 Shiyu Wang Zhiwei Liu Haolin Chen Thai Hoang Juan Carlos Niebles Shelby Heinecke 3 3 footnotemark: 3 Weiran Yao 3 3 footnotemark: 3 Huan Wang 3 3 footnotemark: 3 Silvio Savarese 3 3 footnotemark: 3 Caiming Xiong 3 3 footnotemark: 3 Salesforce AI Research Co-first Authors Core Contributors Corresponding Authors Abstract Training effective AI agents for multi-turn interactions requires high-qu…

**Conclusion.** Discussion A Benchmarks Description B Prompts APIGen-MT : A gentic PI peline for M ulti- T urn Data Gen eration via Simulated Agent-Human Interplay Akshara Prabhakar Zuxin Liu 1 1 footnotemark: 1 Ming Zhu Jianguo Zhang 2 2 footnotemark: 2 Tulika Awalgaonkar 2 2 footnotemark: 2 Shiyu Wang Zhiwei Liu Haolin Chen Thai Hoang Juan Carlos Niebles Shelby Heinecke 3 3 footnotemark: 3 Weiran Yao 3 3 footnotemark: 3 Huan Wang 3 3 footnotemark: 3 Silvio Savarese 3 3 footnotemark: 3 Caiming Xiong 3 3 footnotemark: 3 Salesforce AI Research Co-first Authors Core Contributors Corresponding Authors Abstract Training effective AI agents for multi-turn interactions requires high-quality data that captures real…

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[bfcl]] · [[claude]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2504.03601v4.md` · `raw/arxiv/2504.03601v4.fulltext.md`
