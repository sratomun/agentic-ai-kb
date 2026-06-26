---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WebThinker: Empowering Large Reasoning Models with Deep Research Capability"
authors: Xiaoxi Li, Jiajie Jin, Guanting Dong, Hongjin Qian et al.
url: https://arxiv.org/abs/2504.21776v2
date: 2025-04-30
citationCount: 279
influentialCitationCount: 29
velocity: 20.32
ingested: 2026-06-22
tags: [science-agents, agent-reliability, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# WebThinker: Empowering Large Reasoning Models with Deep Research Capability

**arXiv [2504.21776v2](https://arxiv.org/abs/2504.21776v2)** · 2025-04-30 · **279 citations** (29 influential · 20.32/mo) · Xiaoxi Li, Jiajie Jin, Guanting Dong, Hongjin Qian et al.

## Abstract
Large reasoning models (LRMs), such as OpenAI-o1 and DeepSeek-R1, demonstrate impressive long-horizon reasoning capabilities. However, their reliance on static internal knowledge limits their performance on complex, knowledge-intensive tasks and hinders their ability to produce comprehensive research reports requiring synthesis of diverse web information. To address this, we propose WebThinker, a deep research agent that empowers LRMs to autonomously search the web, navigate among web pages, and draft reports during the reasoning process. WebThinker integrates a Deep Web Explorer module, enabling LRMs to dynamically search, navigate, and extract information from the web when encountering knowledge gaps. It also employs an Autonomous Think-Search-and-Draft strategy, allowing the model to seamlessly interleave reasoning, information gathering, and report writing in real time. To further enhance research tool utilization, we introduce an RL-based training strategy via iterative online Direct Preference Optimization (DPO). Extensive experiments on complex reasoning benchmarks (GPQA, GAIA, WebWalkerQA, HLE) and scientific report generation tasks (Glaive) demonstrate that WebThinker significantly outperforms existing methods and strong proprietary systems. Our approach enhances LRM reliability and applicability in complex scenarios, paving the way for more capable and versatile deep research systems. The code is available at https://github.com/RUC-NLPIR/WebThinker.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Large Reasoning Models. Retrieval-Augmented Generation. 3 Methodology 3.1 Problem Formulation 3.2 Overview of the WebThinker Framework 3.3 Solving Complex Reasoning Tasks with the Deep Web Explorer 3.4 Generating Comprehensive Reports via Autonomous Think-Search-and-Draft 3.5 Improving LRMs with Research Tools via Reinforcement Learning Preference Data Construction. Iterative Online DPO Training. 4 Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Complex Problem-Solving Main Results. 4.5 Results on Scientific Report Generation Main Results. Analysis of Information Scopes. 4.6 Adaptability of WebThinker Across Different LRM Backbones. 4.7 Ablation Studies 5 Conclusion A Inference Process A.1 Research-Related Tools A.2 Inference Process of WebThinker A.2.1 Inference for Main Reasoning Process Problem-Solving Mode: Report Generation Mode: A.2.2 Inference for Deep Web Explorer Deep Web Explorer: B Datasets B.1 Comple…

**Method / approach.** Methodology 3.1 Problem Formulation 3.2 Overview of the WebThinker Framework 3.3 Solving Complex Reasoning Tasks with the Deep Web Explorer 3.4 Generating Comprehensive Reports via Autonomous Think-Search-and-Draft 3.5 Improving LRMs with Research Tools via Reinforcement Learning Preference Data Construction. Iterative Online DPO Training. 4 Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Complex Problem-Solving Main Results. 4.5 Results on Scientific Report Generation Main Results. Analysis of Information Scopes. 4.6 Adaptability of WebThinker Across Different LRM Backbones. 4.7 Ablation Studies 5 Conclusion A Inference Process A.1 Research-Related Tools A.2 Inference Process of WebThinker A.2.1 Inference for Main Reasoning Process Problem-Solving Mode: Report Generation Mode: A.2.2 Inference for Deep Web Explorer Deep Web Explorer: B Datasets B.1 Comp…

**Results.** Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Complex Problem-Solving Main Results. 4.5 Results on Scientific Report Generation Main Results. Analysis of Information Scopes. 4.6 Adaptability of WebThinker Across Different LRM Backbones. 4.7 Ablation Studies 5 Conclusion A Inference Process A.1 Research-Related Tools A.2 Inference Process of WebThinker A.2.1 Inference for Main Reasoning Process Problem-Solving Mode: Report Generation Mode: A.2.2 Inference for Deep Web Explorer Deep Web Explorer: B Datasets B.1 Complex Reasoning Tasks B.2 Scientific Report Generation Tasks C Instruction Templates C.1 Instructions for WebThinker C.2 Task Instructions C.2.1 Task Instruction for QwQ-based Models C.2.2 Task Instruction for DeepSeek-R1-based Models C.3 Instructions for Evaluation C.3.1 Evaluation Instructio…

**Conclusion.** Conclusion A Inference Process A.1 Research-Related Tools A.2 Inference Process of WebThinker A.2.1 Inference for Main Reasoning Process Problem-Solving Mode: Report Generation Mode: A.2.2 Inference for Deep Web Explorer Deep Web Explorer: B Datasets B.1 Complex Reasoning Tasks B.2 Scientific Report Generation Tasks C Instruction Templates C.1 Instructions for WebThinker C.2 Task Instructions C.2.1 Task Instruction for QwQ-based Models C.2.2 Task Instruction for DeepSeek-R1-based Models C.3 Instructions for Evaluation C.3.1 Evaluation Instruction for Problem-Solving Tasks C.3.2 Evaluation Instruction for Report Quality C.4 Additional Notes D Case Study D.1 Case Study f…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]] · [[deepseek]]
- **Raw:** `raw/arxiv/2504.21776v2.md` · `raw/arxiv/2504.21776v2.fulltext.md`
