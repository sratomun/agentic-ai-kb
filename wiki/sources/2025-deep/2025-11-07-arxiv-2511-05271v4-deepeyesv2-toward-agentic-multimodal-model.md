---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepEyesV2: Toward Agentic Multimodal Model"
authors: Jack Hong, Chenxiao Zhao, ChengLin Zhu, Weiheng Lu et al.
url: https://arxiv.org/abs/2511.05271v4
date: 2025-11-07
citationCount: 72
influentialCitationCount: 10
velocity: 9.65
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# DeepEyesV2: Toward Agentic Multimodal Model

**arXiv [2511.05271v4](https://arxiv.org/abs/2511.05271v4)** · 2025-11-07 · **72 citations** (10 influential · 9.65/mo) · Jack Hong, Chenxiao Zhao, ChengLin Zhu, Weiheng Lu et al.

## Abstract
Agentic multimodal models should not only comprehend text and images, but also actively invoke external tools, such as code execution environments and web search, and integrate these operations into reasoning. In this work, we introduce DeepEyesV2 and explore how to build an agentic multimodal model from the perspectives of data construction, training methods, and model evaluation. We observe that direct reinforcement learning alone fails to induce robust tool-use behavior. This phenomenon motivates a two-stage training pipeline: a cold-start stage to establish tool-use patterns, and reinforcement learning stage to further refine tool invocation. We curate a diverse, moderately challenging training dataset, specifically including examples where tool use is beneficial. We further introduce RealX-Bench, a comprehensive benchmark designed to evaluate real-world multimodal reasoning, which inherently requires the integration of multiple capabilities, including perception, search, and reasoning. We evaluate DeepEyesV2 on RealX-Bench and other representative benchmarks, demonstrating its effectiveness across real-world understanding, mathematical reasoning, and search-intensive tasks. Moreover, DeepEyesV2 exhibits task-adaptive tool invocation, tending to use image operations for perception tasks and numerical computations for reasoning tasks. Reinforcement learning further enables complex tool combinations and allows model to selectively invoke tools based on context. We hope our study can provide guidance for community in developing agentic multimodal models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 DeepEyesV2 3.1 Overall Pipeline 3.2 Pioneer Experiments 3.3 Training Data Curation 3.4 Agentic Reinforcement Learning 4 RealX-Bench 4.1 Design Principles. 4.2 Benchmark Construction 4.3 Data Statistics. 5 Experiments 5.1 Implementation Details 5.2 Evaluation on RealX-Bench 5.3 Results on Other Benchmarks 5.4 Analysis 6 Conclusion References A Appendix A.1 Training Data A.2 Evaluation Protocol A.3 Performance Comparison with Proprietary Models A.4 Tool Usage Pattern Evolution A.5 Zero-Shot Generalization of Tool Usage A.6 Tool Taxonomy A.7 Error Analysis A.8 Prompt A.9 More Cases License: CC BY 4.0 arXiv:2511.05271v4 [cs.CV] 11 Mar 2026 DeepEyesV2: Toward Agentic Multimodal Model Jack Hong , Chenxiao Zhao ∗ , ChengLin Zhu ∗ , Weiheng Lu, Guohai Xu , XingYu Xiaohongshu Inc. Project Homepage jaaackhong@gmail.com , {chenxiao2, xuguohai}@xiaohongshu.com Equal contribution.Corresponding author. Abstract Agentic multimodal models should not only comprehend text…

**Method / approach.** methods, and model evaluation. We observe that direct reinforcement learning alone fails to induce robust tool-use behavior. This phenomenon motivates a two-stage training pipeline: a cold-start stage to establish tool-use patterns, and reinforcement learning stage to further refine tool invocation. We curate a diverse, moderately challenging training dataset, specifically including examples where tool use is beneficial. We further introduce RealX-Bench, a comprehensive benchmark designed to evaluate real-world multimodal reasoning, which inherently requires the integration of multiple capabilities, including perception, search, and reasoning. We evaluate DeepEyesV2 on RealX-Bench and other representative benchmarks, demonstrating its effectiveness across real-world understanding, mathematical reasoning, and search-intensive tasks. Moreover, DeepEyesV2 exhibits task-adaptive tool invocation, tending to use image operations for perception tasks and numerical computations for reasoning…

**Results.** Experiments 3.3 Training Data Curation 3.4 Agentic Reinforcement Learning 4 RealX-Bench 4.1 Design Principles. 4.2 Benchmark Construction 4.3 Data Statistics. 5 Experiments 5.1 Implementation Details 5.2 Evaluation on RealX-Bench 5.3 Results on Other Benchmarks 5.4 Analysis 6 Conclusion References A Appendix A.1 Training Data A.2 Evaluation Protocol A.3 Performance Comparison with Proprietary Models A.4 Tool Usage Pattern Evolution A.5 Zero-Shot Generalization of Tool Usage A.6 Tool Taxonomy A.7 Error Analysis A.8 Prompt A.9 More Cases License: CC BY 4.0 arXiv:2511.05271v4 [cs.CV] 11 Mar 2026 DeepEyesV2: Toward Agentic Multimodal Model Jack Hong , Chenxiao Zhao ∗ , ChengLin Zhu ∗ , Weiheng Lu, Guohai Xu , XingYu Xiaohongshu Inc. Project Homepage jaaackhong@gmail.com , {chenxiao2, xuguohai}@xiaohongshu.com Equal contribution.Corresponding author. Abstr…

**Conclusion.** Conclusion References A Appendix A.1 Training Data A.2 Evaluation Protocol A.3 Performance Comparison with Proprietary Models A.4 Tool Usage Pattern Evolution A.5 Zero-Shot Generalization of Tool Usage A.6 Tool Taxonomy A.7 Error Analysis A.8 Prompt A.9 More Cases License: CC BY 4.0 arXiv:2511.05271v4 [cs.CV] 11 Mar 2026 DeepEyesV2: Toward Agentic Multimodal Model Jack Hong , Chenxiao Zhao ∗ , ChengLin Zhu ∗ , Weiheng Lu, Guohai Xu , XingYu Xiaohongshu Inc. Project Homepage jaaackhong@gmail.com , {chenxiao2, xuguohai}@xiaohongshu.com Equal contribution.Corresponding author. Abstract Agentic multimodal models should not only comprehend text and images, but also actively invoke externa…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.05271v4.md` · `raw/arxiv/2511.05271v4.fulltext.md`
