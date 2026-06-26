---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "TesserAct: Learning 4D Embodied World Models"
authors: Haoyu Zhen, Qiao Sun, Hongxin Zhang, Junyan Li et al.
url: https://arxiv.org/abs/2504.20995v1
date: 2025-04-29
citationCount: 65
influentialCitationCount: 10
velocity: 4.72
ingested: 2026-06-22
tags: [embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# TesserAct: Learning 4D Embodied World Models

**arXiv [2504.20995v1](https://arxiv.org/abs/2504.20995v1)** · 2025-04-29 · **65 citations** (10 influential · 4.72/mo) · Haoyu Zhen, Qiao Sun, Hongxin Zhang, Junyan Li et al.

## Abstract
This paper presents an effective approach for learning novel 4D embodied world models, which predict the dynamic evolution of 3D scenes over time in response to an embodied agent's actions, providing both spatial and temporal consistency. We propose to learn a 4D world model by training on RGB-DN (RGB, Depth, and Normal) videos. This not only surpasses traditional 2D models by incorporating detailed shape, configuration, and temporal changes into their predictions, but also allows us to effectively learn accurate inverse dynamic models for an embodied agent. Specifically, we first extend existing robotic manipulation video datasets with depth and normal information leveraging off-the-shelf models. Next, we fine-tune a video generation model on this annotated dataset, which jointly predicts RGB-DN (RGB, Depth, and Normal) for each frame. We then present an algorithm to directly convert generated RGB, Depth, and Normal videos into a high-quality 4D scene of the world. Our method ensures temporal and spatial coherence in 4D scene predictions from embodied scenarios, enables novel view synthesis for embodied environments, and facilitates policy learning that significantly outperforms those derived from prior video-based world models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Preliminaries 3.1 Latent Video Diffusion Models 3.2 Depth Optimization via Normal Integration 4 Learning a 4D Embodied World Model 4.1 4D Embodied Video Dataset 4.2 Model Architecture and Training Strategy 4.3 4D Scene Reconstruction 4.4 Embodied Action Planning with 4D Scenes 5 Experiments 5.1 4D Scene Prediction 5.1.1 Setup 5.1.2 Results and Analysis 5.2 Embodied Action Planning 5.2.1 Results and Analysis 6 Conclusion 7 Limitations 1 Implementation Details 1.1 Video Diffusion Model Details 1.2 4D Scene Generation 1.3 Implementation Details for Robotics Planning 2 More Qualitative Results 2.1 Data Annotation 2.2 4D Generation 2.3 Video Generation 2.4 Explicit Action Planning Tes ser Act : Learning 4D Embodied World Models Haoyu Zhen 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Qiao Sun 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Hongxin Zhang 1 Junyan Li 1 Siyuan Zhou 2 Yilun Du 3 Chuang Gan 1 1 UMass Amherst 2 HKUST 3…

**Method / approach.** method ensures temporal and spatial coherence in 4D scene predictions from embodied scenarios, enables novel view synthesis for embodied environments, and facilitates policy learning that significantly outperforms those derived from prior video-based world models. https://TesserActWorld.github.io Figure 1 : We propose TesserAct, the 4D Embodied World Model, which takes an input image and text instruction to generate RGB, depth, and normal videos, reconstructing a 4D scene and predicting actions. Our model not only achieves strong performance on in-domain data (right) but also generalizes effectively to unseen scenes, novel objects (top left), and cross-domain scenarios (bottom left). † † footnotetext: ∗ Equal contribution. 1 Introduction Learned world models [ 21 , 67 , 77 , 64 ] , which simulate environmental dynamics, play a crucial role in enabling embodied intelligent agents. Such models enable flexible policy synthesis [ 15 , 40 ] , data simulation and generation…

**Results.** Experiments 5.1 4D Scene Prediction 5.1.1 Setup 5.1.2 Results and Analysis 5.2 Embodied Action Planning 5.2.1 Results and Analysis 6 Conclusion 7 Limitations 1 Implementation Details 1.1 Video Diffusion Model Details 1.2 4D Scene Generation 1.3 Implementation Details for Robotics Planning 2 More Qualitative Results 2.1 Data Annotation 2.2 4D Generation 2.3 Video Generation 2.4 Explicit Action Planning Tes ser Act : Learning 4D Embodied World Models Haoyu Zhen 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Qiao Sun 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Hongxin Zhang 1 Junyan Li 1 Siyuan Zhou 2 Yilun Du 3 Chuang Gan 1 1 UMass Amherst 2 HKUST 3 Harvard University Abstract This paper presents an effective approach for learning novel 4D embodied world models, which predict the dynamic evolution of 3D scenes over time in respon…

**Conclusion.** Conclusion 7 Limitations 1 Implementation Details 1.1 Video Diffusion Model Details 1.2 4D Scene Generation 1.3 Implementation Details for Robotics Planning 2 More Qualitative Results 2.1 Data Annotation 2.2 4D Generation 2.3 Video Generation 2.4 Explicit Action Planning Tes ser Act : Learning 4D Embodied World Models Haoyu Zhen 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Qiao Sun 1 ⁣ ∗ 1 {}^{1\ *} start_FLOATSUPERSCRIPT 1 ∗ end_FLOATSUPERSCRIPT Hongxin Zhang 1 Junyan Li 1 Siyuan Zhou 2 Yilun Du 3 Chuang Gan 1 1 UMass Amherst 2 HKUST 3 Harvard University Abstract This paper presents an effective approach for learning novel 4D embodied world models, which predict the dy…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.20995v1.md` · `raw/arxiv/2504.20995v1.fulltext.md`
