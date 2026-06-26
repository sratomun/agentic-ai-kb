---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GLM-4.5V and GLM-4.1V-Thinking: Towards Versatile Multimodal Reasoning with Scalable Reinforcement Learning"
authors: GLM-V Team, :, Wenyi Hong, Wenmeng Yu et al.
url: https://arxiv.org/abs/2507.01006v6
date: 2025-07-01
citationCount: 263
influentialCitationCount: 28
velocity: 22.49
ingested: 2026-06-22
tags: [computer-use-agents, agentic-rl, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# GLM-4.5V and GLM-4.1V-Thinking: Towards Versatile Multimodal Reasoning with Scalable Reinforcement Learning

**arXiv [2507.01006v6](https://arxiv.org/abs/2507.01006v6)** · 2025-07-01 · **263 citations** (28 influential · 22.49/mo) · GLM-V Team, :, Wenyi Hong, Wenmeng Yu et al.

## Abstract
We present GLM-4.1V-Thinking, GLM-4.5V, and GLM-4.6V, a family of vision-language models (VLMs) designed to advance general-purpose multimodal understanding and reasoning. In this report, we share our key findings in the development of the reasoning-centric training framework. We first develop a capable vision foundation model with significant potential through large-scale pre-training, which arguably sets the upper bound for the final performance. We then propose Reinforcement Learning with Curriculum Sampling (RLCS) to unlock the full potential of the model, leading to comprehensive capability enhancement across a diverse range of tasks, including STEM problem solving, video understanding, content recognition, coding, grounding, GUI-based agents, and long document interpretation. In a comprehensive evaluation across 42 public benchmarks, GLM-4.5V achieves state-of-the-art performance on nearly all tasks among open-source models of similar size, and demonstrates competitive or even superior results compared to closed-source models such as Gemini-2.5-Flash on challenging tasks including Coding and GUI Agents. Meanwhile, the smaller GLM-4.1V-9B-Thinking remains highly competitive-achieving superior results to the much larger Qwen2.5-VL-72B on 29 benchmarks. We open-source both GLM-4.1V-9B-Thinking and GLM-4.5V. We further introduce the GLM-4.6V series, open-source multimodal models with native tool use and a 128K context window. A brief overview is available at https://z.ai/blog/glm-4.6v. Code, models and more information are released at https://github.com/zai-org/GLM-V.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Overview and Architecture 3 Pre-training 3.1 Pre-training Data 3.2 Training Recipe 4 Supervised Fine-Tuning 4.1 Supervised Fine-Tuning Data 4.2 Training Recipe 5 Reinforcement Learning: What Is Challenging and What Works 5.1 Data Preparation 5.2 Reward System 5.3 Reinforcement Learning with Curriculum Sampling (RLCS) 5.3.1 Improving Effectiveness 5.3.2 Improving Stability 5.4 Infrastructure 6 Evaluation 6.1 Evaluation Setting Benchmarks. Setting. Evaluation protocol and instructions. 6.2 Comparison to Other Advanced MLLMs 6.3 Investigating Cross-Domain Generalization in Reinforcement Learning 7 Discussion: Limitations and Future Work 8 Contribution A Qualitative Examples A.1 UI Code Generation A.2 Video Description Setting Atmosphere Characters Actions Interaction Mood Object Details A.3 Video Description (in Chinese) 场景与环境 人物与互动 氛围与情感 A.4 Video QA A.5 GUI Agent A.6 Chart QA A.7 Geolocation A.8 OCR + Coding A.9 Chemistry Problem Solving A.10 Math Problem S…

**Method / approach.** methodology inspired by Nougat [ blecher2023nougat ] . A large corpus of papers is sourced from arXiv, where the LaTeX source code is first normalized and converted to HTML format using the LaTeXML tool. The HTML is then parsed and transformed into a lightweight markup language. Finally, this content is segmented according to the original PDF page breaks and rasterized, creating a high-quality dataset of paired PDF page renderings and their corresponding structured source markup. Grounding data. To endow the model with precise visual localization capabilities, we construct a hybrid grounding dataset spanning two primary domains: natural images and graphical user interfaces (GUIs). 1. Natural image grounding : In the domain of natural images, we utilize LAION-115M [ li2023blip ] as a foundational dataset. Leveraging the GLIPv2 [ zhang2022glipv2 ] model, we parse the caption of each image and automatically predict the corresponding bounding boxes for every noun phrase. To e…

**Results.** Experimental Results of GLM-4.1V-9B-Thinking GLM-4.5V and GLM-4.1V-Thinking: Towards Versatile Multimodal Reasoning with Scalable Reinforcement Learning GLM-V Team Zhipu AI Tsinghua University (For the complete list of authors, please refer to the Contribution section) Abstract We present GLM-4.1V-Thinking, GLM-4.5V, and GLM-4.6V, a family of vision-language models (VLMs) designed to advance general-purpose multimodal understanding and reasoning. In this report, we share our key findings in the development of the reasoning-centric training framework. We first develop a capable vision foundation model with significant potential through large-scale pre-training, which arguably sets the upper bound for the final performance. We then propose R einforcement L earning with C urriculum S ampling ( RLCS ) to unlock the full potential of the model, leading to comprehensive capability enhancement across a diverse range of tasks,…

**Conclusion.** Discussion: Limitations and Future Work 8 Contribution A Qualitative Examples A.1 UI Code Generation A.2 Video Description Setting Atmosphere Characters Actions Interaction Mood Object Details A.3 Video Description (in Chinese) 场景与环境 人物与互动 氛围与情感 A.4 Video QA A.5 GUI Agent A.6 Chart QA A.7 Geolocation A.8 OCR + Coding A.9 Chemistry Problem Solving A.10 Math Problem Solving A.11 Long Document Understanding A.12 Spatial Reasoning A.13 Visual Grounding A.14 Tool Using B Evaluation Protocols and Instructions B.1 Evaluation Protocol of VLM Coding B.2 GUI Agent Instructions B.3 Visual Grounding Instructions C Experimental Results of GLM-4.1V-9B-Thinking GLM-4.5V and GLM-4.1…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[glm-45]]
- **Raw:** `raw/arxiv/2507.01006v6.md` · `raw/arxiv/2507.01006v6.fulltext.md`
