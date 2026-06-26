---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience"
authors: Zeyi Sun, Ziyu Liu, Yuhang Zang, Yuhang Cao et al.
url: https://arxiv.org/abs/2508.04700v2
date: 2025-08-06
citationCount: 45
influentialCitationCount: 5
velocity: 4.28
ingested: 2026-06-22
tags: [computer-use-agents, agent-reliability, self-evolving-agents, agentic-rl, agent-security, arxiv, 2025, cited]
---

# SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience

**arXiv [2508.04700v2](https://arxiv.org/abs/2508.04700v2)** · 2025-08-06 · **45 citations** (5 influential · 4.28/mo) · Zeyi Sun, Ziyu Liu, Yuhang Zang, Yuhang Cao et al.

## Abstract
Repurposing large vision-language models (LVLMs) as computer use agents (CUAs) has led to substantial breakthroughs, primarily driven by human-labeled data. However, these models often struggle with novel and specialized software, particularly in scenarios lacking human annotations. To address this challenge, we propose SEAgent, an agentic self-evolving framework enabling CUAs to autonomously evolve through interactions with unfamiliar software. Specifically, SEAgent empowers computer-use agents to autonomously master novel software environments via experiential learning, where agents explore new software, learn through iterative trial-and-error, and progressively tackle auto-generated tasks organized from simple to complex. To achieve this goal, we design a World State Model for step-wise trajectory assessment, along with a Curriculum Generator that generates increasingly diverse and challenging tasks. The agent's policy is updated through experiential learning, comprised of adversarial imitation of failure actions and Group Relative Policy Optimization (GRPO) on successful ones. Furthermore, we introduce a specialist-to-generalist training strategy that integrates individual experiential insights from specialist agents, facilitating the development of a stronger generalist CUA capable of continuous autonomous evolution. This unified agent ultimately achieves performance surpassing ensembles of individual specialist agents on their specialized software. We validate the effectiveness of SEAgent across five novel software environments within OS-World. Our approach achieves a significant improvement of 23.2% in success rate, from 11.3% to 34.5%, over a competitive open-source CUA, i.e., UI-TARS.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Agent for Computer Use. Reinforcement Learning for LLMs/LVLMs. 3 Methods 3.1 Autonomous Exploration with Self-evolving Curriculum 3.2 Reinforcement Learning from Experience 3.3 From Specialist to Generalist. 4 Experiments 4.1 Benchmark of Reward Model for computer use agent. 4.2 Self evolution of GUI Agents Models Before Self-Evolution. Evolution Process Details. Specialist Evaluation. From Specialist to Generalist. Ablation Study of Specialist Training. 5 Conclusion A World State Model A.1 Model Architecture and Operation A.2 Fine-Tuning Dataset and Process Data Construction Fine-Tuning Process A.3 Reward Generation from Trajectory Analysis B Curriculum Generator B.1 Task Generation Mechanism C Details of Curriculum Generator. C.1 Exemplar Case during Task Evolution. C.2 Comparative Analysis of Instruction Generation Strategies. Experimental Setup Results and Discussion D Test on TARS-1.5 E Sensitivity Analysis on Key Hyperparameters Number of Generated…

**Method / approach.** Methods 3.1 Autonomous Exploration with Self-evolving Curriculum 3.2 Reinforcement Learning from Experience 3.3 From Specialist to Generalist. 4 Experiments 4.1 Benchmark of Reward Model for computer use agent. 4.2 Self evolution of GUI Agents Models Before Self-Evolution. Evolution Process Details. Specialist Evaluation. From Specialist to Generalist. Ablation Study of Specialist Training. 5 Conclusion A World State Model A.1 Model Architecture and Operation A.2 Fine-Tuning Dataset and Process Data Construction Fine-Tuning Process A.3 Reward Generation from Trajectory Analysis B Curriculum Generator B.1 Task Generation Mechanism C Details of Curriculum Generator. C.1 Exemplar Case during Task Evolution. C.2 Comparative Analysis of Instruction Generation Strategies. Experimental Setup Results and Discussion D Test on TARS-1.5 E Sensitivity Analysis on Key Hyperparameters Number of Generated Tasks…

**Results.** Experiments 4.1 Benchmark of Reward Model for computer use agent. 4.2 Self evolution of GUI Agents Models Before Self-Evolution. Evolution Process Details. Specialist Evaluation. From Specialist to Generalist. Ablation Study of Specialist Training. 5 Conclusion A World State Model A.1 Model Architecture and Operation A.2 Fine-Tuning Dataset and Process Data Construction Fine-Tuning Process A.3 Reward Generation from Trajectory Analysis B Curriculum Generator B.1 Task Generation Mechanism C Details of Curriculum Generator. C.1 Exemplar Case during Task Evolution. C.2 Comparative Analysis of Instruction Generation Strategies. Experimental Setup Results and Discussion D Test on TARS-1.5 E Sensitivity Analysis on Key Hyperparameters Number of Generated Tasks Number of Change Descriptions F Ablation on the Loss Balance Factor. G Reward Function for Differen…

**Conclusion.** Conclusion A World State Model A.1 Model Architecture and Operation A.2 Fine-Tuning Dataset and Process Data Construction Fine-Tuning Process A.3 Reward Generation from Trajectory Analysis B Curriculum Generator B.1 Task Generation Mechanism C Details of Curriculum Generator. C.1 Exemplar Case during Task Evolution. C.2 Comparative Analysis of Instruction Generation Strategies. Experimental Setup Results and Discussion D Test on TARS-1.5 E Sensitivity Analysis on Key Hyperparameters Number of Generated Tasks Number of Change Descriptions F Ablation on the Loss Balance Factor. G Reward Function for Different Actions. H Data Statistics during Iterative Reinforcement Learning.…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2508.04700v2.md` · `raw/arxiv/2508.04700v2.fulltext.md`
