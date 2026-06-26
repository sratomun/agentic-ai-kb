---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey of Automatic Prompt Engineering: An Optimization Perspective"
authors: Wenwu Li, Xiangfeng Wang, Wenhao Li, Bo Jin
url: https://arxiv.org/abs/2502.11560v1
date: 2025-02-17
citationCount: 53
influentialCitationCount: 5
velocity: 3.29
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# A Survey of Automatic Prompt Engineering: An Optimization Perspective

**arXiv [2502.11560v1](https://arxiv.org/abs/2502.11560v1)** · 2025-02-17 · **53 citations** (5 influential · 3.29/mo) · Wenwu Li, Xiangfeng Wang, Wenhao Li, Bo Jin

## Abstract
The rise of foundation models has shifted focus from resource-intensive fine-tuning to prompt engineering, a paradigm that steers model behavior through input design rather than weight updates. While manual prompt engineering faces limitations in scalability, adaptability, and cross-modal alignment, automated methods, spanning foundation model (FM) based optimization, evolutionary methods, gradient-based optimization, and reinforcement learning, offer promising solutions. Existing surveys, however, remain fragmented across modalities and methodologies. This paper presents the first comprehensive survey on automated prompt engineering through a unified optimization-theoretic lens. We formalize prompt optimization as a maximization problem over discrete, continuous, and hybrid prompt spaces, systematically organizing methods by their optimization variables (instructions, soft prompts, exemplars), task-specific objectives, and computational frameworks. By bridging theoretical formulation with practical implementations across text, vision, and multimodal domains, this survey establishes a foundational framework for both researchers and practitioners, while highlighting underexplored frontiers in constrained optimization and agent-oriented prompt design.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Optimization Problem Formulation 4 Optimization Spaces 4.1 Discrete Variables Instructions Thoughts Few-shot Examples Annotations 4.2 Continuous Variables 4.3 Mixed Variables 5 Objective Functions 5.1 Downstream Tasks Instruction Induction. Text Classification. Math Reasoning. Commonsense Reasoning. Multi-Hop Reasoning. Domain-Specific Tasks. Multimodal Tasks. 5.2 Constrained Objectives 6 Optimization Methods 6.1 FM-based Optimization Heuristic Meta-Prompt Automatic Meta-Prompt Generation Strategic Search and Replanning 6.2 Evolutionary Computing Genetic Operators and Heuristics Self-Referential Evolution 6.3 Gradient-Based Optimization Discrete Token Gradient Methods Soft Prompt Tuning 6.4 Reinforcement Learning Prompt Editing as RL Actions Multi-Objective and Inverse RL Strategies 7 Future Directions Constraint optimization Multi-task prompt optimization Online prompt optimization Multi-objective prompt optimization Heterogeneous modality optimiza…

**Method / approach.** Methods 6.1 FM-based Optimization Heuristic Meta-Prompt Automatic Meta-Prompt Generation Strategic Search and Replanning 6.2 Evolutionary Computing Genetic Operators and Heuristics Self-Referential Evolution 6.3 Gradient-Based Optimization Discrete Token Gradient Methods Soft Prompt Tuning 6.4 Reinforcement Learning Prompt Editing as RL Actions Multi-Objective and Inverse RL Strategies 7 Future Directions Constraint optimization Multi-task prompt optimization Online prompt optimization Multi-objective prompt optimization Heterogeneous modality optimization Bi-level prompt optimization Broader application scenarios 8 Discussion and Conclusion A Survey of Automatic Prompt Engineering: An Optimization Perspective Wenwu Li School of Computer Science and Technology, Tongji University Xiangfeng Wang Key Laboratory of Mathematics and Engineering Applications, MoE, East China Normal University School of Computer Scie…

**Results.** Evaluation relies on comparing numeric outputs or perplexity. Commonsense Reasoning. Models must incorporate external, everyday knowledge to answer or infer implicit context. Tasks like CommonsenseQA [ THLB19 ] , and StrategyQA [ GKS + 21 ] evaluate f ⁢ ( P ⁢ ( x ) ) 𝑓 𝑃 𝑥 f\bigl{(}P(x)\bigr{)} italic_f ( italic_P ( italic_x ) ) for multi-step common-sense inferences. Exact match are typical performance metrics. Multi-Hop Reasoning. Extending beyond single-step inferences, multi-hop tasks demand chaining evidence from multiple sources. BBH [ SSS + 23 ] exemplifies this domain. The key objective is again max ⁡ 𝔼 ⁢ [ g ⁢ ( ⋅ ) ] 𝔼 delimited-[] 𝑔 ⋅ \max\mathbb{E}[g(\cdot)] roman_max blackboard_E [ italic_g ( ⋅ ) ] over correctness but with specialized intermediate-step or CoT evaluations. Domain-Specific Tasks. Focus on specialized areas demanding expert-level knowledge, e.g., biomedical tasks in MedQA [ JPO + 21 ]…

**Conclusion.** Conclusion A Survey of Automatic Prompt Engineering: An Optimization Perspective Wenwu Li School of Computer Science and Technology, Tongji University Xiangfeng Wang Key Laboratory of Mathematics and Engineering Applications, MoE, East China Normal University School of Computer Science and Technology, East China Normal University Wenhao Li whli@tongji.edu.cn School of Computer Science and Technology, Tongji University Bo Jin bjin@tongji.edu.cn Shanghai Research Institute for Intelligent Autonomous Systems, Tongji University School of Computer Science and Technology, Tongji University Abstract The rise of foundation models has shifted focus from resource-intensive fine-tuning to prompt engineering, a paradig…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.11560v1.md` · `raw/arxiv/2502.11560v1.fulltext.md`
