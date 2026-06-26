---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Magma: A Foundation Model for Multimodal AI Agents"
authors: Jianwei Yang, Reuben Tan, Qianhui Wu, Ruijie Zheng et al.
url: https://arxiv.org/abs/2502.13130v1
date: 2025-02-18
citationCount: 149
influentialCitationCount: 11
velocity: 9.28
ingested: 2026-06-22
tags: [embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# Magma: A Foundation Model for Multimodal AI Agents

**arXiv [2502.13130v1](https://arxiv.org/abs/2502.13130v1)** · 2025-02-18 · **149 citations** (11 influential · 9.28/mo) · Jianwei Yang, Reuben Tan, Qianhui Wu, Ruijie Zheng et al.

## Abstract
We present Magma, a foundation model that serves multimodal AI agentic tasks in both the digital and physical worlds. Magma is a significant extension of vision-language (VL) models in that it not only retains the VL understanding ability (verbal intelligence) of the latter, but is also equipped with the ability to plan and act in the visual-spatial world (spatial-temporal intelligence) and complete agentic tasks ranging from UI navigation to robot manipulation. To endow the agentic capabilities, Magma is pretrained on large amounts of heterogeneous datasets spanning from images, videos to robotics data, where the actionable visual objects (e.g., clickable buttons in GUI) in images are labeled by Set-of-Mark (SoM) for action grounding, and the object movements (e.g., the trace of human hands or robotic arms) in videos are labeled by Trace-of-Mark (ToM) for action planning. Extensive experiments show that SoM and ToM reach great synergy and facilitate the acquisition of spatial-temporal intelligence for our Magma model, which is fundamental to a wide range of tasks as shown in Fig.1. In particular, Magma creates new state-of-the-art results on UI navigation and robotic manipulation tasks, outperforming previous models that are specifically tailored to these tasks. On image and video-related multimodal tasks, Magma also compares favorably to popular large multimodal models that are trained on much larger datasets. We make our model and code public for reproducibility at https://microsoft.github.io/Magma.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Multimodal Agentic Modeling 3.1 Problem Definition 3.2 Method 3.2.1 Set-of-Mark for Action Grounding 3.2.2 Trace-of-Mark for Action Planning 3.3 Modeling 4 Multimodal Agentic Pretraining 4.1 Datasets 4.2 SoM and ToM Generation 4.2.1 SoM for UI Navigation 4.2.2 SoM and ToM for Videos and Robotic Data 4.3 Pretraining 5 Experiment 5.1 Evaluating Agentic Capability 5.1.1 Zero-Shot Evaluation 5.1.2 Efficient Finetuning 5.2 Evaluating Spatial Reasoning 5.3 Evaluating Multimodal Understanding Image instruction tuning. Video Instruction Tuning 6 Conclusion Social Impacts and Limitations. Responsible AI . Acknowledgments. A Pretraining and Finetuning B Datasets B.1 Pretraining Data B.1.1 UI Navigation B.1.2 Instructional Videos B.1.3 Robotic Manipulation B.1.4 Multimodal Image Understanding B.1.5 Data Statistics B.2 Downstream Data B.2.1 UI Agent Navigation B.2.2 Robot Manipulation B.2.3 Image Instruction Tuning B.2.4 Video Instruction Tuning B.2.5…

**Method / approach.** Method 3.2.1 Set-of-Mark for Action Grounding 3.2.2 Trace-of-Mark for Action Planning 3.3 Modeling 4 Multimodal Agentic Pretraining 4.1 Datasets 4.2 SoM and ToM Generation 4.2.1 SoM for UI Navigation 4.2.2 SoM and ToM for Videos and Robotic Data 4.3 Pretraining 5 Experiment 5.1 Evaluating Agentic Capability 5.1.1 Zero-Shot Evaluation 5.1.2 Efficient Finetuning 5.2 Evaluating Spatial Reasoning 5.3 Evaluating Multimodal Understanding Image instruction tuning. Video Instruction Tuning 6 Conclusion Social Impacts and Limitations. Responsible AI . Acknowledgments. A Pretraining and Finetuning B Datasets B.1 Pretraining Data B.1.1 UI Navigation B.1.2 Instructional Videos B.1.3 Robotic Manipulation B.1.4 Multimodal Image Understanding B.1.5 Data Statistics B.2 Downstream Data B.2.1 UI Agent Navigation B.2.2 Robot Manipulation B.2.3 Image Instruction Tuning B.2.4 Video Instruction Tuning B.2.…

**Results.** Experiment 5.1 Evaluating Agentic Capability 5.1.1 Zero-Shot Evaluation 5.1.2 Efficient Finetuning 5.2 Evaluating Spatial Reasoning 5.3 Evaluating Multimodal Understanding Image instruction tuning. Video Instruction Tuning 6 Conclusion Social Impacts and Limitations. Responsible AI . Acknowledgments. A Pretraining and Finetuning B Datasets B.1 Pretraining Data B.1.1 UI Navigation B.1.2 Instructional Videos B.1.3 Robotic Manipulation B.1.4 Multimodal Image Understanding B.1.5 Data Statistics B.2 Downstream Data B.2.1 UI Agent Navigation B.2.2 Robot Manipulation B.2.3 Image Instruction Tuning B.2.4 Video Instruction Tuning B.2.5 Details about SoM for training and evaluation C Qualitative Analysis C.1 UI Navigation C.2 Robotics Manipulation Magma: A Foundation Model for Multimodal AI Agents Jianwei Yang 1* † † \dagger † Reuben Tan 1 † † \dagger † Qia…

**Conclusion.** Conclusion Social Impacts and Limitations. Responsible AI . Acknowledgments. A Pretraining and Finetuning B Datasets B.1 Pretraining Data B.1.1 UI Navigation B.1.2 Instructional Videos B.1.3 Robotic Manipulation B.1.4 Multimodal Image Understanding B.1.5 Data Statistics B.2 Downstream Data B.2.1 UI Agent Navigation B.2.2 Robot Manipulation B.2.3 Image Instruction Tuning B.2.4 Video Instruction Tuning B.2.5 Details about SoM for training and evaluation C Qualitative Analysis C.1 UI Navigation C.2 Robotics Manipulation Magma: A Foundation Model for Multimodal AI Agents Jianwei Yang 1* † † \dagger † Reuben Tan 1 † † \dagger † Qianhui Wu 1 † † \dagger † Ruijie Zheng 2 ‡ ‡ \dd…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.13130v1.md` · `raw/arxiv/2502.13130v1.fulltext.md`
