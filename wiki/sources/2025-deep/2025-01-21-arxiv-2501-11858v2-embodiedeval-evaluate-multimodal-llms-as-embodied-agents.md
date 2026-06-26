---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "EmbodiedEval: Evaluate Multimodal LLMs as Embodied Agents"
authors: Zhili Cheng, Yuge Tu, Ran Li, Shiqi Dai et al.
url: https://arxiv.org/abs/2501.11858v2
date: 2025-01-21
citationCount: 52
influentialCitationCount: 2
velocity: 3.06
ingested: 2026-06-22
tags: [embodied-agents, agent-evaluation, arxiv, 2025, cited]
---

# EmbodiedEval: Evaluate Multimodal LLMs as Embodied Agents

**arXiv [2501.11858v2](https://arxiv.org/abs/2501.11858v2)** · 2025-01-21 · **52 citations** (2 influential · 3.06/mo) · Zhili Cheng, Yuge Tu, Ran Li, Shiqi Dai et al.

## Abstract
Multimodal Large Language Models (MLLMs) have shown significant advancements, providing a promising future for embodied agents. Existing benchmarks for evaluating MLLMs primarily utilize static images or videos, limiting assessments to non-interactive scenarios. Meanwhile, existing embodied AI benchmarks are task-specific and not diverse enough, which do not adequately evaluate the embodied capabilities of MLLMs. To address this, we propose EmbodiedEval, a comprehensive and interactive evaluation benchmark for MLLMs with embodied tasks. EmbodiedEval features 328 distinct tasks within 125 varied 3D scenes, each of which is rigorously selected and annotated. It covers a broad spectrum of existing embodied AI tasks with significantly enhanced diversity, all within a unified simulation and evaluation framework tailored for MLLMs. The tasks are organized into five categories: navigation, object interaction, social interaction, attribute question answering, and spatial question answering to assess different capabilities of the agents. We evaluated the state-of-the-art MLLMs on EmbodiedEval and found that they have a significant shortfall compared to human level on embodied tasks. Our analysis demonstrates the limitations of existing MLLMs in embodied capabilities, providing insights for their future development. We open-source all evaluation data and simulation framework at https://github.com/thunlp/EmbodiedEval.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 EmbodiedEval 3.1 Evaluation Formulation 3.2 Task Categories 3.3 Benchmark Construction 3.3.1 Scene Collection 3.3.2 Task Collection 3.3.3 Task Annotation 3.4 Dataset Statistics 4 Experiments 4.1 Experimental Setup 4.2 Main Results 4.3 Performance Analysis 4.4 Error Case Analysis 4.5 Future Improvements 5 Conclusion 6 Limitations 7 Potential Risks A Task Samples B Details of Evaluation Framework B.1 Movement Space B.2 Interaction Space B.3 Answering Space B.4 Success Criteria C Details of Task Annotation C.1 Annotation Process C.2 Annotation Criteria C.3 Annotation System C.4 Quality Control D Creation of Objaverse Synthetic E Temperature Setting F Success Cases F.1 Attribute QA F.2 Spatial QA F.3 Navigation F.4 Object Interaction F.5 Social Interaction G Error Cases G.1 Attribute QA G.2 Spatial QA G.3 Navigation G.4 Object Interaction G.5 Social Interaction EmbodiedEval : Evaluate Multimodal LLMs as Embodied Agents Zhili Cheng ‡ Yug…

**Method / approach.** methods (Deitke et al., 2022 ) , we sequentially placed them based on their attributes. After the scene is generated, we further refine the scenes using a self-developed runtime scene editor. See more details about this synthetic process in Appendix D . In addition, we incorporate indoor room scenes with interactive objects from AI2THOR, and some public spaces, such as stores and supermarkets, from HSSD and Sketchfab. We organize all scenes into the same format. 3.3.2 Task Collection For task collection, we first gather seed tasks for each of the five task categories from over 30 existing datasets. Using these tasks as seeds, we prompt Claude and ChatGPT to generate diverse task examples. We ask the LLMs to incorporate various capabilities, including complex grounding, episodic memory, spatial reasoning, quantitative reasoning, common sense reasoning, and planning, which resulted in many novel tasks. From this extensive task pool, we select over 300 distinct tasks as the cand…

**Results.** Experiments 4.1 Experimental Setup 4.2 Main Results 4.3 Performance Analysis 4.4 Error Case Analysis 4.5 Future Improvements 5 Conclusion 6 Limitations 7 Potential Risks A Task Samples B Details of Evaluation Framework B.1 Movement Space B.2 Interaction Space B.3 Answering Space B.4 Success Criteria C Details of Task Annotation C.1 Annotation Process C.2 Annotation Criteria C.3 Annotation System C.4 Quality Control D Creation of Objaverse Synthetic E Temperature Setting F Success Cases F.1 Attribute QA F.2 Spatial QA F.3 Navigation F.4 Object Interaction F.5 Social Interaction G Error Cases G.1 Attribute QA G.2 Spatial QA G.3 Navigation G.4 Object Interaction G.5 Social Interaction EmbodiedEval : Evaluate Multimodal LLMs as Embodied Agents Zhili Cheng ‡ Yuge Tu ∗ Ran Li ∗ Shiqi Dai ∗ Jinyi Hu ∗ ‡ absent ‡ {}^{*\hskip 0.70004pt{\ddagger}} s…

**Conclusion.** Conclusion 6 Limitations 7 Potential Risks A Task Samples B Details of Evaluation Framework B.1 Movement Space B.2 Interaction Space B.3 Answering Space B.4 Success Criteria C Details of Task Annotation C.1 Annotation Process C.2 Annotation Criteria C.3 Annotation System C.4 Quality Control D Creation of Objaverse Synthetic E Temperature Setting F Success Cases F.1 Attribute QA F.2 Spatial QA F.3 Navigation F.4 Object Interaction F.5 Social Interaction G Error Cases G.1 Attribute QA G.2 Spatial QA G.3 Navigation G.4 Object Interaction G.5 Social Interaction EmbodiedEval : Evaluate Multimodal LLMs as Embodied Agents Zhili Cheng ‡ Yuge Tu ∗ Ran Li ∗ Shiqi Dai ∗…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2501.11858v2.md` · `raw/arxiv/2501.11858v2.fulltext.md`
