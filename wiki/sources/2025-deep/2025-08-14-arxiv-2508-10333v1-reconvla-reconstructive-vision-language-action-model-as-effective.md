---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver"
authors: Wenxuan Song, Ziyang Zhou, Han Zhao, Jiayi Chen et al.
url: https://arxiv.org/abs/2508.10333v1
date: 2025-08-14
citationCount: 53
influentialCitationCount: 3
velocity: 5.17
ingested: 2026-06-22
tags: [embodied-agents, arxiv, 2025, cited]
---

# ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver

**arXiv [2508.10333v1](https://arxiv.org/abs/2508.10333v1)** · 2025-08-14 · **53 citations** (3 influential · 5.17/mo) · Wenxuan Song, Ziyang Zhou, Han Zhao, Jiayi Chen et al.

## Abstract
Recent advances in Vision-Language-Action (VLA) models have enabled robotic agents to integrate multimodal understanding with action execution. However, our empirical analysis reveals that current VLAs struggle to allocate visual attention to target regions. Instead, visual attention is always dispersed. To guide the visual attention grounding on the correct target, we propose ReconVLA, a reconstructive VLA model with an implicit grounding paradigm. Conditioned on the model's visual outputs, a diffusion transformer aims to reconstruct the gaze region of the image, which corresponds to the target manipulated objects. This process prompts the VLA model to learn fine-grained representations and accurately allocate visual attention, thus effectively leveraging task-specific visual information and conducting precise manipulation. Moreover, we curate a large-scale pretraining dataset comprising over 100k trajectories and 2 million data samples from open-source robotic datasets, further boosting the model's generalization in visual reconstruction. Extensive experiments in simulation and the real world demonstrate the superiority of our implicit grounding method, showcasing its capabilities of precise manipulation and generalization. Our project page is https://zionchow.github.io/ReconVLA/.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Action-centric Vision-language-action Models. Generative Methods for Manipulation. Visual Grounding Methods for Manipulation. 3 Method 3.1 Preliminaries Architecture. 3.2 Reconstructive Vision-Language-Action Model Reconstruction Target. Loss Function. Latent Visual Reconstruction. Implementation Details. 3.3 Visual Pretraining Dataset. Training. 4 Experiments 4.1 Simulation Environment 4.2 Paradigm Comparison Explicit Grounding (EG). Chain-of-Thought Grounding (CG). Results. 4.3 In-depth Analysis Attention Visualization Precise Manipulation. 4.4 Ablation Study 4.5 Comparison with State-of-the-arts Compared Methods. Results. 4.6 Multi-task Experiments in the Real World Setup. Tasks. Results. 5 Conclusion ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver Wenxuan Song 1 , Ziyang Zhou 1 , Han Zhao 2,3 , Jiayi Chen 1 , Pengxiang Ding 2,3 , Haodong Yan 1 , Yuxin Huang 1 , Feilong Tang 4 , Donglin Wang 2 , Haoang Li 1 Ab…

**Method / approach.** Methods for Manipulation. Visual Grounding Methods for Manipulation. 3 Method 3.1 Preliminaries Architecture. 3.2 Reconstructive Vision-Language-Action Model Reconstruction Target. Loss Function. Latent Visual Reconstruction. Implementation Details. 3.3 Visual Pretraining Dataset. Training. 4 Experiments 4.1 Simulation Environment 4.2 Paradigm Comparison Explicit Grounding (EG). Chain-of-Thought Grounding (CG). Results. 4.3 In-depth Analysis Attention Visualization Precise Manipulation. 4.4 Ablation Study 4.5 Comparison with State-of-the-arts Compared Methods. Results. 4.6 Multi-task Experiments in the Real World Setup. Tasks. Results. 5 Conclusion ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver Wenxuan Song 1 , Ziyang Zhou 1 , Han Zhao 2,3 , Jiayi Chen 1 , Pengxiang Ding 2,3 , Haodong Yan 1 , Yuxin Huang 1 , Feilong Tang 4 , Donglin Wang 2 , Haoang Li 1…

**Results.** Experiments 4.1 Simulation Environment 4.2 Paradigm Comparison Explicit Grounding (EG). Chain-of-Thought Grounding (CG). Results. 4.3 In-depth Analysis Attention Visualization Precise Manipulation. 4.4 Ablation Study 4.5 Comparison with State-of-the-arts Compared Methods. Results. 4.6 Multi-task Experiments in the Real World Setup. Tasks. Results. 5 Conclusion ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver Wenxuan Song 1 , Ziyang Zhou 1 , Han Zhao 2,3 , Jiayi Chen 1 , Pengxiang Ding 2,3 , Haodong Yan 1 , Yuxin Huang 1 , Feilong Tang 4 , Donglin Wang 2 , Haoang Li 1 Abstract Recent advances in Vision-Language-Action (VLA) models have enabled robotic agents to integrate multimodal understanding with action execution. However, our empirical analysis reveals that current VLAs struggle to allocate visual attention to target regions. Instead,…

**Conclusion.** Conclusion ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver Wenxuan Song 1 , Ziyang Zhou 1 , Han Zhao 2,3 , Jiayi Chen 1 , Pengxiang Ding 2,3 , Haodong Yan 1 , Yuxin Huang 1 , Feilong Tang 4 , Donglin Wang 2 , Haoang Li 1 Abstract Recent advances in Vision-Language-Action (VLA) models have enabled robotic agents to integrate multimodal understanding with action execution. However, our empirical analysis reveals that current VLAs struggle to allocate visual attention to target regions. Instead, visual attention is always dispersed. To guide the visual attention grounding on the correct target, we propose ReconVLA , a reconstructive VLA model with an implicit grounding paradigm. Conditioned on t…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]]
- **Entities:** [[vla]]
- **Raw:** `raw/arxiv/2508.10333v1.md` · `raw/arxiv/2508.10333v1.fulltext.md`
