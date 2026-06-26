---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SceneWeaver: All-in-One 3D Scene Synthesis with an Extensible and Self-Reflective Agent"
authors: Yandan Yang, Baoxiong Jia, Shujie Zhang, Siyuan Huang
url: https://arxiv.org/abs/2509.20414v2
date: 2025-09-24
citationCount: 37
influentialCitationCount: 7
velocity: 4.16
ingested: 2026-06-22
tags: [embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# SceneWeaver: All-in-One 3D Scene Synthesis with an Extensible and Self-Reflective Agent

**arXiv [2509.20414v2](https://arxiv.org/abs/2509.20414v2)** · 2025-09-24 · **37 citations** (7 influential · 4.16/mo) · Yandan Yang, Baoxiong Jia, Shujie Zhang, Siyuan Huang

## Abstract
Indoor scene synthesis has become increasingly important with the rise of Embodied AI, which requires 3D environments that are not only visually realistic but also physically plausible and functionally diverse. While recent approaches have advanced visual fidelity, they often remain constrained to fixed scene categories, lack sufficient object-level detail and physical consistency, and struggle to align with complex user instructions. In this work, we present SceneWeaver, a reflective agentic framework that unifies diverse scene synthesis paradigms through tool-based iterative refinement. At its core, SceneWeaver employs a language model-based planner to select from a suite of extensible scene generation tools, ranging from data-driven generative models to visual- and LLM-based methods, guided by self-evaluation of physical plausibility, visual realism, and semantic alignment with user input. This closed-loop reason-act-reflect design enables the agent to identify semantic inconsistencies, invoke targeted tools, and update the environment over successive iterations. Extensive experiments on both common and open-vocabulary room types demonstrate that SceneWeaver not only outperforms prior methods on physical, visual, and semantic metrics, but also generalizes effectively to complex scenes with diverse instructions, marking a step toward general-purpose 3D environment generation. Project website: https://scene-weaver.github.io/.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related work 3D Indoor Scene Synthesis Spatial Reasoning of LLM-based Agentic Framework 3 The SceneWeaver Framework 3.1 Standardized Scene Synthesis Tool Interface Tool Catalog Standardized Tool Cards 3.2 Feedback-driven Self-reflective Planning Reflection Generation Self-reflective Planning Physics-aware Execution of Plans 4 Experiment Settings Baselines Metrics 4.1 Scene Generation for Common Room Types 4.2 Open-vocabulary Scene Generation 4.3 Additional Analyses Ablation on Agent Design Effectiveness of Tool Cards Iterative Refinement in SceneWeaver with Complex Queries Human Study 5 Conclusion A Details of the SceneWeaver Framework A.1 Scene Representation A.2 Self-reflective Planner Task description: Note: Available Tools: User demand: Memory of step t-1 : Plan for step t : Task Score Guidelines Evaluation Criteria User demand Rendered Image Room layout Results A.3 Implementation of the executor A.4 Tool Cards A.5 Physics-aware Executor A.6 How to ch…

**Method / approach.** methods C Miscellaneous C.1 Claims in Tab. ˜ 1 Real Large-scale Accurate C.2 Broader Impact C.3 Resources used C.4 Time Consumption C.5 API Cost D Limitation D.1 Unrealistic Scaling Placement for Functional Items D.2 Validity of LLM’s Judgement Description Supported Room Types: Use Case 1 Strengths Weaknesses Input Description Supported Room Types Use Case 1 Strengths Weaknesses Input Description Supported Room Types Use Case 1 Strengths Weaknesses Input Description Use Case 1 Strengths Weaknesses Input Description Use Case 1 Use Case 2 Use Case 3 Use Case 4 Use Case 5 Strengths Weaknesses Input Description Use Case 1 Use Case 2 Use Case 3 Use Case 4 Strengths Weaknesses Input Description Use Case 1 Use Case 2 Use Case 3 Use Case 4 Strengths Weaknesses Input Description Use Case 1 Use Case 2 Strengths Weaknesses Input Description Use Case…

**Results.** Experiment Settings Baselines Metrics 4.1 Scene Generation for Common Room Types 4.2 Open-vocabulary Scene Generation 4.3 Additional Analyses Ablation on Agent Design Effectiveness of Tool Cards Iterative Refinement in SceneWeaver with Complex Queries Human Study 5 Conclusion A Details of the SceneWeaver Framework A.1 Scene Representation A.2 Self-reflective Planner Task description: Note: Available Tools: User demand: Memory of step t-1 : Plan for step t : Task Score Guidelines Evaluation Criteria User demand Rendered Image Room layout Results A.3 Implementation of the executor A.4 Tool Cards A.5 Physics-aware Executor A.6 How to choose assets dataset B Experiments B.1 Additional Experimental Details B.2 Additional Scene Generation Results B.3 Simulation in Isaac Sim B.4 User Study B.5 Human-LLM Alignment. B.6 Physical Stability B.7 Metric…

**Conclusion.** Conclusion A Details of the SceneWeaver Framework A.1 Scene Representation A.2 Self-reflective Planner Task description: Note: Available Tools: User demand: Memory of step t-1 : Plan for step t : Task Score Guidelines Evaluation Criteria User demand Rendered Image Room layout Results A.3 Implementation of the executor A.4 Tool Cards A.5 Physics-aware Executor A.6 How to choose assets dataset B Experiments B.1 Additional Experimental Details B.2 Additional Scene Generation Results B.3 Simulation in Isaac Sim B.4 User Study B.5 Human-LLM Alignment. B.6 Physical Stability B.7 Metric improvement during iteration. B.8 Impact of a single tool B.9 Room Structure Single Room Sc…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.20414v2.md` · `raw/arxiv/2509.20414v2.fulltext.md`
