---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mobile-Agent-v3: Fundamental Agents for GUI Automation"
authors: Jiabo Ye, Xi Zhang, Haiyang Xu, Haowei Liu et al.
url: https://arxiv.org/abs/2508.15144v2
date: 2025-08-21
citationCount: 124
influentialCitationCount: 12
velocity: 12.38
ingested: 2026-06-22
tags: [computer-use-agents, self-evolving-agents, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# Mobile-Agent-v3: Fundamental Agents for GUI Automation

**arXiv [2508.15144v2](https://arxiv.org/abs/2508.15144v2)** · 2025-08-21 · **124 citations** (12 influential · 12.38/mo) · Jiabo Ye, Xi Zhang, Haiyang Xu, Haowei Liu et al.

## Abstract
This paper introduces GUI-Owl, a foundational GUI agent model that achieves state-of-the-art performance among open-source end-to-end models on ten GUI benchmarks across desktop and mobile environments, covering grounding, question answering, planning, decision-making, and procedural knowledge. GUI-Owl-7B achieves 66.4 on AndroidWorld and 29.4 on OSWorld. Building on this, we propose Mobile-Agent-v3, a general-purpose GUI agent framework that further improves performance to 73.3 on AndroidWorld and 37.7 on OSWorld, setting a new state-of-the-art for open-source GUI agent frameworks. GUI-Owl incorporates three key innovations: (1) Large-scale Environment Infrastructure: a cloud-based virtual environment spanning Android, Ubuntu, macOS, and Windows, enabling our Self-Evolving GUI Trajectory Production framework. This generates high-quality interaction data via automated query generation and correctness validation, leveraging GUI-Owl to refine trajectories iteratively, forming a self-improving loop. It supports diverse data pipelines and reduces manual annotation. (2) Diverse Foundational Agent Capabilities: by integrating UI grounding, planning, action semantics, and reasoning patterns, GUI-Owl supports end-to-end decision-making and can act as a modular component in multi-agent systems. (3) Scalable Environment RL: we develop a scalable reinforcement learning framework with fully asynchronous training for real-world alignment. We also introduce Trajectory-aware Relative Policy Optimization (TRPO) for online RL, achieving 34.9 on OSWorld. GUI-Owl and Mobile-Agent-v3 are open-sourced at https://github.com/X-PLUG/MobileAgent.

## From the paper (full-text excerpts)
**Introduction.** Introduction Large-scale Environment Infrastructure. Diverse Foundational Agents Capability Construction. Scalable Environment RL. 2 GUI-Owl 2.1 End-to-end GUI interactions 2.2 Foundational Agents Capability 2.2.1 Self-Evolving Trajectory Production Framework 2.2.2 Diverse GUI Data Synthesis Grounding. Task Planning. Action Semantics. 2.2.3 Enhanced Robust Reasoning Offline Hint-Guided Rejection Sampling. Distillation from Multi-Agent Framework. Iterative Online Rejection Sampling. 3 Training Paradigm 3.1 Scalable Reinforcement Learning 3.1.1 Infrastructure 3.1.2 Task Mixture Trajectory-aware Relative Policy Optimization for Online Environment RL. 4 Mobile-Agent-v3 5 Experiments 5.1 Model Evaluation 5.1.1 grounding capability 5.1.2 Comprehensive GUI Understanding 5.1.3 End2end and Multi-Agent capability on Online environment 5.2 Trajectory-level Online Reinforcement Learning 5.2.1 Scaling of interaction steps and historical images 5.3 Effect of Reasoning Data Synthesis 5.4 Evaluation on Agen…

**Method / approach.** methods can be broadly divided into two categories. The first category builds agent frameworks based on closed-source models (Yang et al., 2025 ; Xie et al., 2025 ; Agashe et al., 2025 ; Song et al., 2025 ; Wang et al., 2024b ) , however, these approaches struggle to handle unfamiliar tasks and adapt to dynamic environments. The second category focuses mainly on end-to-end model performance (Qin et al., 2025 ; Wang et al., 2025a ) , but such methods often fail to follow instructions faithfully and lack compatibility with diverse agent frameworks, significantly limiting their practical utility. The GUI agents require this foundational model to have the following capabilities: 1) The strong UI perception capabilities (such as for Mobile, PC, and Web); 2) The planning, reflection, and reasoning in various dynamic environments; 3) The flexibility to integrate with various multi-agent frameworks. Figure 2: Overview of our Mobile-Agent-v3. We illustrate our multi-platform environment s…

**Results.** Experiments 5.1 Model Evaluation 5.1.1 grounding capability 5.1.2 Comprehensive GUI Understanding 5.1.3 End2end and Multi-Agent capability on Online environment 5.2 Trajectory-level Online Reinforcement Learning 5.2.1 Scaling of interaction steps and historical images 5.3 Effect of Reasoning Data Synthesis 5.4 Evaluation on Agentic Frameworks 6 Details of Self-Evolving Trajectory Data Production 6.1 Overview 6.2 High-quality Query Generation Mobile. Computer. 6.3 Trajectory Correctness Judgment Module Problem Definition of Trajectory Correctness Judgment. Step-Level Critic. Trajectory-Level Critic. 6.4 Query-specific Guidance Generation 6.5 Examples of Training Data 7 Details of Mobile-Agent-v3 7.1 Core Components and Formalism 7.1.1 State Variables and Definitions 7.2 Agent Architecture in Detail 7.2.1 External Knowledge Retrieval with RAG 7.2.2 The Manager Agen…

**Conclusion.** Conclusion \useunder \ul Mobile-Agent-v3: Fundamental Agents for GUI Automation Abstract This paper introduces GUI-Owl, a foundational GUI agent model that achieves new state-of-the-art performance among open-source end-to-end models across ten GUI benchmarks spanning both desktop and mobile environments, covering grounding, question answering, planning, decision-making, and general procedural knowledge in GUI automation scenarios. Notably, GUI-Owl-7B achieves a score of 66.4 on the AndroidWorld benchmark and 29.4 on the OSWorld-Verified benchmark. Building on this model, we propose a general-purpose GUI agent framework, Mobile-Agent-v3, which further enhances GUI-Owl’s performance (73.3 on AndroidWorld and 37.7 on OSWorld-Veri…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[osworld]]
- **Raw:** `raw/arxiv/2508.15144v2.md` · `raw/arxiv/2508.15144v2.fulltext.md`
