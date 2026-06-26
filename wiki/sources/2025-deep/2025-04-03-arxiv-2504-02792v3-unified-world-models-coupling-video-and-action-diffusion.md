---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets"
authors: Chuning Zhu, Raymond Yu, Siyuan Feng, Benjamin Burchfiel et al.
url: https://arxiv.org/abs/2504.02792v3
date: 2025-04-03
citationCount: 124
influentialCitationCount: 13
velocity: 8.48
ingested: 2026-06-22
tags: [embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets

**arXiv [2504.02792v3](https://arxiv.org/abs/2504.02792v3)** · 2025-04-03 · **124 citations** (13 influential · 8.48/mo) · Chuning Zhu, Raymond Yu, Siyuan Feng, Benjamin Burchfiel et al.

## Abstract
Imitation learning has emerged as a promising approach towards building generalist robots. However, scaling imitation learning for large robot foundation models remains challenging due to its reliance on high-quality expert demonstrations. Meanwhile, large amounts of video data depicting a wide range of environments and diverse behaviors are readily available. This data provides a rich source of information about real-world dynamics and agent-environment interactions. Leveraging this data directly for imitation learning, however, has proven difficult due to the lack of action annotation. In this work, we present Unified World Models (UWM), a framework that allows for leveraging both video and action data for policy learning. Specifically, a UWM integrates an action diffusion process and a video diffusion process within a unified transformer architecture, where independent diffusion timesteps govern each modality. By controlling each diffusion timestep, UWM can flexibly represent a policy, a forward dynamics, an inverse dynamics, and a video generator. Through simulated and real-world experiments, we show that: (1) UWM enables effective pretraining on large-scale multitask robot datasets with both dynamics and action predictions, resulting in more generalizable and robust policies than imitation learning, (2) UWM naturally facilitates learning from action-free video data through independent control of modality-specific diffusion timesteps, further improving the performance of finetuned policies. Our results suggest that UWM offers a promising step toward harnessing large, heterogeneous datasets for scalable robot learning, and provides a simple unification between the often disparate paradigms of imitation learning and world modeling. Videos and code are available at https://weirdlabuw.github.io/uwm/.

## From the paper (full-text excerpts)
**Introduction.** Introduction II Preliminaries II-A Diffusion Models Conditional Generation with Diffusion Models III Method III-A Problem Setup III-B Unified World Models via Coupled Video-Action Diffusion III-C Architecture III-D Training Paradigms IV Experiments IV-A Baselines IV-B Real Robot Experiments IV-B 1 Setup IV-B 2 Discussion IV-C Simulated Experiments IV-D Analysis and Ablation Experiments IV-D 1 Forward Dynamics IV-D 2 Inverse Dynamics IV-D 3 Categorized OOD Experiments IV-D 4 Real-World Learning from Scratch V Related Work Imitation Learning Learning from Videos Unified Inference VI Discussion VII Limitations -A Additional Implementation Details -A 1 Model Architecture -A 2 Training and Inference Details -A 3 Training Compute -B Baseline Details -B 1 Diffusion Policies -B 2 PAD -B 3 GR1 -C Additional Details on Real-World Experiments -C 1 Robot Setup -C 2 Tasks -C 3 Evaluation Protocol -C 4 Failure Modes A Additional Details on Simulated Experiments A- 1 Simulated Enviro…

**Method / approach.** Method III-A Problem Setup III-B Unified World Models via Coupled Video-Action Diffusion III-C Architecture III-D Training Paradigms IV Experiments IV-A Baselines IV-B Real Robot Experiments IV-B 1 Setup IV-B 2 Discussion IV-C Simulated Experiments IV-D Analysis and Ablation Experiments IV-D 1 Forward Dynamics IV-D 2 Inverse Dynamics IV-D 3 Categorized OOD Experiments IV-D 4 Real-World Learning from Scratch V Related Work Imitation Learning Learning from Videos Unified Inference VI Discussion VII Limitations -A Additional Implementation Details -A 1 Model Architecture -A 2 Training and Inference Details -A 3 Training Compute -B Baseline Details -B 1 Diffusion Policies -B 2 PAD -B 3 GR1 -C Additional Details on Real-World Experiments -C 1 Robot Setup -C 2 Tasks -C 3 Evaluation Protocol -C 4 Failure Modes A Additional Details on Simulated Experiments A- 1 Simulated Environments A-A…

**Results.** Experiments IV-A Baselines IV-B Real Robot Experiments IV-B 1 Setup IV-B 2 Discussion IV-C Simulated Experiments IV-D Analysis and Ablation Experiments IV-D 1 Forward Dynamics IV-D 2 Inverse Dynamics IV-D 3 Categorized OOD Experiments IV-D 4 Real-World Learning from Scratch V Related Work Imitation Learning Learning from Videos Unified Inference VI Discussion VII Limitations -A Additional Implementation Details -A 1 Model Architecture -A 2 Training and Inference Details -A 3 Training Compute -B Baseline Details -B 1 Diffusion Policies -B 2 PAD -B 3 GR1 -C Additional Details on Real-World Experiments -C 1 Robot Setup -C 2 Tasks -C 3 Evaluation Protocol -C 4 Failure Modes A Additional Details on Simulated Experiments A- 1 Simulated Environments A-A Additional Experiments A-A 1 Ablations of Design Choices A-A 2 Ablation of Learning Objective…

**Conclusion.** Discussion IV-C Simulated Experiments IV-D Analysis and Ablation Experiments IV-D 1 Forward Dynamics IV-D 2 Inverse Dynamics IV-D 3 Categorized OOD Experiments IV-D 4 Real-World Learning from Scratch V Related Work Imitation Learning Learning from Videos Unified Inference VI Discussion VII Limitations -A Additional Implementation Details -A 1 Model Architecture -A 2 Training and Inference Details -A 3 Training Compute -B Baseline Details -B 1 Diffusion Policies -B 2 PAD -B 3 GR1 -C Additional Details on Real-World Experiments -C 1 Robot Setup -C 2 Tasks -C 3 Evaluation Protocol -C 4 Failure Modes A Additional Details on Simulated Experiments A- 1 Simulated Environme…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.02792v3.md` · `raw/arxiv/2504.02792v3.fulltext.md`
