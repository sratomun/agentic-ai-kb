---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "VAGEN: Reinforcing World Model Reasoning for Multi-Turn VLM Agents"
authors: Kangrui Wang, Pingyue Zhang, Zihan Wang, Yaning Gao et al.
url: https://arxiv.org/abs/2510.16907v1
date: 2025-10-19
citationCount: 45
influentialCitationCount: 2
velocity: 5.57
ingested: 2026-06-22
tags: [embodied-agents, agent-reliability, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# VAGEN: Reinforcing World Model Reasoning for Multi-Turn VLM Agents

**arXiv [2510.16907v1](https://arxiv.org/abs/2510.16907v1)** · 2025-10-19 · **45 citations** (2 influential · 5.57/mo) · Kangrui Wang, Pingyue Zhang, Zihan Wang, Yaning Gao et al.

## Abstract
A key challenge in training Vision-Language Model (VLM) agents, compared to Language Model (LLM) agents, lies in the shift from textual states to complex visual observations. This transition introduces partial observability and demands robust world modeling. We ask: Can VLM agents construct internal world models through explicit visual state reasoning? To address this question, we architecturally enforce and reward the agent's reasoning process via reinforcement learning (RL), formulating it as a Partially Observable Markov Decision Process (POMDP). We find that decomposing the agent's reasoning into State Estimation ("what is the current state?") and Transition Modeling ("what comes next?") is critical for success, as demonstrated through five reasoning strategies. Our investigation into how agents represent internal beliefs reveals that the optimal representation is task-dependent: Natural Language excels at capturing semantic relationships in general tasks, while Structured formats are indispensable for precise manipulation and control. Building on these insights, we design a World Modeling Reward that provides dense, turn-level supervision for accurate state prediction, and introduce Bi-Level General Advantage Estimation (Bi-Level GAE) for turn-aware credit assignment. Through this form of visual state reasoning, a 3B-parameter model achieves a score of 0.82 across five diverse agent benchmarks, representing a 3$\times$ improvement over its untrained counterpart (0.21) and outperforming proprietary reasoning models such as GPT-5 (0.75), Gemini 2.5 Pro (0.67) and Claude 4.5 (0.62). All experiments are conducted within our VAGEN framework, a scalable system for training and analyzing multi-turn VLM agents in diverse visual environments. Code and data are publicly available at https://vagen-ai.github.io.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Build Internal World Models via Visual State Reasoning in Multi-Turn RL 2.1 Problem Formulation 2.2 Visual State Reasoning as an Internal World Model Reasoning Trajectory Rollout for Multi-Turn VLM Agents. Visual State Reasoning as World Modeling. Policy Optimization. Advantage and Value Estimation. 2.3 Reward Design in Different Environments and Tasks for VLM Agents Reward Strategy and Metrics. 2.4 What Can We Reason About Visual States? Off-the-Shelf VLMs struggle to solve multi-turn agentic tasks. World Modeling can improve visual reasoning via multi-turn RL. Existing RL methods are inadequate for multi-turn VLM agents. 3 How Can We Represent Internal Beliefs about the World? Results and Insights. 4 Can World Modeling Help with Reward Shaping and Credit Assignment? 4.1 WorldModeling Reward 4.2 Bi-Level General Advantage Estimation (GAE) 4.3 VAGEN-Full Multi-Turn Reinforcement Learning Framework Experiment Setup. Results and Insights. 4.4 Ablations 4.5 Case Studies and Findings Enhanced Spat…

**Method / approach.** methods are inadequate for multi-turn VLM agents. 3 How Can We Represent Internal Beliefs about the World? Results and Insights. 4 Can World Modeling Help with Reward Shaping and Credit Assignment? 4.1 WorldModeling Reward 4.2 Bi-Level General Advantage Estimation (GAE) 4.3 VAGEN-Full Multi-Turn Reinforcement Learning Framework Experiment Setup. Results and Insights. 4.4 Ablations 4.5 Case Studies and Findings Enhanced Spatial Understanding and Planning. Response Convergence and Reduced Exploration. Reward Hacking and Over-optimization. 5 Related Work RL for LLMs and VLMs. Multi-turn Agent Training for LLMs and VLMs. World Model Reasoning and Visual State Reasoning. 6 Conclusion and Limitations Appendix A World Modeling for Visual State Reasoning via Multi-Turn RL A.1 Problem Formulation: VLM Agent Training under a POMDP Formulation Inherent Partial Observability in Environments. Methodological Congruence with POMD…

**Results.** Experiment Setup. Results and Insights. 4.4 Ablations 4.5 Case Studies and Findings Enhanced Spatial Understanding and Planning. Response Convergence and Reduced Exploration. Reward Hacking and Over-optimization. 5 Related Work RL for LLMs and VLMs. Multi-turn Agent Training for LLMs and VLMs. World Model Reasoning and Visual State Reasoning. 6 Conclusion and Limitations Appendix A World Modeling for Visual State Reasoning via Multi-Turn RL A.1 Problem Formulation: VLM Agent Training under a POMDP Formulation Inherent Partial Observability in Environments. Methodological Congruence with POMDPs. A.2 Multi-Turn Reinforcement Learning in VLM Agentic Tasks A.3 VAGEN Framework A.4 Environments and Tasks for VLM Agents Sokoban FrozenLake Navigation PrimitiveSkill SVG Reconstruction A.5 Reward Assignment Sokoban FrozenLake Navigation PrimitiveSkill SVG A.6 Ev…

**Conclusion.** Conclusion and Limitations Appendix A World Modeling for Visual State Reasoning via Multi-Turn RL A.1 Problem Formulation: VLM Agent Training under a POMDP Formulation Inherent Partial Observability in Environments. Methodological Congruence with POMDPs. A.2 Multi-Turn Reinforcement Learning in VLM Agentic Tasks A.3 VAGEN Framework A.4 Environments and Tasks for VLM Agents Sokoban FrozenLake Navigation PrimitiveSkill SVG Reconstruction A.5 Reward Assignment Sokoban FrozenLake Navigation PrimitiveSkill SVG A.6 Evaluation Metrics Metrics for Task-Completion Environments Metrics for SVG Reconstruction B What Can We Reason About Visual States? B.1 Bottleneck of Off-the-Shelf VLM…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2510.16907v1.md` · `raw/arxiv/2510.16907v1.fulltext.md`
