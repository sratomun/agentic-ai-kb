---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SoFar: Language-Grounded Orientation Bridges Spatial Reasoning and Object Manipulation"
authors: Zekun Qi, Wenyao Zhang, Yufei Ding, Runpei Dong et al.
url: https://arxiv.org/abs/2502.13143v2
date: 2025-02-18
citationCount: 51
influentialCitationCount: 3
velocity: 3.17
ingested: 2026-06-22
tags: [embodied-agents, arxiv, 2025, cited]
---

# SoFar: Language-Grounded Orientation Bridges Spatial Reasoning and Object Manipulation

**arXiv [2502.13143v2](https://arxiv.org/abs/2502.13143v2)** · 2025-02-18 · **51 citations** (3 influential · 3.17/mo) · Zekun Qi, Wenyao Zhang, Yufei Ding, Runpei Dong et al.

## Abstract
While spatial reasoning has made progress in object localization relationships, it often overlooks object orientation-a key factor in 6-DoF fine-grained manipulation. Traditional pose representations rely on pre-defined frames or templates, limiting generalization and semantic grounding. In this paper, we introduce the concept of semantic orientation, which defines object orientations using natural language in a reference-frame-free manner (e.g., the "plug-in" direction of a USB or the "handle" direction of a cup). To support this, we construct OrienText300K, a large-scale dataset of 3D objects annotated with semantic orientations, and develop PointSO, a general model for zero-shot semantic orientation prediction. By integrating semantic orientation into VLM agents, our SoFar framework enables 6-DoF spatial reasoning and generates robotic actions. Extensive experiments demonstrated the effectiveness and generalization of our SoFar, e.g., zero-shot 48.7% successful rate on Open6DOR and zero-shot 74.9% successful rate on SIMPLER-Env.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Semantic Orientation: Connecting Language and Object Orientation 2.1 Definition of Semantic Orientation 2.2 OrienText300K: Orientation-Text Paired Data at Scale 2.3 PointSO: A Cross-Modal 3D Transformer for Semantic Orientation Prediction 3 SoFar : Semantic Orientation Bridges Spatial Reasoning and Object Manipulation 3.1 Scene Graph with 6-DoF Information 3.2 Spatial-Aware Task Reasoning 4 Experiments 4.1 Real-world Language-Grounded Object Manipulation 4.2 Semantic Orientation Prediction 4.3 6-DoF Object Rearrangement Evaluation on Open6DOR V2 4.4 Simulation Object Manipulation Evaluation on SIMPLER [ 62 ] 4.5 Orientation-Aware Robotic Navigation 4.6 Spatial Reasoning Evaluation on 6-DoF SpatialBench 5 Limitations Conclusions A Robot Setups A.1 Simulation Robot Setups A.2 Real World Robot Setups B Additional Experiments B.1 Articulated Objects Manipulation Evaluation B.2 Spatial Reasoning on EmbSpatial-Bench [ 29 ] B.3 Cross Embodiment Generalization B.4 Long Horizon Object Manipulation Experiment B.…

**Method / approach.** method significantly outperforms state-of-the-art VLMs and VLA models—even those trained on expensive robot trajectories—across both simulated and real-world tasks. We also introduce 6-DoF SpatialBench, a new spatial visual-question-answering benchmark to rigorously assess orientation-aware reasoning. In summary, we propose Semantic Orientation as a new representation that bridges spatial reasoning and robotic manipulation, enabling open-vocabulary, template-free orientation understanding for unseen objects. We introduce OrienText300K , a large-scale dataset including 350K diverse objects orientations and 8M images through careful filtering and annotating. We develop the SoFar system, which enhances spatial reasoning with 6-DoF scene graph and achieves SOTA performance on Open6DOR, SimplerEnv, and generalizes across embodiments ( e.g. , grippers, suction cups, dexterous hands) and tasks ( e.g. , manipulation, navigation, VQA) without any task-specific fine-tuning. Finally, we prese…

**Results.** Experiments 4.1 Real-world Language-Grounded Object Manipulation 4.2 Semantic Orientation Prediction 4.3 6-DoF Object Rearrangement Evaluation on Open6DOR V2 4.4 Simulation Object Manipulation Evaluation on SIMPLER [ 62 ] 4.5 Orientation-Aware Robotic Navigation 4.6 Spatial Reasoning Evaluation on 6-DoF SpatialBench 5 Limitations Conclusions A Robot Setups A.1 Simulation Robot Setups A.2 Real World Robot Setups B Additional Experiments B.1 Articulated Objects Manipulation Evaluation B.2 Spatial Reasoning on EmbSpatial-Bench [ 29 ] B.3 Cross Embodiment Generalization B.4 Long Horizon Object Manipulation Experiment B.5 Close-Loop Execution Experiment B.6 In the Wild Evaluation of Semantic Orientation B.7 Cross-View Generalization B.8 Failure Case Distribution Analysis C Ablation Study C.1 Semantic Orientation Ablation C.2 Scaling Law C.3 Cross-Modal Fusion Choices C.4 Open Voc…

**Conclusion.** Conclusions A Robot Setups A.1 Simulation Robot Setups A.2 Real World Robot Setups B Additional Experiments B.1 Articulated Objects Manipulation Evaluation B.2 Spatial Reasoning on EmbSpatial-Bench [ 29 ] B.3 Cross Embodiment Generalization B.4 Long Horizon Object Manipulation Experiment B.5 Close-Loop Execution Experiment B.6 In the Wild Evaluation of Semantic Orientation B.7 Cross-View Generalization B.8 Failure Case Distribution Analysis C Ablation Study C.1 Semantic Orientation Ablation C.2 Scaling Law C.3 Cross-Modal Fusion Choices C.4 Open Vocabulary Object Detection Module D Additional Implementation Details D.1 Detail Real World Experiment Results D.2 PointSO Model Details D.3…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]]
- **Raw:** `raw/arxiv/2502.13143v2.md` · `raw/arxiv/2502.13143v2.fulltext.md`
