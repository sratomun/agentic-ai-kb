---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents"
authors: Jiaye Lin, Yifu Guo, Yuzhen Han, Sen Hu et al.
url: https://arxiv.org/abs/2508.02085v6
date: 2025-08-04
citationCount: 45
influentialCitationCount: 2
velocity: 4.25
ingested: 2026-06-22
tags: [coding-agents, self-evolving-agents, tool-use, agentic-ai, arxiv, 2025, cited]
---

# SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents

**arXiv [2508.02085v6](https://arxiv.org/abs/2508.02085v6)** · 2025-08-04 · **45 citations** (2 influential · 4.25/mo) · Jiaye Lin, Yifu Guo, Yuzhen Han, Sen Hu et al.

## Abstract
Large Language Model (LLM)-based agents have recently shown impressive capabilities in complex reasoning and tool use via multi-step interactions with their environments. While these agents have the potential to tackle complicated tasks, their problem-solving process, i.e., agents' interaction trajectory leading to task completion, remains underexploited. These trajectories contain rich feedback that can navigate agents toward the right directions for solving problems correctly. Although prevailing approaches, such as Monte Carlo Tree Search (MCTS), can effectively balance exploration and exploitation, they ignore the interdependence among various trajectories and lack the diversity of search spaces, which leads to redundant reasoning and suboptimal outcomes. To address these challenges, we propose SE-Agent, a Self-Evolution framework that enables Agents to optimize their reasoning processes iteratively. Our approach revisits and enhances former pilot trajectories through three key operations: revision, recombination, and refinement. This evolutionary mechanism enables two critical advantages: (1) it expands the search space beyond local optima by intelligently exploring diverse solution paths guided by previous trajectories, and (2) it leverages cross-trajectory inspiration to efficiently enhance performance while mitigating the impact of suboptimal reasoning paths. Through these mechanisms, SE-Agent achieves continuous self-evolution that incrementally improves reasoning quality. We evaluate SE-Agent on SWE-bench Verified to resolve real-world GitHub issues. Experimental results across five strong LLMs show that integrating SE-Agent delivers up to 55% relative improvement, achieving state-of-the-art performance among all open-source agents on SWE-bench Verified. Our code and demonstration materials are publicly available at https://github.com/JARVIS-Xs/SE-Agent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works Code Agents Agent Capability Enhancement 3 Preliminaries and Problem Setup Task-Oriented Reasoning Environment Reasoning Trajectories Objective of SE-Agent 4 SE-Agent 4.1 Overview of SE-Agent 4.2 Revision Operation 4.2.1 Generating Initial Trajectories Multi-Planning Exploration Mutation-Based Diversification 4.2.2 Reflection and Revision 4.3 Recombination Operation Crossover Transfer Learning Restructuring 4.4 Refinement Operation 4.4.1 Evaluation Function 4.4.2 Selection and Convergence 5 Experiments 5.1 Experimental Setup Benchmark Evaluation Metrics Baselines Implementation Details 5.2 Experimental Results Performance Comparison Ablation Study Hyperparameter Analysis Case Study 6 Conclusion A Prompts A.1 Revision Operation A.1.1 Multi-Planning A.1.2 Reflection and Revision A.2 Recombination Operation A.3 Refinement Operation SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents Jiaye Lin 1,∗…

**Method / approach.** methods such as Monte Carlo Tree Search (MCTS) effectively balance exploration and exploitation [ 16 ; 17 ] , they treat trajectories as independent entities, ignoring the rich interdependencies and potential synergies among different solution paths [ 18 ] . Moreover, even when employing diverse sampling strategies (e.g., varying temperature parameters or prompts), agents tend to converge on structurally similar trajectories that differ only in surface-level expressions, leading to a critical phenomenon: despite generating multiple trajectories, the final outcomes remain surprisingly homogeneous [ 19 ; 20 ; 21 ] . This limitation stems from the inherent nature of probabilistic language models, which naturally gravitate toward high-probability solution patterns, thereby constraining the diversity of the search space [ 22 ; 23 ; 24 ] . To overcome these limitations, we propose SE-Agent, a S elf- E volution framework that enables Agents to iteratively optimize their reasoning proc…

**Results.** Experiments 5.1 Experimental Setup Benchmark Evaluation Metrics Baselines Implementation Details 5.2 Experimental Results Performance Comparison Ablation Study Hyperparameter Analysis Case Study 6 Conclusion A Prompts A.1 Revision Operation A.1.1 Multi-Planning A.1.2 Reflection and Revision A.2 Recombination Operation A.3 Refinement Operation SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents Jiaye Lin 1,∗ Yifu Guo 2,∗ Yuzhen Han 3 Sen Hu 4 Ziyi Ni 5,6 Licheng Wang 5 Mingguang Chen 7 Hongzhang Liu 4,8 Ronghao Chen 4 Yangfan He 9 Daxin Jiang 2 Binxing Jiao 2 Chen Hu 2,† Huacan Wang 5,†, 1 THU 2 StepFun 3 UofT 4 PKU 5 UCAS 6 CASIA 7 UCR 8 USYD 9 UMN Equal Contribution. † Corresponding Authors. R quantaalpha.ai@gmail.com JARVIS-Xs/SE-Agent {abstract2} Large Language Model (LLM)-bas…

**Conclusion.** Conclusion A Prompts A.1 Revision Operation A.1.1 Multi-Planning A.1.2 Reflection and Revision A.2 Recombination Operation A.3 Refinement Operation SE-Agent: Self-Evolution Trajectory Optimization in Multi-Step Reasoning with LLM-Based Agents Jiaye Lin 1,∗ Yifu Guo 2,∗ Yuzhen Han 3 Sen Hu 4 Ziyi Ni 5,6 Licheng Wang 5 Mingguang Chen 7 Hongzhang Liu 4,8 Ronghao Chen 4 Yangfan He 9 Daxin Jiang 2 Binxing Jiao 2 Chen Hu 2,† Huacan Wang 5,†, 1 THU 2 StepFun 3 UofT 4 PKU 5 UCAS 6 CASIA 7 UCR 8 USYD 9 UMN Equal Contribution. † Corresponding Authors. R quantaalpha.ai@gmail.com JARVIS-Xs/SE-Agent {abstract2} Large Language Model (LLM)-based agents have recently sh…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2508.02085v6.md` · `raw/arxiv/2508.02085v6.fulltext.md`
