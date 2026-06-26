---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Scaling Computer-Use Grounding via User Interface Decomposition and Synthesis"
authors: Tianbao Xie, Jiaqi Deng, Xiaochuan Li, Junlin Yang et al.
url: https://arxiv.org/abs/2505.13227v3
date: 2025-05-19
citationCount: 101
influentialCitationCount: 24
velocity: 7.71
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Scaling Computer-Use Grounding via User Interface Decomposition and Synthesis

**arXiv [2505.13227v3](https://arxiv.org/abs/2505.13227v3)** · 2025-05-19 · **101 citations** (24 influential · 7.71/mo) · Tianbao Xie, Jiaqi Deng, Xiaochuan Li, Junlin Yang et al.

## Abstract
Graphical user interface (GUI) grounding, the ability to map natural language instructions to specific actions on graphical user interfaces, remains a critical bottleneck in computer use agent development. Current benchmarks oversimplify grounding tasks as short referring expressions, failing to capture the complexity of real-world interactions that require software commonsense, layout understanding, and fine-grained manipulation capabilities. To address these limitations, we introduce OSWorld-G, a comprehensive benchmark comprising 564 finely annotated samples across diverse task types including text matching, element recognition, layout understanding, and precise manipulation. Additionally, we synthesize and release the largest computer use grounding dataset Jedi, which contains 4 million examples through multi-perspective decoupling of tasks. Our multi-scale models trained on Jedi demonstrate its effectiveness by outperforming existing approaches on ScreenSpot-v2, ScreenSpot-Pro, and our OSWorld-G. Furthermore, we demonstrate that improved grounding with Jedi directly enhances agentic capabilities of general foundation models on complex computer tasks, improving from 5% to 27% on OSWorld. Through detailed ablation studies, we identify key factors contributing to grounding performance and verify that combining specialized data for different interface elements enables compositional generalization to novel interfaces. All benchmark, data, checkpoints, and code are open-sourced and available at https://osworld-grounding.github.io.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Approach Task Definition 2.1 OSWorld-G 2.1.1 Benchmark Construction 2.1.2 Data Types Text Matching Element Recognition Layout Understanding Fine-grained Manipulation Infeasible 2.2 Jedi Data Construction 2.2.1 Icon GitHub Repositories and Specialized Icon Websites Reverse Engineering Software 2.2.2 Component Synthesis Process Real-world Augmentation 2.2.3 Layout Prototype Designs Real-World Application Screenshots 2.2.4 Data Processing 2.2.5 Supplementary Training Data 3 Experiments 3.1 Grounding Ability 3.2 Agentic Ability 4 Analysis 4.1 Effectiveness of Knowledge 4.2 Performance as Data Scaling 4.3 Case Study 5 Related Work Digital Agents GUI Grounding 6 Conclusion 7 Limitations A Appendix A.1 OSWorld-G Statistics A.1.1 Data Types A.1.2 Comparison with Previous Work A.1.3 Data Examples Layout Understanding Fine-grained Manipulation Text Matching Element Recognition Refusal Instruction A.1.4 Annotation Details A.2 Jedi Statistics A.…

**Method / approach.** methods in Figure 4 provides an overview of this pipeline. 2.2.1 Icon Icons are essential visual elements in graphical user interfaces that convey functionality through compact, recognizable imagery. To create a comprehensive collection of icons and corresponding metadata for grounding, we employ three complementary data collection strategies. GitHub Repositories and Specialized Icon Websites Many open-source software projects archive their design icons within GitHub repositories. To acquire a varied collection, we systematically mine repositories containing the key term such as “icon” applying filtering criteria including star count, quantity of icon images, and temporal relevance. This yield icons representing various design paradigms such as flat design, fluent design, and skeuomorphism. To supplement our collection with production website icons, we implement a targeted web crawling pipeline that identifies and extracts icon elements from popular websites across vari…

**Results.** Experiments 3.1 Grounding Ability 3.2 Agentic Ability 4 Analysis 4.1 Effectiveness of Knowledge 4.2 Performance as Data Scaling 4.3 Case Study 5 Related Work Digital Agents GUI Grounding 6 Conclusion 7 Limitations A Appendix A.1 OSWorld-G Statistics A.1.1 Data Types A.1.2 Comparison with Previous Work A.1.3 Data Examples Layout Understanding Fine-grained Manipulation Text Matching Element Recognition Refusal Instruction A.1.4 Annotation Details A.2 Jedi Statistics A.2.1 Overview A.2.2 Icon Statistics A.2.3 Component Statistics A.2.4 Layout Statistics A.2.5 Cost Analysis A.3 Jedi Dataset Construction: A Detailed Pipeline for Component A.3.1 Component Collection and Style Augmentation A.3.2 Rendering and Interaction Preparation Step 1: Generate Action Intents Example Example Step 1: Element Extraction and Filtering Step 2: Multimodal Context E…

**Conclusion.** Conclusion 7 Limitations A Appendix A.1 OSWorld-G Statistics A.1.1 Data Types A.1.2 Comparison with Previous Work A.1.3 Data Examples Layout Understanding Fine-grained Manipulation Text Matching Element Recognition Refusal Instruction A.1.4 Annotation Details A.2 Jedi Statistics A.2.1 Overview A.2.2 Icon Statistics A.2.3 Component Statistics A.2.4 Layout Statistics A.2.5 Cost Analysis A.3 Jedi Dataset Construction: A Detailed Pipeline for Component A.3.1 Component Collection and Style Augmentation A.3.2 Rendering and Interaction Preparation Step 1: Generate Action Intents Example Example Step 1: Element Extraction and Filtering Step 2: Multimodal Context Encoding Step 3:…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[osworld]]
- **Raw:** `raw/arxiv/2505.13227v3.md` · `raw/arxiv/2505.13227v3.fulltext.md`
