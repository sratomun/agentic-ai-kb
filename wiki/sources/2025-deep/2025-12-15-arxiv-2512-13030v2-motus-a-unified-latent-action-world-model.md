---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Motus: A Unified Latent Action World Model"
authors: Hongzhe Bi, Hengkai Tan, Shenghao Xie, Zeyuan Wang et al.
url: https://arxiv.org/abs/2512.13030v2
date: 2025-12-15
citationCount: 91
influentialCitationCount: 13
velocity: 14.66
ingested: 2026-06-22
tags: [embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# Motus: A Unified Latent Action World Model

**arXiv [2512.13030v2](https://arxiv.org/abs/2512.13030v2)** · 2025-12-15 · **91 citations** (13 influential · 14.66/mo) · Hongzhe Bi, Hengkai Tan, Shenghao Xie, Zeyuan Wang et al.

## Abstract
While a general embodied agent must function as a unified system, current methods are built on isolated models for understanding, world modeling, and control. This fragmentation prevents unifying multimodal generative capabilities and hinders learning from large-scale, heterogeneous data. In this paper, we propose Motus, a unified latent action world model that leverages existing general pretrained models and rich, sharable motion information. Motus introduces a Mixture-of-Transformer (MoT) architecture to integrate three experts (i.e., understanding, video generation, and action) and adopts a UniDiffuser-style scheduler to enable flexible switching between different modeling modes (i.e., world models, vision-language-action models, inverse dynamics models, video generation models, and video-action joint prediction models). Motus further leverages the optical flow to learn latent actions and adopts a recipe with three-phase training pipeline and six-layer data pyramid, thereby extracting pixel-level "delta action" and enabling large-scale action pretraining. Experiments show that Motus achieves superior performance against state-of-the-art methods in both simulation (a +15% improvement over X-VLA and a +45% improvement over Pi0.5) and real-world scenarios(improved by +11~48%), demonstrating unified modeling of all functionalities and priors significantly benefits downstream robotic tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Unified Multimodal Models 2.2 Latent Action Models 3 Problem Formulation and Challenges Embodied Policies Challenge 1: Unifying Multimodal Generative Capabilities. Challenge 2: Utilization of Heterogeneous Data. 4 Methodology 4.1 Motus Model Architecture. Action-Dense Video-Sparse Prediction. Experts Details. 4.2 Latent Actions Optical Flow Based Representation. Training and Distribution Alignment. 4.3 Model Training and Data Motus Training. Data. 5 Experiments 5.1 Baselines 5.2 Evaluation in Simulation Environment 5.3 Real-World Experiments 5.4 Ablation Study 6 Conclusion and Limitations 7 Training and Inference of the Unified Model 7.1 Theorectical Analysis VGM. World Model. IDM. VLA. Video-Action Joint Prediction Model. 7.2 Experimental Results VGM. World Model. IDM. Video-Action Joint Prediction Model. 8 More Experiments Results 8.1 Overall Comparison on RoboTwin 2.0 Simulation Data with More Baselines 8.2 Other Benchmarks LIBERO-Lon…

**Method / approach.** Methodology 4.1 Motus Model Architecture. Action-Dense Video-Sparse Prediction. Experts Details. 4.2 Latent Actions Optical Flow Based Representation. Training and Distribution Alignment. 4.3 Model Training and Data Motus Training. Data. 5 Experiments 5.1 Baselines 5.2 Evaluation in Simulation Environment 5.3 Real-World Experiments 5.4 Ablation Study 6 Conclusion and Limitations 7 Training and Inference of the Unified Model 7.1 Theorectical Analysis VGM. World Model. IDM. VLA. Video-Action Joint Prediction Model. 7.2 Experimental Results VGM. World Model. IDM. Video-Action Joint Prediction Model. 8 More Experiments Results 8.1 Overall Comparison on RoboTwin 2.0 Simulation Data with More Baselines 8.2 Other Benchmarks LIBERO-Long. VLABench. 8.3 More Real-World Results 9 Implementation Details 9.1 Model Architecture 9.2 Datasets 9.3 Training Configuration Motus: A Unified Laten…

**Results.** Experiments 5.1 Baselines 5.2 Evaluation in Simulation Environment 5.3 Real-World Experiments 5.4 Ablation Study 6 Conclusion and Limitations 7 Training and Inference of the Unified Model 7.1 Theorectical Analysis VGM. World Model. IDM. VLA. Video-Action Joint Prediction Model. 7.2 Experimental Results VGM. World Model. IDM. Video-Action Joint Prediction Model. 8 More Experiments Results 8.1 Overall Comparison on RoboTwin 2.0 Simulation Data with More Baselines 8.2 Other Benchmarks LIBERO-Long. VLABench. 8.3 More Real-World Results 9 Implementation Details 9.1 Model Architecture 9.2 Datasets 9.3 Training Configuration Motus: A Unified Latent Action World Model Hongzhe Bi 1∗† , Hengkai Tan 1∗† , Shenghao Xie 2,1∗ , Zeyuan Wang 1∗ , Shuhe Huang 1∗ , Haitian Liu 1∗ , Ruowen Zhao 1 , Yao Feng 1 , Chendong Xiang 1 , Yinze Rong 1 , Hongyan Zhao 1 , Hanyu Liu 2 ,…

**Conclusion.** Conclusion and Limitations 7 Training and Inference of the Unified Model 7.1 Theorectical Analysis VGM. World Model. IDM. VLA. Video-Action Joint Prediction Model. 7.2 Experimental Results VGM. World Model. IDM. Video-Action Joint Prediction Model. 8 More Experiments Results 8.1 Overall Comparison on RoboTwin 2.0 Simulation Data with More Baselines 8.2 Other Benchmarks LIBERO-Long. VLABench. 8.3 More Real-World Results 9 Implementation Details 9.1 Model Architecture 9.2 Datasets 9.3 Training Configuration Motus: A Unified Latent Action World Model Hongzhe Bi 1∗† , Hengkai Tan 1∗† , Shenghao Xie 2,1∗ , Zeyuan Wang 1∗ , Shuhe Huang 1∗ , Haitian Liu 1∗ , Ruowen Zhao 1 , Yao F…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[vla]]
- **Raw:** `raw/arxiv/2512.13030v2.md` · `raw/arxiv/2512.13030v2.fulltext.md`
