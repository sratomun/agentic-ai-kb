---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent Laboratory: Using LLM Agents as Research Assistants"
authors: Samuel Schmidgall, Yusheng Su, Ze Wang, Ximeng Sun et al.
url: https://arxiv.org/abs/2501.04227v2
date: 2025-01-08
citationCount: 370
influentialCitationCount: 22
velocity: 21.25
ingested: 2026-06-22
tags: [coding-agents, science-agents, agentic-ai, arxiv, 2025, cited]
---

# Agent Laboratory: Using LLM Agents as Research Assistants

**arXiv [2501.04227v2](https://arxiv.org/abs/2501.04227v2)** · 2025-01-08 · **370 citations** (22 influential · 21.25/mo) · Samuel Schmidgall, Yusheng Su, Ze Wang, Ximeng Sun et al.

## Abstract
Historically, scientific discovery has been a lengthy and costly process, demanding substantial time and resources from initial conception to final results. To accelerate scientific discovery, reduce research costs, and improve research quality, we introduce Agent Laboratory, an autonomous LLM-based framework capable of completing the entire research process. This framework accepts a human-provided research idea and progresses through three stages--literature review, experimentation, and report writing to produce comprehensive research outputs, including a code repository and a research report, while enabling users to provide feedback and guidance at each stage. We deploy Agent Laboratory with various state-of-the-art LLMs and invite multiple researchers to assess its quality by participating in a survey, providing human feedback to guide the research process, and then evaluate the final paper. We found that: (1) Agent Laboratory driven by o1-preview generates the best research outcomes; (2) The generated machine learning code is able to achieve state-of-the-art performance compared to existing methods; (3) Human involvement, providing feedback at each stage, significantly improves the overall quality of research; (4) Agent Laboratory significantly reduces research expenses, achieving an 84% decrease compared to previous autonomous research methods. We hope Agent Laboratory enables researchers to allocate more effort toward creative ideation rather than low-level coding and writing, ultimately accelerating scientific discovery.

## From the paper (full-text excerpts)
**Introduction.** Introduction Scientists frequently face constraints that limit the number of research ideas they can explore at any given time, resulting in ideas being prioritized based on predicted impact. While this process helps determine which concepts are worth investing time in and how best to allocate limited resources effectively, many high quality ideas remain unexplored. If the process of exploring ideas had less limitations, researchers would be able to investigate multiple concepts simultaneously, increasing the likelihood of scientific discovery. In an effort to achieve this, recent work has explored the capability of LLMs to perform research ideation and automated paper generation, where LLM agents perform the role of human scientists (Baek et al. (2024); Ghafarollahi & Buehler (2024b); Lu et al. (2024a); Swanson et al. (2024)). The work of Baek et al. (2024) introduces ResearchAgent, which automatically generates research ideas, methods, and experiment designs, iteratively refining them through feedback from multiple reviewing agents that mirror peer discussions and leverage human-al…

**Method / approach.** methods; (3) Human involvement, providing feedback at each stage, significantly improves the overall quality of research; (4) Agent Laboratory significantly reduces research expenses, achieving an 84% decrease compared to previous autonomous research methods. We hope Agent Laboratory enables researchers to allocate more effort toward creative ideation rather than low-level coding and writing, ultimately accelerating scientific discovery. § https://AgentLaboratory.github.io Figure 1 | Agent Laboratory takes as input a human research idea and a set of notes, provides this to a pipeline of specialized LLM-driven agents, and produces a research report and code repository. Corresponding author(s): Samuel Schmidgall (sschmi46@jhu.edu) Agent Laboratory: Using LLM Agents as Research Assistants 1. Introduction Scientists frequently face constraints that limit the number of research ideas they can explore at any given time, resulting in ideas being prioritized based on predicted impact. W…

**Results.** experimentation, and report writing to produce comprehensive research outputs, including a code repository and a research report, while enabling users to provide feedback and guidance at each stage. We deploy Agent Laboratory with various state-of-the-art LLMs and invite multiple researchers to assess its quality by participating in a survey, providing human feedback to guide the research process, and then evaluate the final paper. We found that: (1) Agent Laboratory driven by o1-preview generates the best research outcomes; (2) The generated machine learning code is able to achieve state-of-the-art performance compared to existing methods; (3) Human involvement, providing feedback at each stage, significantly improves the overall quality of research; (4) Agent Laboratory significantly reduces research expenses, achieving an 84% decrease compared to previous autonomous research methods. We hope Agent Laboratory enables researchers to al…

**Conclusion.** conclusions about the idea novelty (Ashkinaze et al. (2024); Liu et al. (2024); Padmakumar & He (2024)). These findings suggest that, with the current LLMs, the strongest research systems would combine human-guided ideation with LLM-based workflows. LLMs for autonomous research Recent advancements in automated scientific workflows have focused on leveraging LLMs to emulate the process of research. Swanson et al. (2024) introduces a team of LLM agents working as scientists alongside a human researcher who provides high-level feedback, with the end result being novel nanobody binders aimed at addressing recent variants of SARS-CoV-2. ChemCrow (M. Bran et al. (2024)) and Coscientist (Boiko et al. (2023)) demonstrate the ability for autonomous…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[science-agents|Science agents]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[agent-laboratory]]
- **Raw:** `raw/arxiv/2501.04227v2.md` · `raw/arxiv/2501.04227v2.fulltext.md`
