---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond"
authors: Xiaoye Qu, Yafu Li, Zhao-Chen Su, Weigao Sun et al.
url: https://arxiv.org/abs/2503.21614v2
date: 2025-03-27
citationCount: 132
influentialCitationCount: 6
velocity: 8.89
ingested: 2026-06-22
tags: [coding-agents, agentic-ai, arxiv, 2025, cited]
---

# A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond

**arXiv [2503.21614v2](https://arxiv.org/abs/2503.21614v2)** · 2025-03-27 · **132 citations** (6 influential · 8.89/mo) · Xiaoye Qu, Yafu Li, Zhao-Chen Su, Weigao Sun et al.

## Abstract
Recent Large Reasoning Models (LRMs), such as DeepSeek-R1 and OpenAI o1, have demonstrated strong performance gains by scaling up the length of Chain-of-Thought (CoT) reasoning during inference. However, a growing concern lies in their tendency to produce excessively long reasoning traces, which are often filled with redundant content (e.g., repeated definitions), over-analysis of simple problems, and superficial exploration of multiple reasoning paths for harder tasks. This inefficiency introduces significant challenges for training, inference, and real-world deployment (e.g., in agent-based systems), where token economy is critical. In this survey, we provide a comprehensive overview of recent efforts aimed at improving reasoning efficiency in LRMs, with a particular focus on the unique challenges that arise in this new paradigm. We identify common patterns of inefficiency, examine methods proposed across the LRM lifecycle, i.e., from pretraining to inference, and discuss promising future directions for research. To support ongoing development, we also maintain a real-time GitHub repository tracking recent progress in the field. We hope this survey serves as a foundation for further exploration and inspires innovation in this rapidly evolving area.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Structure of the Survey 1.2 Position and Contribution 2 Reasoning Efficiency: Definition, Patterns, and Challenges 2.1 Definition of Reasoning Efficiency 2.2 Patterns of Reasoning Inefficiency Redundant Content. Overthinking Simple Questions. Incoherent and Suboptimal Reasoning. 2.3 Unique Challenges for Efficient Reasoning in the Era of LRMs Quantifying Reasoning Utility: A Balancing Act. Controlling Thinking Length: An Open Frontier. Beyond Transformers: Architectural Bottlenecks. Cross-Task Generalization: One Size Doesn’t Fit All. 3 Efficient Reasoning during Inference 3.1 Length Budgeting 3.2 System Switch 3.3 Model Switch 3.4 Parallel Search 3.5 Summary and Outlook 4 Efficient Reasoning with SFT 4.1 Reasoning Chain Compression 4.2 Latent-Space SFT 4.3 Summary and Outlook 5 Efficient Reasoning with Reinforcement Learning 5.1 Trajectory-level Budgeted Length Rewards 5.2 Redundancy-aware and Step-level Length Rewards 5.3 Adaptive Budget Allocation 5.4 Reasoning Mode Switching 5.5 Altern…

**Method / approach.** methods proposed across the LRM lifecycle, i.e., from pretraining to inference, and discuss promising future directions for research. To support ongoing development, we also maintain a real-time GitHub repository tracking recent progress in the field. 1 1 1 https://github.com/XiaoYee/Awesome_Efficient_LRM_Reasoning We hope this survey serves as a foundation for further exploration and inspires innovation in this rapidly evolving area. A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond Xiaoye Qu 1 † † thanks: Project Lead and Equal Contributions. , Yafu Li 1∗ , Zhao-Chen Su 2 † † thanks: Core Contributors. , Weigao Sun 1† , Jianhao Yan 3† , Dongrui Liu 1† , Ganqu Cui 1 , Daizong Liu 4 , Shuxian Liang 5 , Junxian He 6 , Peng Li 7 , Wei Wei 8 , Jing Shao 1 , Chaochao Lu 1 , Yue Zhang 3 , Xian-Sheng Hua 5 , Bowen Zhou 1,7 , Yu Cheng 9 † † thanks: Corresponding Author. 1 Shanghai AI Laboratory 2 Soochow University 3 Wes…

**Results.** Evaluation and Benchmark 8 Conclusion A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond Xiaoye Qu 1 , Yafu Li 1∗ , Zhao-Chen Su 2 , Weigao Sun 1† , Jianhao Yan 3† , Dongrui Liu 1† , Ganqu Cui 1 , Daizong Liu 4 , Shuxian Liang 5 , Junxian He 6 , Peng Li 7 , Wei Wei 8 , Jing Shao 1 , Chaochao Lu 1 , Yue Zhang 3 , Xian-Sheng Hua 5 , Bowen Zhou 1,7 , Yu Cheng 9 1 Shanghai AI Laboratory 2 Soochow University 3 Westlake University 4 Peking University 5 Tongji University 6 The Hong Kong University of Science and Technology 7 Tsinghua University 8 Huazhong University of Science and Technology 9 The Chinese University of Hong Kong Project Lead and Equal Contributions.Core Contributors.Corresponding Author. Abstract Recent Large Reasoning Models (LRMs), such as DeepSeek-R1 and OpenAI o1, have demonstrated strong performance gains by scaling up the length of Chain-…

**Conclusion.** Conclusion A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond Xiaoye Qu 1 , Yafu Li 1∗ , Zhao-Chen Su 2 , Weigao Sun 1† , Jianhao Yan 3† , Dongrui Liu 1† , Ganqu Cui 1 , Daizong Liu 4 , Shuxian Liang 5 , Junxian He 6 , Peng Li 7 , Wei Wei 8 , Jing Shao 1 , Chaochao Lu 1 , Yue Zhang 3 , Xian-Sheng Hua 5 , Bowen Zhou 1,7 , Yu Cheng 9 1 Shanghai AI Laboratory 2 Soochow University 3 Westlake University 4 Peking University 5 Tongji University 6 The Hong Kong University of Science and Technology 7 Tsinghua University 8 Huazhong University of Science and Technology 9 The Chinese University of Hong Kong Project Lead and Equal Contributions.Core Contributors.Corresponding Au…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2503.21614v2.md` · `raw/arxiv/2503.21614v2.fulltext.md`
