---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Point Policy: Unifying Observations and Actions with Key Points for Robot Manipulation"
authors: Siddhant Haldar, Lerrel Pinto
url: https://arxiv.org/abs/2502.20391v1
date: 2025-02-27
citationCount: 54
influentialCitationCount: 12
velocity: 3.42
ingested: 2026-06-22
tags: [embodied-agents, arxiv, 2025, cited]
---

# Point Policy: Unifying Observations and Actions with Key Points for Robot Manipulation

**arXiv [2502.20391v1](https://arxiv.org/abs/2502.20391v1)** · 2025-02-27 · **54 citations** (12 influential · 3.42/mo) · Siddhant Haldar, Lerrel Pinto

## Abstract
Building robotic agents capable of operating across diverse environments and object types remains a significant challenge, often requiring extensive data collection. This is particularly restrictive in robotics, where each data point must be physically executed in the real world. Consequently, there is a critical need for alternative data sources for robotics and frameworks that enable learning from such data. In this work, we present Point Policy, a new method for learning robot policies exclusively from offline human demonstration videos and without any teleoperation data. Point Policy leverages state-of-the-art vision models and policy architectures to translate human hand poses into robot poses while capturing object states through semantically meaningful key points. This approach yields a morphology-agnostic representation that facilitates effective policy learning. Our experiments on 8 real-world tasks demonstrate an overall 75% absolute improvement over prior works when evaluated in identical settings as training. Further, Point Policy exhibits a 74% gain across tasks for novel object instances and is robust to significant background clutter. Videos of the robot are best viewed at https://point-policy.github.io/.

## From the paper (full-text excerpts)
**Introduction.** Introduction II Related Works II-A Imitation Learning II-B Object-centric Representation Learning II-C Human-to-Robot Transfer for Policy Learning III Background III-A Imitation learning III-B Behavior Cloning III-C Semantic Correspondence and Point Tracking IV Point Policy IV-A Point-based Scene Representation IV-A 1 Human-to-Robot Pose Transfer IV-A 2 Environment state through point priors IV-B Policy Learning IV-C Backtrack Robot Actions from Predicted Key Points V Experiments V-A Experimental Setup V-B Task Descriptions Close drawer Put bread on plate Fold towel Close oven Sweep broom Put bottle on rack Put bowl in oven Make bottle upright V-C Baselines Behavior Cloning (BC) [ 28 ] Behavior Cloning (BC) with Depth Motion Track Policy (MT- π 𝜋 \pi italic_π ) [ 67 ] P3-PO [ 45 ] V-D Considerations for policy learning V-E How well does Point Policy work for policy learning? V-F How well does Point Policy work for novel object instances? V-G Can Point Policy handle background distractor…

**Method / approach.** method for learning robot policies exclusively from offline human demonstration videos and without any teleoperation data. Point Policy leverages state-of-the-art vision models and policy architectures to translate human hand poses into robot poses while capturing object states through semantically meaningful key points. This approach yields a morphology-agnostic representation that facilitates effective policy learning. Our experiments on 8 real-world tasks demonstrate an overall 75% absolute improvement over prior works when evaluated in identical settings as training. Further, Point Policy exhibits a 74% gain across tasks for novel object instances and is robust to significant background clutter. Videos of the robot are best viewed at point-policy.github.io . I Introduction Recent years have witnessed remarkable advancements in computer vision (CV) and natural language processing (NLP), resulting in models capable of complex reasoning [ 2 , 66 , 76 ] , generating photorealis…

**Results.** Experiments V-A Experimental Setup V-B Task Descriptions Close drawer Put bread on plate Fold towel Close oven Sweep broom Put bottle on rack Put bowl in oven Make bottle upright V-C Baselines Behavior Cloning (BC) [ 28 ] Behavior Cloning (BC) with Depth Motion Track Policy (MT- π 𝜋 \pi italic_π ) [ 67 ] P3-PO [ 45 ] V-D Considerations for policy learning V-E How well does Point Policy work for policy learning? V-F How well does Point Policy work for novel object instances? V-G Can Point Policy handle background distractors? V-H Can Point Policy be improved with robot demonstrations? V-I What design choices matter for human-to-robot learning? Depth Sensing Significance of Object Points VI Conclusion and Limitations VII Acknowledgments -A Background -A 1 Semantic Correspondence -A 2 Point Tracking -B Algorithmic Details -B 1 Point Triangulation…

**Conclusion.** Conclusion and Limitations VII Acknowledgments -A Background -A 1 Semantic Correspondence -A 2 Point Tracking -B Algorithmic Details -B 1 Point Triangulation -C Hyperparameters -D Implementation Details for MT- π 𝜋 \pi italic_π -E Experiments -E 1 Illustration of Spatial Generalization and Novel Object Instances -E 2 Illustration of Depth Discrepancy -E 3 Significance of Object Points \useunder \ul Point Policy: Unifying Observations and Actions with Key Points for Robot Manipulation Siddhant Haldar Lerrel Pinto New York University point-policy.github.io Correspondence to: siddhanthaldar@nyu.edu Abstract Building robotic agents capable of operating across diverse environments an…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]]
- **Raw:** `raw/arxiv/2502.20391v1.md` · `raw/arxiv/2502.20391v1.fulltext.md`
