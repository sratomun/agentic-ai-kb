---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning"
authors: Chi-Pin Huang, Yueh-Hua Wu, Min-Hung Chen, Yu-Chiang Frank Wang et al.
url: https://arxiv.org/abs/2507.16815v2
date: 2025-07-22
citationCount: 125
influentialCitationCount: 15
velocity: 11.36
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning

**arXiv [2507.16815v2](https://arxiv.org/abs/2507.16815v2)** · 2025-07-22 · **125 citations** (15 influential · 11.36/mo) · Chi-Pin Huang, Yueh-Hua Wu, Min-Hung Chen, Yu-Chiang Frank Wang et al.

## Abstract
Vision-language-action (VLA) reasoning tasks require agents to interpret multimodal instructions, perform long-horizon planning, and act adaptively in dynamic environments. Existing approaches typically train VLA models in an end-to-end fashion, directly mapping inputs to actions without explicit reasoning, which hinders their ability to plan over multiple steps or adapt to complex task variations. In this paper, we propose ThinkAct, a dual-system framework that bridges high-level reasoning with low-level action execution via reinforced visual latent planning. ThinkAct trains a multimodal LLM to generate embodied reasoning plans guided by reinforcing action-aligned visual rewards based on goal completion and trajectory consistency. These reasoning plans are compressed into a visual plan latent that conditions a downstream action model for robust action execution on target environments. Extensive experiments on embodied reasoning and robot manipulation benchmarks demonstrate that ThinkAct enables few-shot adaptation, long-horizon planning, and self-correction behaviors in complex embodied AI tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Vision-Language-Action Models 2.2 Reasoning in Vision-Language-(Action) Models 3 Method 3.1 Problem Formulation 3.2 Reinforced Visual Latent Planning for Embodied Reasoning Reward Shaping from Action-Aligned Visual Feedback Reinforced Fine-Tuning for Eliciting Visual Latent Planning 3.3 Reasoning-Enhanced Action Adaptation 3.4 Learning Strategy and Inference 4 Experiment 4.1 Experimental Setup Implementation Details Training Datasets and Evaluation Benchmarks 4.2 Quantitative Evaluation Robot Manipulation Embodied Reasoning 4.3 Qualitative Results 4.4 Ablation Study 4.5 Analysis of ThinkAct Reasoning Enhance Few-Shot Adaptation Reasoning Elicit Self-Correction 5 Conclusion Limitations Broader Impacts A Additional Experimental Setup A.1 Implementation Details Reinforced Fine-Tuning for Eliciting Visual Latent Planning Reasoning-Enhanced Action Adaptation A.2 Training Data Preparation A.2.1 Training Datasets 2D Trajectory of Manipulation RoboVQA Sermanet…

**Method / approach.** Method 3.1 Problem Formulation 3.2 Reinforced Visual Latent Planning for Embodied Reasoning Reward Shaping from Action-Aligned Visual Feedback Reinforced Fine-Tuning for Eliciting Visual Latent Planning 3.3 Reasoning-Enhanced Action Adaptation 3.4 Learning Strategy and Inference 4 Experiment 4.1 Experimental Setup Implementation Details Training Datasets and Evaluation Benchmarks 4.2 Quantitative Evaluation Robot Manipulation Embodied Reasoning 4.3 Qualitative Results 4.4 Ablation Study 4.5 Analysis of ThinkAct Reasoning Enhance Few-Shot Adaptation Reasoning Elicit Self-Correction 5 Conclusion Limitations Broader Impacts A Additional Experimental Setup A.1 Implementation Details Reinforced Fine-Tuning for Eliciting Visual Latent Planning Reasoning-Enhanced Action Adaptation A.2 Training Data Preparation A.2.1 Training Datasets 2D Trajectory of Manipulation RoboVQA Sermanet et al. ( 2024 ) Reflect…

**Results.** Experiment 4.1 Experimental Setup Implementation Details Training Datasets and Evaluation Benchmarks 4.2 Quantitative Evaluation Robot Manipulation Embodied Reasoning 4.3 Qualitative Results 4.4 Ablation Study 4.5 Analysis of ThinkAct Reasoning Enhance Few-Shot Adaptation Reasoning Elicit Self-Correction 5 Conclusion Limitations Broader Impacts A Additional Experimental Setup A.1 Implementation Details Reinforced Fine-Tuning for Eliciting Visual Latent Planning Reasoning-Enhanced Action Adaptation A.2 Training Data Preparation A.2.1 Training Datasets 2D Trajectory of Manipulation RoboVQA Sermanet et al. ( 2024 ) Reflect (RoboFail) Liu et al. ( 2023c ) EgoPlan-Bench Chen et al. ( 2023 ) Video-R1-CoT Feng et al. ( 2025 ) LLaVA-Video-178K Zhang et al. ( 2024 ) A.2.2 Training Data Construction Supervised Fine-Tuning for Cold Start Reinforced Fine-Tuning for E…

**Conclusion.** Conclusion Limitations Broader Impacts A Additional Experimental Setup A.1 Implementation Details Reinforced Fine-Tuning for Eliciting Visual Latent Planning Reasoning-Enhanced Action Adaptation A.2 Training Data Preparation A.2.1 Training Datasets 2D Trajectory of Manipulation RoboVQA Sermanet et al. ( 2024 ) Reflect (RoboFail) Liu et al. ( 2023c ) EgoPlan-Bench Chen et al. ( 2023 ) Video-R1-CoT Feng et al. ( 2025 ) LLaVA-Video-178K Zhang et al. ( 2024 ) A.2.2 Training Data Construction Supervised Fine-Tuning for Cold Start Reinforced Fine-Tuning for Eliciting Visual Latent Planning A.3 Evaluation Benchmarks SimplerEnv Li et al. ( 2024c ) LIBERO Liu et al. ( 2023a ) EgoPlan-Bench2 Q…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[vla]]
- **Raw:** `raw/arxiv/2507.16815v2.md` · `raw/arxiv/2507.16815v2.fulltext.md`
