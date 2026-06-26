---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SciToolAgent: A Knowledge Graph-Driven Scientific Agent for Multi-Tool Integration"
authors: Keyan Ding, Jing Yu, Junjie Huang, Yuchen Yang et al.
url: https://arxiv.org/abs/2507.20280v1
date: 2025-07-27
citationCount: 56
influentialCitationCount: 3
velocity: 5.17
ingested: 2026-06-22
tags: [knowledge-graph, agent-security, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# SciToolAgent: A Knowledge Graph-Driven Scientific Agent for Multi-Tool Integration

**arXiv [2507.20280v1](https://arxiv.org/abs/2507.20280v1)** · 2025-07-27 · **56 citations** (3 influential · 5.17/mo) · Keyan Ding, Jing Yu, Junjie Huang, Yuchen Yang et al.

## Abstract
Scientific research increasingly relies on specialized computational tools, yet effectively utilizing these tools demands substantial domain expertise. While Large Language Models (LLMs) show promise in tool automation, they struggle to seamlessly integrate and orchestrate multiple tools for complex scientific workflows. Here, we present SciToolAgent, an LLM-powered agent that automates hundreds of scientific tools across biology, chemistry, and materials science. At its core, SciToolAgent leverages a scientific tool knowledge graph that enables intelligent tool selection and execution through graph-based retrieval-augmented generation. The agent also incorporates a comprehensive safety-checking module to ensure responsible and ethical tool usage. Extensive evaluations on a curated benchmark demonstrate that SciToolAgent significantly outperforms existing approaches. Case studies in protein engineering, chemical reactivity prediction, chemical synthesis, and metal-organic framework screening further demonstrate SciToolAgent's capability to automate complex scientific workflows, making advanced research tools accessible to both experts and non-experts.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Results 2.1 Overview of SciToolAgent 2.2 Performance on SciToolEval 2.3 Case Studies 2.3.1 Protein design and analysis 2.3.2 Chemical reactivity prediction 2.3.3 Chemical synthesis and analysis 2.3.4 MOF materials screening 3 Discussion 4 Methods 4.1 Collection of Scientific Tools 4.2 Construction of SciToolKG 4.3 Construction of SciToolEval 4.4 Implementation of SciToolAgent 4.4.1 Planner 4.4.2 Executor 4.4.3 Summarizer 4.4.4 Foundation models \equalcont These authors contributed equally to this work. \equalcont These authors contributed equally to this work. [3,2] \fnm Qiang \sur Zhang [1,2,5] \fnm Huajun \sur Chen 1] \orgdiv College of Computer Science and Technology, \orgname Zhejiang University, Hangzhou, China 2] \orgdiv Zhejiang Key Laboratory of Intelligent Manufacturing for Functional Chemicals, ZJU-Hangzhou Global Scientific and Technological Innovation Center, \orgname Zhejiang University, Hangzhou, China 3] \orgdiv ZJU-UIUC Institute, \orgname Zhejiang University, Haining, China 4] \orgdiv The Pol…

**Method / approach.** Methods 4.1 Collection of Scientific Tools 4.2 Construction of SciToolKG 4.3 Construction of SciToolEval 4.4 Implementation of SciToolAgent 4.4.1 Planner 4.4.2 Executor 4.4.3 Summarizer 4.4.4 Foundation models \equalcont These authors contributed equally to this work. \equalcont These authors contributed equally to this work. [3,2] \fnm Qiang \sur Zhang [1,2,5] \fnm Huajun \sur Chen 1] \orgdiv College of Computer Science and Technology, \orgname Zhejiang University, Hangzhou, China 2] \orgdiv Zhejiang Key Laboratory of Intelligent Manufacturing for Functional Chemicals, ZJU-Hangzhou Global Scientific and Technological Innovation Center, \orgname Zhejiang University, Hangzhou, China 3] \orgdiv ZJU-UIUC Institute, \orgname Zhejiang University, Haining, China 4] \orgdiv The Polytechnic Institute, \orgname Zhejiang University, Hangzhou, China 5] \orgname State Key Laboratory of Ocean Sensing, Hangzhou, China SciToolAgent: A Knowledge Graph-Driven Scientif…

**Results.** experimental replicates is n = 5 n=5 italic_n = 5 , and the error bars are standard error of the mean. 2.2 Performance on SciToolEval Dataset: To quantitatively evaluate the performance of SciToolAgent, we curated SciToolEval, a comprehensive scientific tool evaluation dataset, comprising 531 diverse scientific questions across various fields, such as molecular property prediction, protein analysis, and material retrieval. The process of dataset construction is elaborated in Sec. 4.3 . The final dataset is divided into two levels: Level-1 includes 152 questions that can be addressed using a single tool, while Level-2 comprises 379 questions that require the use of multiple tools. Evaluation metrics: To rigorously assess the effectiveness of SciToolAgent, we utilize three distinct evaluation metrics: (1) Pass Rate, which quantifies the proportion of successfully completed queries; (2) Tool Planning Accuracy, which measures the…

**Conclusion.** Discussion 4 Methods 4.1 Collection of Scientific Tools 4.2 Construction of SciToolKG 4.3 Construction of SciToolEval 4.4 Implementation of SciToolAgent 4.4.1 Planner 4.4.2 Executor 4.4.3 Summarizer 4.4.4 Foundation models \equalcont These authors contributed equally to this work. \equalcont These authors contributed equally to this work. [3,2] \fnm Qiang \sur Zhang [1,2,5] \fnm Huajun \sur Chen 1] \orgdiv College of Computer Science and Technology, \orgname Zhejiang University, Hangzhou, China 2] \orgdiv Zhejiang Key Laboratory of Intelligent Manufacturing for Functional Chemicals, ZJU-Hangzhou Global Scientific and Technological Innovation Center, \orgname Zhejiang University, Hangzhou, China 3] \orgdiv Z…

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.20280v1.md` · `raw/arxiv/2507.20280v1.fulltext.md`
