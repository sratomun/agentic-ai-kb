---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OmniRetarget: Interaction-Preserving Data Generation for Humanoid Whole-Body Loco-Manipulation and Scene Interaction"
authors: Lujie Yang, Xiaoyu Huang, Zhen Wu, Angjoo Kanazawa et al.
url: https://arxiv.org/abs/2509.26633v3
date: 2025-09-30
citationCount: 81
influentialCitationCount: 11
velocity: 9.3
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agent-skills, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# OmniRetarget: Interaction-Preserving Data Generation for Humanoid Whole-Body Loco-Manipulation and Scene Interaction

**arXiv [2509.26633v3](https://arxiv.org/abs/2509.26633v3)** · 2025-09-30 · **81 citations** (11 influential · 9.3/mo) · Lujie Yang, Xiaoyu Huang, Zhen Wu, Angjoo Kanazawa et al.

## Abstract
A dominant paradigm for teaching humanoid robots complex skills is to retarget human motions as kinematic references to train reinforcement learning (RL) policies. However, existing retargeting pipelines often struggle with the significant embodiment gap between humans and robots, producing physically implausible artifacts like foot-skating and penetration. More importantly, common retargeting methods neglect the rich human-object and human-environment interactions essential for expressive locomotion and loco-manipulation. To address this, we introduce OmniRetarget, an interaction-preserving data generation engine based on an interaction mesh that explicitly models and preserves the crucial spatial and contact relationships between an agent, the terrain, and manipulated objects. By minimizing the Laplacian deformation between the human and robot meshes while enforcing kinematic constraints, OmniRetarget generates kinematically feasible trajectories. Moreover, preserving task-relevant interactions enables efficient data augmentation, from a single demonstration to different robot embodiments, terrains, and object configurations. We comprehensively evaluate OmniRetarget by retargeting motions from OMOMO, LAFAN1, and our in-house MoCap datasets, generating over 8-hour trajectories that achieve better kinematic constraint satisfaction and contact preservation than widely used baselines. Such high-quality data enables proprioceptive RL policies to successfully execute long-horizon (up to 30 seconds) parkour and loco-manipulation skills on a Unitree G1 humanoid, trained with only 5 reward terms and simple domain randomization shared by all tasks, without any learning curriculum.

## From the paper (full-text excerpts)
**Introduction.** Introduction II Related Works II-A Motion Retargeting II-B Learning-Based Humanoid Whole-Body Control II-C Data Generation for Humanoid Loco-Manipulation III Interaction-Preserving Motion Retargeting III-A Interaction Mesh with Hard Constraints III-B Terrain, Object Shape and Spatial Augmentation IV RL Training with Minimal Formulation V Experimental Results V-A Whole-Body Scene-Object-Interaction Agile Loco-Manipulation Sim-to-real with Augmented Data V-B Benchmark Against Prior Retargeting Pipelines Kinematics Quality Downstream RL Performance VI Conclusion References VI-A Different Sources of Human Motion Data VI-A 1 SMPL Data Model Fitting (PHC, VideoMimic) Direct Scaling (GMR OmniRetarget ) VI-A 2 Skeleton Hierarchy Data VI-B Different Kinematic Retargeting Formulations VI-B 1 PHC VI-B 2 GMR VI-B 3 VideoMimic VI-B 4 IMMA Multi-stage Optimization VI-B 5 OmniRetarget VI-C Data Augmentation Details VI-C 1 Augmented Object Trajectory VI-C 2 Interaction Mesh Construction in Object Frame VI-D…

**Method / approach.** methods neglect the rich human-object and human-environment interactions essential for expressive locomotion and loco-manipulation. To address this, we introduce OmniRetarget , an interaction-preserving data generation engine based on an interaction mesh that explicitly models and preserves the crucial spatial and contact relationships between an agent, the terrain, and manipulated objects. By minimizing the Laplacian deformation between the human and robot meshes while enforcing kinematic constraints, OmniRetarget generates kinematically feasible trajectories. Moreover, preserving task-relevant interactions enables efficient data augmentation, from a single demonstration to different robot embodiments, terrains, and object configurations. We comprehensively evaluate OmniRetarget by retargeting motions from OMOMO [ 1 ] , LAFAN1 [ 2 ] , and our in-house MoCap datasets, generating over 8-hour trajectories that achieve better kinematic constraint satisfaction and contact preservation tha…

**Results.** Experimental Results V-A Whole-Body Scene-Object-Interaction Agile Loco-Manipulation Sim-to-real with Augmented Data V-B Benchmark Against Prior Retargeting Pipelines Kinematics Quality Downstream RL Performance VI Conclusion References VI-A Different Sources of Human Motion Data VI-A 1 SMPL Data Model Fitting (PHC, VideoMimic) Direct Scaling (GMR OmniRetarget ) VI-A 2 Skeleton Hierarchy Data VI-B Different Kinematic Retargeting Formulations VI-B 1 PHC VI-B 2 GMR VI-B 3 VideoMimic VI-B 4 IMMA Multi-stage Optimization VI-B 5 OmniRetarget VI-C Data Augmentation Details VI-C 1 Augmented Object Trajectory VI-C 2 Interaction Mesh Construction in Object Frame VI-D Sequential SOCP Details VI-E Downstream RL Evaluation Breakdown License: CC BY 4.0 arXiv:2509.26633v3 [cs.RO] 15 Jun 2026 OmniRetarget: Interaction-Preserving Data Generation for Humanoid Whole-Body Loco-Mani…

**Conclusion.** Conclusion References VI-A Different Sources of Human Motion Data VI-A 1 SMPL Data Model Fitting (PHC, VideoMimic) Direct Scaling (GMR OmniRetarget ) VI-A 2 Skeleton Hierarchy Data VI-B Different Kinematic Retargeting Formulations VI-B 1 PHC VI-B 2 GMR VI-B 3 VideoMimic VI-B 4 IMMA Multi-stage Optimization VI-B 5 OmniRetarget VI-C Data Augmentation Details VI-C 1 Augmented Object Trajectory VI-C 2 Interaction Mesh Construction in Object Frame VI-D Sequential SOCP Details VI-E Downstream RL Evaluation Breakdown License: CC BY 4.0 arXiv:2509.26633v3 [cs.RO] 15 Jun 2026 OmniRetarget: Interaction-Preserving Data Generation for Humanoid Whole-Body Loco-Manipulation and Scene Interaction Luj…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.26633v3.md` · `raw/arxiv/2509.26633v3.fulltext.md`
