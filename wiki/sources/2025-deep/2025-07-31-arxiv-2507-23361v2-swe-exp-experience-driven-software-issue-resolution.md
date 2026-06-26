---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-Exp: Experience-Driven Software Issue Resolution"
authors: Silin Chen, Shaoxin Lin, Yuling Shi, Heng Lian et al.
url: https://arxiv.org/abs/2507.23361v2
date: 2025-07-31
citationCount: 43
influentialCitationCount: 1
velocity: 4.02
ingested: 2026-06-22
tags: [coding-agents, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# SWE-Exp: Experience-Driven Software Issue Resolution

**arXiv [2507.23361v2](https://arxiv.org/abs/2507.23361v2)** · 2025-07-31 · **43 citations** (1 influential · 4.02/mo) · Silin Chen, Shaoxin Lin, Yuling Shi, Heng Lian et al.

## Abstract
Recent advances in large language model (LLM) agents have shown remarkable progress in software issue resolution, leveraging advanced techniques such as multi-agent collaboration and Monte Carlo Tree Search (MCTS). However, current agents act as memoryless explorers - treating each problem separately without retaining or reusing knowledge from previous repair experiences. This leads to redundant exploration of failed trajectories and missed chances to adapt successful issue resolution methods to similar problems. To address this problem, we introduce SWE-Exp, an experience-enhanced approach that distills concise and actionable experience from prior agent trajectories, enabling continuous learning across issues. Our method introduces a multi-faceted experience bank that captures both successful and failed repair attempts. Specifically, it extracts reusable issue resolution knowledge at different levels - from high-level problem comprehension to specific code changes. Experiments show that SWE-Exp achieves a Pass@1 resolution rate of 73.0% on SWE-Bench Verified using the state-of-the-art LLM Claude 4 Sonnet, significantly outperforming prior results under other agent frameworks. Our approach establishes a new paradigm in which automated software engineering agents systematically accumulate and leverage repair expertise, fundamentally shifting from trial-and-error exploration to strategic, experience-driven issue resolution.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Motivation 3 Methodology 3.1 Conceptual Framework 3.2 Trajectories Collection 3.3 Experiences Extraction 3.3.1 Experience Representation. 3.3.2 Offline Embedding and Storage 3.3.3 Multi-facet Categorization 3.4 Experiences Reuse 3.4.1 Experience Retrieval 3.4.2 Agent Role Separation 4 Experimental Setup 4.1 Research Questions 4.2 Datasets 4.3 Baselines 4.4 Implementation Details 5 Results 5.1 RQ1: Effectiveness 5.2 RQ2: Ablation Study 5.3 RQ3: Impact of Hyperparameters 5.4 Case Study 6 Discussion 6.1 Data Leakage 6.2 Quality of Extracted Experience 6.3 Cost Analysis 6.4 Limitations and Future Directions 7 Threats to Validity 8 Related Work 8.1 Repository-Level Issue Resolution 8.2 Experience Enhanced AI Agents 9 Conclusion A Hyperparameters of MCTS B Prompt Templates B.1 Instructor B.2 Assistant B.3 Issue Agent B.4 Issue Comprehension ExpAgent B.4.1 Successful Experience Extraction Prompt B.4.2 Failed Experience Extraction Prompt B.5 Modification ExpAgent…

**Method / approach.** Methodology 3.1 Conceptual Framework 3.2 Trajectories Collection 3.3 Experiences Extraction 3.3.1 Experience Representation. 3.3.2 Offline Embedding and Storage 3.3.3 Multi-facet Categorization 3.4 Experiences Reuse 3.4.1 Experience Retrieval 3.4.2 Agent Role Separation 4 Experimental Setup 4.1 Research Questions 4.2 Datasets 4.3 Baselines 4.4 Implementation Details 5 Results 5.1 RQ1: Effectiveness 5.2 RQ2: Ablation Study 5.3 RQ3: Impact of Hyperparameters 5.4 Case Study 6 Discussion 6.1 Data Leakage 6.2 Quality of Extracted Experience 6.3 Cost Analysis 6.4 Limitations and Future Directions 7 Threats to Validity 8 Related Work 8.1 Repository-Level Issue Resolution 8.2 Experience Enhanced AI Agents 9 Conclusion A Hyperparameters of MCTS B Prompt Templates B.1 Instructor B.2 Assistant B.3 Issue Agent B.4 Issue Comprehension ExpAgent B.4.1 Successful Experience Extraction Prompt B.4.…

**Results.** Experimental Setup 4.1 Research Questions 4.2 Datasets 4.3 Baselines 4.4 Implementation Details 5 Results 5.1 RQ1: Effectiveness 5.2 RQ2: Ablation Study 5.3 RQ3: Impact of Hyperparameters 5.4 Case Study 6 Discussion 6.1 Data Leakage 6.2 Quality of Extracted Experience 6.3 Cost Analysis 6.4 Limitations and Future Directions 7 Threats to Validity 8 Related Work 8.1 Repository-Level Issue Resolution 8.2 Experience Enhanced AI Agents 9 Conclusion A Hyperparameters of MCTS B Prompt Templates B.1 Instructor B.2 Assistant B.3 Issue Agent B.4 Issue Comprehension ExpAgent B.4.1 Successful Experience Extraction Prompt B.4.2 Failed Experience Extraction Prompt B.5 Modification ExpAgent B.6 RerankAgent B.7 Reuser B.7.1 Reuse Comprehension Experience Prompt B.7.2 Reuse Modification Experience Prompt SWE-Exp: Experience-Driven Software Issue Resolution Si…

**Conclusion.** Conclusion A Hyperparameters of MCTS B Prompt Templates B.1 Instructor B.2 Assistant B.3 Issue Agent B.4 Issue Comprehension ExpAgent B.4.1 Successful Experience Extraction Prompt B.4.2 Failed Experience Extraction Prompt B.5 Modification ExpAgent B.6 RerankAgent B.7 Reuser B.7.1 Reuse Comprehension Experience Prompt B.7.2 Reuse Modification Experience Prompt SWE-Exp: Experience-Driven Software Issue Resolution Silin Chen Shanghai Jiao Tong University China cslsolow@gmail.com , Shaoxin Lin Huawei China 2120200411@mail.nankai.edu.cn , Yuling Shi Shanghai Jiao Tong University China yuling.shi@sjtu.edu.cn , Heng Lian Xidian University China lianheng23@16…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[claude]]
- **Raw:** `raw/arxiv/2507.23361v2.md` · `raw/arxiv/2507.23361v2.fulltext.md`
