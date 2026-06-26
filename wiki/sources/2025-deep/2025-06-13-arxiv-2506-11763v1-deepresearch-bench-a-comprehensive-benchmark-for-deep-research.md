---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents"
authors: Mingxuan Du, Benfeng Xu, Chiwei Zhu, Xiaorui Wang et al.
url: https://arxiv.org/abs/2506.11763v1
date: 2025-06-13
citationCount: 168
influentialCitationCount: 49
velocity: 13.67
ingested: 2026-06-22
tags: [science-agents, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents

**arXiv [2506.11763v1](https://arxiv.org/abs/2506.11763v1)** · 2025-06-13 · **168 citations** (49 influential · 13.67/mo) · Mingxuan Du, Benfeng Xu, Chiwei Zhu, Xiaorui Wang et al.

## Abstract
Deep Research Agents are a prominent category of LLM-based agents. By autonomously orchestrating multistep web exploration, targeted retrieval, and higher-order synthesis, they transform vast amounts of online information into analyst-grade, citation-rich reports--compressing hours of manual desk research into minutes. However, a comprehensive benchmark for systematically evaluating the capabilities of these agents remains absent. To bridge this gap, we present DeepResearch Bench, a benchmark consisting of 100 PhD-level research tasks, each meticulously crafted by domain experts across 22 distinct fields. Evaluating DRAs is inherently complex and labor-intensive. We therefore propose two novel methodologies that achieve strong alignment with human judgment. The first is a reference-based method with adaptive criteria to assess the quality of generated research reports. The other framework is introduced to evaluate DRA's information retrieval and collection capabilities by assessing its effective citation count and overall citation accuracy. We have open-sourced DeepResearch Bench and key components of these frameworks at https://github.com/Ayanami0730/deep_research_bench to accelerate the development of practical LLM-based agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction We now enter a new phase of AI [35], a period marked by comprehensive advances in the capabilities of the large language model (LLM) [5, 20]. These advancements enable the construction of LLM-based Agent systems designed to tackle increasingly complex tasks [15, 8, 34]. In this evolving landscape, defining tasks that genuinely reflect real-world demands and designing robust evaluation methodologies to measure the progress of these Agent systems are becoming critically important. Deep research represents one such well-defined task domain, with Deep Research Agents (DRAs) [13, 37, 24] emerging as the most widely utilized LLM-based agents today. Users leverage these agents to enhance their productivity significantly. However, comprehensively evaluating the capabilities of these DRAs presents substantial challenges. Because their internal reasoning and information retrieval processes are not transparent, the final generated report becomes the primary interface through which their overall performance can be assessed. Moreover, evaluating the quality of these extensive resear…

**Method / approach.** methodologies that achieve strong alignment with human judgment. The first is a reference-based method with adaptive criteria to assess the quality of generated research reports. The other framework is introduced to evaluate DRA’s information retrieval and collection capabilities by assessing its effective citation count and overall citation accuracy. We have open-sourced DeepResearch Bench and key components of these frameworks at https://github.com/Ayanami0730/deep_research_bench to accelerate the development of practical LLMbased agents. Figure 1: Overview of agent performance on DeepResearch Bench. Left: Generated report quality scores across evaluation dimensions. Right: Agent citation accuracy and average number of effective citations. ∗ † Work done during the internship at Metastone. Corresponding author: Zhendong Mao. Preprint. Work in progress. 1 Introduction We now enter a new phase of AI [35], a period marked by comprehensive advances in the capabilities of the large…

**Results.** experiments suggest that scoring reports in isolation often yields insufficiently discriminative results; models tend to assign uniformly high scores, thereby masking genuine quality variations. To mitigate this, RACE adopts a reference-based scoring strategy. For each task t, a high-quality report Rref is selected as a reference. All generated criteria {cd,k } across all dimensions are aggregated into a comprehensive list Ct . The Judge LLM then analyzes the target report Rtgt and the reference report Rref against each criterion c ∈ Ct . This yields lists of scores for both reports for each criterion, which are then used for final score calculation: ({stgt,c }c∈Ct , {sref,c }c∈Ct ) = JudgeLLM(t, Rtgt , Rref , Ct ) (2) Overall Score Calculation. Finally, we compute the overall quality score of the target report. First, dimension-level scores Sd (R) are calculated by weighting criterion-level scores sR,cd,k with criterion weights wd,k…

**Conclusion.** Conclusion In this work, we introduce DeepResearch Bench, the first comprehensive benchmark for evaluating the report generation and web retrieval capabilities of Deep Research Agents. Comprising 100 high-quality research tasks across 22 distinct domains, this benchmark is meticulously curated to reflect authentic user needs. Our key evaluation frameworks, RACE and FACT, have demonstrated high consistency with human judgments, affirming their reliability. We hope DeepResearch Bench will guide developers and researchers in constructing more powerful and human-centric AI agent systems that truly address genuine user requirements. 9 References [1] Yushi Bai, Jiajie Zhang, Xin Lv, Linzhi Zheng, Siqi Zhu, Lei Hou, Yuxiao Dong, Jie Tang, and J…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2506.11763v1.md` · `raw/arxiv/2506.11763v1.fulltext.md`
