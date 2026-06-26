---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies"
authors: Han Zhou, Xingchen Wan, Ruoxi Sun, Hamid Palangi et al.
url: https://arxiv.org/abs/2502.02533v2
date: 2025-02-04
citationCount: 92
influentialCitationCount: 7
velocity: 5.57
ingested: 2026-06-22
tags: [multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies

**arXiv [2502.02533v2](https://arxiv.org/abs/2502.02533v2)** · 2025-02-04 · **92 citations** (7 influential · 5.57/mo) · Han Zhou, Xingchen Wan, Ruoxi Sun, Hamid Palangi et al.

## Abstract
Large language models, employed as multiple agents that interact and collaborate with each other, have excelled at solving complex tasks. The agents are programmed with prompts that declare their functionality, along with the topologies that orchestrate interactions across agents. Designing prompts and topologies for multi-agent systems (MAS) is inherently complex. To automate the entire design process, we first conduct an in-depth analysis of the design space aiming to understand the factors behind building effective MAS. We reveal that prompts together with topologies play critical roles in enabling more effective MAS design. Based on the insights, we propose Multi-Agent System Search (MASS), a MAS optimization framework that efficiently exploits the complex MAS design space by interleaving its optimization stages, from local to global, from prompts to topologies, over three stages: 1) block-level (local) prompt optimization; 2) workflow topology optimization; 3) workflow-level (global) prompt optimization, where each stage is conditioned on the iteratively optimized prompts/topologies from former stages. We show that MASS-optimized multi-agent systems outperform a spectrum of existing alternatives by a substantial margin. Based on the MASS-found systems, we finally propose design principles behind building effective multi-agent systems.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Designing Multi-Agent Systems 2.1 Block-level Analysis: Prompt Design for Agents 2.2 Workflow-level Search Space Design 3 Mass : Multi-Agent System Search 4 Experiments 5 Related Work 6 Conclusion A Limitations and future work B Implementation details B.1 Datasets B.2 Baselines B.3 Mass details and Construction Rules C Additional experiments C.1 Generalization across LLM backbones C.2 Discussion on Mass -found topologies C.3 Cost analysis C.4 Graph optimization baseline C.5 Ablation on prompt optimizers D Prompt template E Best Prompts Discovered \pdftrailerid redacted \correspondingauthor {hzhouml, soarik}@google.com. Work done while Han Zhou was a Student Researcher at Google. Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies Han Zhou Xingchen Wan Google Ruoxi Sun Google Hamid Palangi Google Shariq Iqbal Google Ivan Vulić Anna Korhonen University of Cambridge Sercan Ö. Arık Google Abstract Large language models, employed as multiple agents that…

**Method / approach.** methods —such as discovering the most efficient and effective way to identify the optimal configuration—there has been less focus on the design of search spaces , which determines the perimeter and the scope of any search algorithm. This imbalance draws a parallel to the historical development of neural architecture search (NAS) (White et al., 2023 ) . Initially, the field concentrated on sophisticated search methods, such as Bayesian optimization (Kandasamy et al., 2018 ; Ru et al., 2021 ) and differentiable search (Liu et al., 2018 ) . Follow-up works have highlighted the often-overlooked importance of search space design, arguing that it can be equally, if not more, critical (Wan et al., 2022 ; Zhou et al., 2023a ) . Inspired by this insight, we hypothesize that manually crafted topologies might be sub-optimal, and automatic topology optimization (potentially framed as a rigorous optimization problem) can play a similarly pivotal role via judiciously designing search space for M…

**Results.** Experiments 5 Related Work 6 Conclusion A Limitations and future work B Implementation details B.1 Datasets B.2 Baselines B.3 Mass details and Construction Rules C Additional experiments C.1 Generalization across LLM backbones C.2 Discussion on Mass -found topologies C.3 Cost analysis C.4 Graph optimization baseline C.5 Ablation on prompt optimizers D Prompt template E Best Prompts Discovered \pdftrailerid redacted \correspondingauthor {hzhouml, soarik}@google.com. Work done while Han Zhou was a Student Researcher at Google. Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies Han Zhou Xingchen Wan Google Ruoxi Sun Google Hamid Palangi Google Shariq Iqbal Google Ivan Vulić Anna Korhonen University of Cambridge Sercan Ö. Arık Google Abstract Large language models, employed as multiple agents that interact and collaborate with each ot…

**Conclusion.** Conclusion A Limitations and future work B Implementation details B.1 Datasets B.2 Baselines B.3 Mass details and Construction Rules C Additional experiments C.1 Generalization across LLM backbones C.2 Discussion on Mass -found topologies C.3 Cost analysis C.4 Graph optimization baseline C.5 Ablation on prompt optimizers D Prompt template E Best Prompts Discovered \pdftrailerid redacted \correspondingauthor {hzhouml, soarik}@google.com. Work done while Han Zhou was a Student Researcher at Google. Multi-Agent Design: Optimizing Agents with Better Prompts and Topologies Han Zhou Xingchen Wan Google Ruoxi Sun Google Hamid Palangi Google Shariq Iqbal Google Ivan Vulić Anna Ko…

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.02533v2.md` · `raw/arxiv/2502.02533v2.fulltext.md`
