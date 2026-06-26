---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Group-in-Group Policy Optimization for LLM Agent Training"
authors: Lang Feng, Zhenghai Xue, Tingcong Liu, Bo An
url: https://arxiv.org/abs/2505.10978v3
date: 2025-05-16
citationCount: 268
influentialCitationCount: 65
velocity: 20.29
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Group-in-Group Policy Optimization for LLM Agent Training

**arXiv [2505.10978v3](https://arxiv.org/abs/2505.10978v3)** · 2025-05-16 · **268 citations** (65 influential · 20.29/mo) · Lang Feng, Zhenghai Xue, Tingcong Liu, Bo An

## Abstract
Recent advances in group-based reinforcement learning (RL) have driven frontier large language models (LLMs) in single-turn tasks like mathematical reasoning. However, their scalability to multi-turn LLM agent training remains limited. Unlike static tasks, agent-environment interactions unfold over many steps and often yield sparse or delayed rewards, making credit assignment across individual steps significantly more challenging. In this work, we propose Group-in-Group Policy Optimization (GiGPO), a novel RL algorithm that achieves fine-grained credit assignment for LLM agents while preserving the appealing properties of group-based RL: critic-free, low memory, and stable convergence. GiGPO introduces a two-level structure for estimating relative advantage: (i) At the episode-level, GiGPO computes macro relative advantages based on groups of complete trajectories; (ii) At the step-level, GiGPO introduces an anchor state grouping mechanism that retroactively constructs step-level groups by identifying repeated environment states across trajectories. Actions stemming from the same state are grouped together, enabling micro relative advantage estimation. This hierarchical structure effectively captures both global trajectory quality and local step effectiveness without relying on auxiliary models or additional rollouts. We evaluate GiGPO on challenging agent benchmarks, including ALFWorld and WebShop, as well as tool-integrated reasoning on search-augmented QA tasks, using Qwen2.5-1.5B/3B/7B-Instruct. Crucially, GiGPO delivers fine-grained per-step credit signals, achieves performance gains of > 12% on ALFWorld and > 9% on WebShop over GRPO, and obtains superior performance on QA tasks (42.1% on 3B and 47.2% on 7B): all while maintaining the same GPU memory overhead, identical LLM rollout, and incurring little to no additional time cost.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Preliminaries 4 Training LLM Agents with GiGPO 4.1 Episode Relative Advantages 4.2 Step Relative Advantages 4.3 Group-in-Group Policy Optimization 5 Experiment 5.1 Experiment Setup 5.2 Performance on ALFWorld and WebShop 5.3 Performance on QA tasks 5.4 Ablation Study 5.5 Dynamics of Step-Level Group 5.6 Computational Budget 6 Conclusions and Limitations A Open Source Codebase: verl-agent B Broader Impacts C Unbiasedness D Pseudo Code E Experiment Details E.1 Details of Training E.2 Prompts E.3 Performance on Vision-Language Agents E.4 Orthogonality to Single-Turn Group-Based RL E.5 Sensitivity Analysis on ω \omega F Reasoning Behavior F.1 ALFWorld F.2 WebShop F.3 Search Group-in-Group Policy Optimization for LLM Agent Training Lang Feng 1 Zhenghai Xue 1 Tingcong Liu 1 Bo An 1,2, 1 Nanyang Technological University, Singapore 2 Skywork AI, Singapore {lang005,zhenghai001,tingcong001}@e.ntu.edu.sg, boan@ntu.edu.sg Corresponding author Abstract Recent advances in…

**Method / approach.** methods replace value-function estimation with simple yet powerful relative advantage estimation within groups of rollouts. This group-based advantage computation enjoys favorable properties such as low memory overhead, critic-free optimization, and scalability to large models. However, their successes have so far been largely limited to single-turn tasks such as math problem solving liu2025understanding ; yu2025dapo and code generation wei2025swe , where reward arrives immediately and credit assignment is straightforward. In contrast, LLM agents operating in external environments face fundamentally different learning landscapes. Their behavior unfolds over long episodes with tens of decision steps and tens of thousands of tokens (e.g., an ALFWorld shridhar2020alfworld episode may include up to 50 steps and over 20k tokens). Rewards are typically sparse (sometimes arriving only at the end of an episode), and the impact of any individual action may only manifest much later in the…

**Results.** Experiment 5.1 Experiment Setup 5.2 Performance on ALFWorld and WebShop 5.3 Performance on QA tasks 5.4 Ablation Study 5.5 Dynamics of Step-Level Group 5.6 Computational Budget 6 Conclusions and Limitations A Open Source Codebase: verl-agent B Broader Impacts C Unbiasedness D Pseudo Code E Experiment Details E.1 Details of Training E.2 Prompts E.3 Performance on Vision-Language Agents E.4 Orthogonality to Single-Turn Group-Based RL E.5 Sensitivity Analysis on ω \omega F Reasoning Behavior F.1 ALFWorld F.2 WebShop F.3 Search Group-in-Group Policy Optimization for LLM Agent Training Lang Feng 1 Zhenghai Xue 1 Tingcong Liu 1 Bo An 1,2, 1 Nanyang Technological University, Singapore 2 Skywork AI, Singapore {lang005,zhenghai001,tingcong001}@e.ntu.edu.sg, boan@ntu.edu.sg Corresponding author Abstract Recent advances in group-based reinforcement learning (RL) have dri…

**Conclusion.** Conclusions and Limitations A Open Source Codebase: verl-agent B Broader Impacts C Unbiasedness D Pseudo Code E Experiment Details E.1 Details of Training E.2 Prompts E.3 Performance on Vision-Language Agents E.4 Orthogonality to Single-Turn Group-Based RL E.5 Sensitivity Analysis on ω \omega F Reasoning Behavior F.1 ALFWorld F.2 WebShop F.3 Search Group-in-Group Policy Optimization for LLM Agent Training Lang Feng 1 Zhenghai Xue 1 Tingcong Liu 1 Bo An 1,2, 1 Nanyang Technological University, Singapore 2 Skywork AI, Singapore {lang005,zhenghai001,tingcong001}@e.ntu.edu.sg, boan@ntu.edu.sg Corresponding author Abstract Recent advances in group-based reinforcement learning (RL) have…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[alfworld]] · [[qwen]]
- **Raw:** `raw/arxiv/2505.10978v3.md` · `raw/arxiv/2505.10978v3.fulltext.md`
