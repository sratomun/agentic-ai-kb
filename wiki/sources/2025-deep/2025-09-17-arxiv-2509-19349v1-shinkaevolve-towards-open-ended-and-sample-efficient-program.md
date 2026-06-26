---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ShinkaEvolve: Towards Open-Ended And Sample-Efficient Program Evolution"
authors: Robert Tjarko Lange, Yuki Imajuku, Edoardo Cetin
url: https://arxiv.org/abs/2509.19349v1
date: 2025-09-17
citationCount: 94
influentialCitationCount: 16
velocity: 10.29
ingested: 2026-06-22
tags: [science-agents, self-evolving-agents, agentic-ai, arxiv, 2025, cited]
---

# ShinkaEvolve: Towards Open-Ended And Sample-Efficient Program Evolution

**arXiv [2509.19349v1](https://arxiv.org/abs/2509.19349v1)** · 2025-09-17 · **94 citations** (16 influential · 10.29/mo) · Robert Tjarko Lange, Yuki Imajuku, Edoardo Cetin

## Abstract
We introduce ShinkaEvolve: a new open-source framework leveraging large language models (LLMs) to advance scientific discovery with state-of-the-art performance and unprecedented efficiency. Recent advances in scaling inference time compute of LLMs have enabled significant progress in generalized scientific discovery. These approaches rely on evolutionary agentic harnesses that leverage LLMs as mutation operators to generate candidate solutions. However, current code evolution methods suffer from critical limitations: they are sample inefficient, requiring thousands of samples to identify effective solutions, and remain closed-source, hindering broad adoption and extension. ShinkaEvolve addresses these limitations, introducing three key innovations: a parent sampling technique balancing exploration and exploitation, code novelty rejection-sampling for efficient search space exploration, and a bandit-based LLM ensemble selection strategy. We evaluate ShinkaEvolve across diverse tasks, demonstrating consistent improvements in sample efficiency and solution quality. ShinkaEvolve discovers a new state-of-the-art circle packing solution using only 150 samples, designs high-performing agentic harnesses for AIME mathematical reasoning tasks, identifies improvements to ALE-Bench competitive programming solutions, and discovers novel mixture-of-expert load balancing loss functions that illuminate the space of optimization strategies. Our results demonstrate that ShinkaEvolve achieves broad applicability with exceptional sample efficiency. By providing open-source accessibility and cost-efficiency, this work democratizes open-ended discovery across diverse computational problems.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Method 3.1 Parent and inspiration sampling 3.2 Program mutation and novelty assessment 3.3 Execution and world feedback 4 Results 4.1 Circle Packing: Reproducing Improving AlphaEvolve Results Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.2 AIME: Evolving Agent Scaffolds for Math Reasoning Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.3 ALE-Bench: Evolving Programs for Combinatorial Optimization Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.4 LLM Training: Evolving Losses for Balanced and Effective Experts Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 5 Ablations Analysis Impact of Parent Selection Strategies. Impact of LLM Ensembling and Prioritization. Impact of Code Embedding-Based Rejection Sampling. 6 Discussion Summary. Limitations. Future Directions. Broader Impact Ethical Considera…

**Method / approach.** Method 3.1 Parent and inspiration sampling 3.2 Program mutation and novelty assessment 3.3 Execution and world feedback 4 Results 4.1 Circle Packing: Reproducing Improving AlphaEvolve Results Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.2 AIME: Evolving Agent Scaffolds for Math Reasoning Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.3 ALE-Bench: Evolving Programs for Combinatorial Optimization Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 4.4 LLM Training: Evolving Losses for Balanced and Effective Experts Task Description. ShinkaEvolve ’s Discovery Dynamics. ShinkaEvolve ’s Discovered Solution. 5 Ablations Analysis Impact of Parent Selection Strategies. Impact of LLM Ensembling and Prioritization. Impact of Code Embedding-Based Rejection Sampling. 6 Discussion Summary. Lim…

**Results.** experiments and test hypotheses (Lu et al., 2024b ; Yamada et al., 2025 ; Novikov et al., 2025 ; Zhang et al., 2025 ) . These frameworks leverage LLMs as sophisticated mutation operators, iteratively refining candidate solutions with successful variants propagating through successive generations. This methodology has proven effective across domains such as competitive programming (Li et al., 2022 ) , mathematical optimization (Romera-Paredes et al., 2024 ) , and automated agentic design (Hu et al., 2024 ) . However, current implementations face significant practical limitations. The primary challenge is substantial sample inefficiency as existing approaches typically require thousands of evaluations, making them computationally expensive and time-consuming. This inefficiency stems from naive exploration strategies that fail to effectively leverage accumulated knowledge from previous generations. Additionally, most leading systems remain…

**Conclusion.** Discussion Summary. Limitations. Future Directions. Broader Impact Ethical Considerations. Robert Tjarko Lange Yuki Imajuku Edoardo Cetin A Shinka Implementation Details B Task Implementation Details B.1 Circle Packing Problem B.2 AIME Math Reasoning Agentic Harness Detailed Task Description. B.3 ALE-Bench Problems Detailed Task Description. B.4 Mixture-of-Experts Load Balancing Loss Detailed Task Description. C ShinkaEvolve Discovered Solutions C.1 Circle Packing Problem C.2 AIME Math Reasoning Agentic Harness C.3 ALE-Bench Problems C.3.1 ALE-Bench LITE task: ahc039 C.3.2 ALE-Bench LITE task: ahc025 C.4 Mixture-of-Experts Load Balancing Loss \sidecaptionvpos figure…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.19349v1.md` · `raw/arxiv/2509.19349v1.fulltext.md`
