---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Towards a Science of Scaling Agent Systems"
authors: Yubin Kim, Ken Gu, Chanwoo Park, Chunjong Park et al.
url: https://arxiv.org/abs/2512.08296v3
date: 2025-12-09
citationCount: 83
influentialCitationCount: 12
velocity: 12.96
ingested: 2026-06-22
tags: [finance-agents, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Towards a Science of Scaling Agent Systems

**arXiv [2512.08296v3](https://arxiv.org/abs/2512.08296v3)** · 2025-12-09 · **83 citations** (12 influential · 12.96/mo) · Yubin Kim, Ken Gu, Chanwoo Park, Chunjong Park et al.

## Abstract
Agents, language model-based systems capable of reasoning, planning, and acting are widely adopted in real-world tasks, yet how their performance changes as these systems scale across key dimensions remains underexplored. We introduce quantitative scaling principles for agent systems as a predictive model, capturing how performance varies with coordination, model capability, and measurable system and task factors. Across 260 configurations spanning six agentic benchmarks, five canonical architectures (Single-Agent and four Multi-Agent: Independent, Centralized, Decentralized, Hybrid), and three LLM families, we perform controlled evaluations, standardizing tools, prompts, and compute to isolate architectural effects. The resulting model achieves a cross-validated R^2=0.373 across all six benchmarks (R^2=0.413 with a task-grounded capability metric). We identify a robust capability-saturation effect and additional patterns: (1) a coordination yields diminishing returns once single-agent baselines exceed certain performance; (2) tool-heavy tasks appear to incur multi-agent overhead; and (3) architectures without centralized verification tend to propagate errors more than those with centralized coordination. Relative performance change compared to single-agent baseline ranges from +80.8% on decomposable financial reasoning to -70.0% on sequential planning, demonstrating that architecture-task alignment determines collaborative success. The framework identifies the best-performing architecture for 87% of held-out configurations and shows consistent relative architecture preferences on unseen frontier models. Agent effectiveness depends on alignment between coordination and task structure, and that mismatched coordination degrades the performance.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Multi-Agent Systems (MAS) versus Single-Agent Systems (SAS) Agentic Tasks and Benchmarks Scaling Laws and Coordination Mechanisms 3 Agent Systems and Tasks 3.1 System Definition Single-Agent System (SAS). Multi-Agent System (MAS). Communication vs. Coordination. 3.2 Agentic Tasks and Benchmarks Why Environment Feedback Matters. Benchmark Design Principles. 4 Experiments Results 4.1 Setup Benchmarks. LLMs and Intelligence Scaling. Agent Architectures and Complexity. Metrics and Validation. 4.2 Main Results MAS exhibits domain-dependence with architectural variation. Domain Complexity Moderates Coordination Efficacy. Architecture-LLM Family Interactions Reveal Vendor-Specific Coordination Mechanisms. 4.3 Scaling principles Regression Model Achieves Cross-Validated R 2 = 0.413 R^{2}{=}0.413 (ACI) / R 2 = 0.373 R^{2}{=}0.373 (Intelligence Index). The Efficiency-Tools Interaction Emerges as a Consistent Directional Pattern ( β ^ = − 0.096 \hat{\beta}=-0.096 , p = 0.002 p=0.002 ). Overhead…

**Method / approach.** Methodology Sample Sizes. Restrictions and Controls. E.5 Information Gain Computation F SWE-bench Verified and Terminal-Bench Results License: arXiv.org perpetual non-exclusive license arXiv:2512.08296v3 [cs.AI] 08 Apr 2026 \correspondingauthor ybkim95@mit.edu; dmduff@google.com; xliucs@google.com \reportnumber Towards a Science of Scaling Agent Systems Yubin Kim Google Research Massachusetts Institute of Technology Corresponding Author Ken Gu Google Research Chanwoo Park Massachusetts Institute of Technology Chunjong Park Google DeepMind Samuel Schmidgall Google DeepMind A. Ali Heydari Google Research Yao Yan Google Research Zhihan Zhang Google Research Yuchen Zhuang Google DeepMind Yun Liu Google Research Mark Malhotra Google Research Paul Pu Liang Massachusetts Institute of Technology Hae Won Park Massachusetts Institute of Technology Yuzhe Yang Google Research Xuhai Xu Google…

**Results.** Experiments Results 4.1 Setup Benchmarks. LLMs and Intelligence Scaling. Agent Architectures and Complexity. Metrics and Validation. 4.2 Main Results MAS exhibits domain-dependence with architectural variation. Domain Complexity Moderates Coordination Efficacy. Architecture-LLM Family Interactions Reveal Vendor-Specific Coordination Mechanisms. 4.3 Scaling principles Regression Model Achieves Cross-Validated R 2 = 0.413 R^{2}{=}0.413 (ACI) / R 2 = 0.373 R^{2}{=}0.373 (Intelligence Index). The Efficiency-Tools Interaction Emerges as a Consistent Directional Pattern ( β ^ = − 0.096 \hat{\beta}=-0.096 , p = 0.002 p=0.002 ). Overhead Scales Non-Linearly with Task Complexity via the O % × T O\%\times T Interaction. Intelligence Shows Linear Positive Effect ( β ^ I = 0.126 \hat{\beta}_{I}=0.126 , p = 0.008 p=0.008 ). Redundancy Provides Marginal Benefit at Scale ( β ^ R × n a = 0.024 \hat{\beta}_{R\times…

**Conclusion.** Conclusion References A Model Intelligence Index Beyond Artificial Analysis Evaluations. B Out-of-Sample Validation Qualitative Findings Validation. Model Family Differences. C Domain Complexity C.1 Complexity Score Assignment C.2 Domain Characterisation C.3 Critical Threshold D Datasets Finance Agent. BrowseComp Plus. WorkBench. Plancraft. SWE-bench Verified. Terminal-Bench. E Implementation Details E.1 Technical Infrastructure API Integration. Tool Environment. E.2 Agent Configuration Architecture Parameters. Heterogeneous Models. E.3 Prompt Compilation System Dataset Integration. E.4 Evaluation Methodology Sample Sizes. Restrictions and Controls. E.5 I…

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2512.08296v3.md` · `raw/arxiv/2512.08296v3.fulltext.md`
