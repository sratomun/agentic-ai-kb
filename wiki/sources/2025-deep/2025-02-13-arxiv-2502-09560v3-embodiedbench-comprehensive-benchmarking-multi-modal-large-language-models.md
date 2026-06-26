---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents"
authors: Rui Yang, Hanyang Chen, Junyu Zhang, Mark Zhao et al.
url: https://arxiv.org/abs/2502.09560v3
date: 2025-02-13
citationCount: 172
influentialCitationCount: 16
velocity: 10.6
ingested: 2026-06-22
tags: [embodied-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents

**arXiv [2502.09560v3](https://arxiv.org/abs/2502.09560v3)** · 2025-02-13 · **172 citations** (16 influential · 10.6/mo) · Rui Yang, Hanyang Chen, Junyu Zhang, Mark Zhao et al.

## Abstract
Leveraging Multi-modal Large Language Models (MLLMs) to create embodied agents offers a promising avenue for tackling real-world tasks. While language-centric embodied agents have garnered substantial attention, MLLM-based embodied agents remain underexplored due to the lack of comprehensive evaluation frameworks. To bridge this gap, we introduce EmbodiedBench, an extensive benchmark designed to evaluate vision-driven embodied agents. EmbodiedBench features: (1) a diverse set of 1,128 testing tasks across four environments, ranging from high-level semantic tasks (e.g., household) to low-level tasks involving atomic actions (e.g., navigation and manipulation); and (2) six meticulously curated subsets evaluating essential agent capabilities like commonsense reasoning, complex instruction understanding, spatial awareness, visual perception, and long-term planning. Through extensive experiments, we evaluated 24 leading proprietary and open-source MLLMs within EmbodiedBench. Our findings reveal that: MLLMs excel at high-level tasks but struggle with low-level manipulation, with the best model, GPT-4o, scoring only 28.9\% on average. EmbodiedBench provides a multifaceted standardized evaluation platform that not only highlights existing challenges but also offers valuable insights to advance MLLM-based embodied agents. Our code and dataset are available at https://embodiedbench.github.io.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Problem Formulation 4 EmbodiedBench 4.1 High-level and Low-level Tasks 4.2 Capability-oriented Data Collection 4.3 Vision-driven Agent Design 5 Experiments 5.1 Experimental Setups 5.2 Benchmark Results 5.3 Language-centric Ablation 5.4 Visual-centric Ablation 5.5 Error Analysis 6 Conclusion A Additional Related Works B Future Research Directions C Details about EmbodiedBench Environments and Datasets C.1 EB-ALFRED Task Description. Dataset Collection. C.2 EB-Habitat Task Description. Dataset Collection. C.3 EB-Navigation Task Description. Dataset Collection. C.4 EB-Manipulation Task description. Dataset Collection. D Model Versions E Definitions and Examples of Capability-oriented Subsets F Additional Experiment Results F.1 Subgoal Success Rate F.2 Average Planner and Environment Steps F.3 Camera Resolution F.4 Detection Boxes F.5 Multi-step Images F.6 Multi-view Images F.7 Visual In-context Learning (ICL) F.8 Additional Ablation Study Conclusion G…

**Method / approach.** methods are needed to effectively leverage visual input for high-level embodied tasks. Fine-grained Results across Subsets. We have the following findings based on our evaluation across 6 subsets. (1) Performance Varies across Different Subsets. We observe that models perform differently across various subsets. For instance, while Claude-3.5-Sonnet is the best model on EB-Habitat overall, GPT-4o surpasses it on long-horizon subsets (64% vs. 58%). This divergence is even more evident in low-level tasks. In EB-Manipulation, for example, Claude-3.5-Sonnet scores 14.6 and 5.6 points higher than GPT-4o on the complex instruction and visual appearance subsets, respectively, but falls significantly behind on other capabilities. These results highlight the importance of fine-grained evaluations to uncover nuanced limitations in current models. (2) Long-Horizon Planning Is the Most Challenging Task . The long-horizon subset consistently proves to be the most difficult, showing the la…

**Results.** Experiments 5.1 Experimental Setups 5.2 Benchmark Results 5.3 Language-centric Ablation 5.4 Visual-centric Ablation 5.5 Error Analysis 6 Conclusion A Additional Related Works B Future Research Directions C Details about EmbodiedBench Environments and Datasets C.1 EB-ALFRED Task Description. Dataset Collection. C.2 EB-Habitat Task Description. Dataset Collection. C.3 EB-Navigation Task Description. Dataset Collection. C.4 EB-Manipulation Task description. Dataset Collection. D Model Versions E Definitions and Examples of Capability-oriented Subsets F Additional Experiment Results F.1 Subgoal Success Rate F.2 Average Planner and Environment Steps F.3 Camera Resolution F.4 Detection Boxes F.5 Multi-step Images F.6 Multi-view Images F.7 Visual In-context Learning (ICL) F.8 Additional Ablation Study Conclusion G Further Discussion on Chat History as Inpu…

**Conclusion.** Conclusion A Additional Related Works B Future Research Directions C Details about EmbodiedBench Environments and Datasets C.1 EB-ALFRED Task Description. Dataset Collection. C.2 EB-Habitat Task Description. Dataset Collection. C.3 EB-Navigation Task Description. Dataset Collection. C.4 EB-Manipulation Task description. Dataset Collection. D Model Versions E Definitions and Examples of Capability-oriented Subsets F Additional Experiment Results F.1 Subgoal Success Rate F.2 Average Planner and Environment Steps F.3 Camera Resolution F.4 Detection Boxes F.5 Multi-step Images F.6 Multi-view Images F.7 Visual In-context Learning (ICL) F.8 Additional Ablation Study Conclusion…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2502.09560v3.md` · `raw/arxiv/2502.09560v3.fulltext.md`
