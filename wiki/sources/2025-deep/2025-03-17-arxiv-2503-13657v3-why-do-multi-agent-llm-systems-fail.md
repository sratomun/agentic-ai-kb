---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Why Do Multi-Agent LLM Systems Fail?"
authors: Mert Cemri, Melissa Z. Pan, Shuyi Yang, Lakshya A. Agrawal et al.
url: https://arxiv.org/abs/2503.13657v3
date: 2025-03-17
citationCount: 402
influentialCitationCount: 71
velocity: 26.49
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Why Do Multi-Agent LLM Systems Fail?

**arXiv [2503.13657v3](https://arxiv.org/abs/2503.13657v3)** · 2025-03-17 · **402 citations** (71 influential · 26.49/mo) · Mert Cemri, Melissa Z. Pan, Shuyi Yang, Lakshya A. Agrawal et al.

**Significance:** The 'Why Do Multi-Agent LLM Systems Fail?' failure taxonomy — required reading before building MAS.

## Abstract
Despite enthusiasm for Multi-Agent LLM Systems (MAS), their performance gains on popular benchmarks are often minimal. This gap highlights a critical need for a principled understanding of why MAS fail. Addressing this question requires systematic identification and analysis of failure patterns. We introduce MAST-Data, a comprehensive dataset of 1600+ annotated traces collected across 7 popular MAS frameworks. MAST-Data is the first multi-agent system dataset to outline the failure dynamics in MAS for guiding the development of better future systems. To enable systematic classification of failures for MAST-Data, we build the first Multi-Agent System Failure Taxonomy (MAST). We develop MAST through rigorous analysis of 150 traces, guided closely by expert human annotators and validated by high inter-annotator agreement (kappa = 0.88). This process identifies 14 unique modes, clustered into 3 categories: (i) system design issues, (ii) inter-agent misalignment, and (iii) task verification. To enable scalable annotation, we develop an LLM-as-a-Judge pipeline with high agreement with human annotations. We leverage MAST and MAST-Data to analyze failure patterns across models (GPT4, Claude 3, Qwen2.5, CodeLlama) and tasks (coding, math, general agent), demonstrating improvement headrooms from better MAS design. Our analysis provides insights revealing that identified failures require more sophisticated solutions, highlighting a clear roadmap for future research. We publicly release our comprehensive dataset (MAST-Data), the MAST, and our LLM annotator to facilitate widespread research and development in MAS.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Challenges in Agentic Systems 2.2 Design Principles for Agentic Systems 2.3 Related Datasets and Taxonomy 3 The Multi-Agent Systems Dataset 3.1 Data Collection with Grounded Theory Analysis 3.2 Standardizing Failure Labels via Inter-Annotator Agreement 3.3 Enabling Scalable Annotation: The LLM-as-a-Judge Pipeline 3.4 Constructing the Multi-Agent Dataset 4 The Multi-Agent System Failure Taxonomy 5 Towards better Multi-Agent LLM Systems 5.1 Failure Breakdown in MAST-Data 5.2 MAST as a Practical Development Tool 5.3 Beyond Model Capabilities: The Primacy of System Design 6 Conclusion A MAST Failure Categories: Deep Dive A.1 FC1. System Design Issues A.2 FC2. Inter-Agent Misalignment A.3 FC3. Task Verification B Details of Multi-Agent Systems Evaluated B.1 Overview of MAS B.2 Multi-Agent Systems in the Initial Annotation Phase B.3 Closed-Source MAS C MAST Python Library D ProgramDev and ProgramDev-v2 Datasets E MAS Failure Modes Correlation F Understanding Failures: The Impact of Di…

**Method / approach.** Methodological workflow for constructing the MAST-Data dataset, involving the empirical identification of failure modes, the development of MAST , iterative refinement through inter-annotator agreement studies ( κ = 0.88 \kappa=0.88{} ), and the creation of a scalable LLM annotation pipeline. This figure highlights our systematic approach to creating a comprehensive dataset for studying MAS failures. To facilitate a principled understanding of why MAS fail and to guide the development of more reliable future systems, we introduce MAST-Data , the Multi-Agent System Failure Dataset. MAST-Data is a comprehensive, empirically grounded dataset comprising 1642 annotated execution traces collected from 7 popular MAS frameworks, covering domains of coding, math, and generic tasks. Constructing such a dataset, however, presents distinct challenges. First, unlike in traditional software where failures often have clearly identifiable root causes, failures in MAS are frequently complex. The…

**Results.** experimental validation. bioRxiv , 2024. doi: 10.1101/2024.11.11.623004 . URL https://www.biorxiv.org/content/early/2024/11/12/2024.11.11.623004 . Park et al. [2023a] Joon Sung Park, Joseph C. O’Brien, Carrie J. Cai, Meredith Ringel Morris, Percy Liang, and Michael S. Bernstein. Generative agents: Interactive simulacra of human behavior, 2023a. URL https://arxiv.org/abs/2304.03442 . Liang et al. [2025] Xinbin Liang, Jinyu Xiang, Zhaoyang Yu, Jiayi Zhang, and Sirui Hong. Openmanus: An open-source framework for building general ai agents. https://github.com/mannaandpoem/OpenManus , 2025. Fourney et al. [2024] Adam Fourney, Gagan Bansal, Hussein Mozannar, Cheng Tan, Eduardo Salinas, Friederike Niedtner, Grace Proebsting, Griffin Bassman, Jack Gerrits, Jacob Alber, et al. Magentic-one: A generalist multi-agent system for solving complex tasks. arXiv preprint arXiv:2411.04468 , 2024. He et al. [2024a] Ju…

**Conclusion.** Conclusion A MAST Failure Categories: Deep Dive A.1 FC1. System Design Issues A.2 FC2. Inter-Agent Misalignment A.3 FC3. Task Verification B Details of Multi-Agent Systems Evaluated B.1 Overview of MAS B.2 Multi-Agent Systems in the Initial Annotation Phase B.3 Closed-Source MAS C MAST Python Library D ProgramDev and ProgramDev-v2 Datasets E MAS Failure Modes Correlation F Understanding Failures: The Impact of Different LLMs and Agent Architectures G Approaches and strategies to improve MASs G.1 Tactical Approaches G.2 Structural Strategies H Intervention Case Studies H.1 Case Study 1: AG2 - MathChat H.2 Case Study 2: ChatDev H.3 Effect of the interventions on MAST I Analysis on Multi-…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]] · [[claude]]
- **Raw:** `raw/arxiv/2503.13657v3.md` · `raw/arxiv/2503.13657v3.fulltext.md`
