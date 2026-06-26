---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "R2E-Gym: Procedural Environments and Hybrid Verifiers for Scaling Open-Weights SWE Agents"
authors: Naman Jain, Jaskirat Singh, Manish Shetty, Liang Zheng et al.
url: https://arxiv.org/abs/2504.07164v1
date: 2025-04-09
citationCount: 87
influentialCitationCount: 21
velocity: 6.03
ingested: 2026-06-22
tags: [coding-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# R2E-Gym: Procedural Environments and Hybrid Verifiers for Scaling Open-Weights SWE Agents

**arXiv [2504.07164v1](https://arxiv.org/abs/2504.07164v1)** · 2025-04-09 · **87 citations** (21 influential · 6.03/mo) · Naman Jain, Jaskirat Singh, Manish Shetty, Liang Zheng et al.

## Abstract
Improving open-source models on real-world SWE tasks (solving GITHUB issues) faces two key challenges: 1) scalable curation of execution environments to train these models, and, 2) optimal scaling of test-time compute. We introduce AgentGym, the largest procedurally-curated executable gym environment for training real-world SWE-agents, consisting of more than 8.7K tasks. AgentGym is powered by two main contributions: 1) SYNGEN: a synthetic data curation recipe that enables scalable curation of executable environments using test-generation and back-translation directly from commits, thereby reducing reliance on human-written issues or unit tests. We show that this enables more scalable training leading to pass@1 performance of 34.4% on SWE-Bench Verified benchmark with our 32B model. 2) Hybrid Test-time Scaling: we provide an in-depth analysis of two test-time scaling axes; execution-based and execution-free verifiers, demonstrating that they exhibit complementary strengths and limitations. Test-based verifiers suffer from low distinguishability, while execution-free verifiers are biased and often rely on stylistic features. Surprisingly, we find that while each approach individually saturates around 42-43%, significantly higher gains can be obtained by leveraging their complementary strengths. Overall, our approach achieves 51% on the SWE-Bench Verified benchmark, reflecting a new state-of-the-art for open-weight SWE-agents and for the first time showing competitive performance with proprietary models such as o1, o1-preview and sonnet-3.5-v2 (with tools). We will open-source our environments, models, and agent trajectories.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 R2E-Gym : Procedural Synthetic Data Generation 3 Training SWE-Agents using R2E-Gym Environments 3.1 Results and Analysis 4 Efficient Inference Time Scaling With Hybrid Verifiers 4.1 Exploring Different Axes for Training Verifiers 4.2 Comparative Analysis of Execution-Based and Execution-Free Verifiers 4.3 Hybrid Inference Time Scaling 4.4 Ablation Studies on Hybrid Verification Design 5 Related Work 6 Conclusion A Dataset Details B SFT Training C Inference Time Scaling C.1 Execution-Based Testing Agents C.2 Execution-Free Verifiers C.3 Execution-Based Analysis C.4 Execution-Free Analysis D Example Testing Agent Outputs D.1 Example 1: SymPy Relational Parsing Tests D.2 Example 2: Django Model Choice Field Validation Tests E Agent Trajectory Example R2E-Gym: Scaling Open-Weights Software Engineering Agents with Procedural Synthetic Data and Agentic Tests Naman Jain 1 ⋆ Jaskirat Singh 2 ⋆ Manish Shetty 1 Liang Zheng 2 Koushik Sen 1 Ion Stoica 1 1 UC Berkeley 2 Australian National…

**Method / approach.** methods actually exhibit complementary strengths and weaknesses. We find two key insights (studied in § 4.2 ): a) Execution-based methods provide direct signals for patch correctness but struggle with discriminating between solutions , and b) Execution-free verifiers provide better discrimination but can be biased by other heuristics ( e.g ., agent thoughts) over the final patch. Based on the above insights, we propose a hybrid scaling approach leveraging the strengths of both methods. Surprisingly, while the performance of both execution-based and execution-free methods plateaus around 42-43%, the hybrid approach yields significantly higher gains, achieving a final performance of 51% on SWEBench-Verified (Figure 1(b) and § 4.3 ). The key contributions of this paper are: 1) We introduce R2E-Gym , the largest procedurally curated environment for training real-world Swe -agents, increasing the number of executable environments by over 3 3 3 3 times. 2) We provide an in-depth analysi…

**Results.** experiments unless specified otherwise. Table 2 shows the statistics of different datasets, and Figure 2 and Figure 8 show the distribution of the repositories in R2E-Gym-Subset and R2E-Gym respectively. Notably, using our SweGen approach, we can collect over 2.5 2.5 2.5 2.5 times more problems than relying on the data collection relying on GitHub issues (Figure 1(a) ). 3 Training SWE-Agents using R2E-Gym Environments Table 3: Resolve Rate (%) Comparison on SWEBench-Verified and SWEBench-Lite benchmarks. We observe that synthetic data curation ( SweGen ): allows our approach to scale better across different model sizes. All experiments use the Qwen-2.5-Coder as base-models. Model SWEBench-Lite SWEBench-Verified Size Base-model SWE-Gym Ours Δ Δ \Delta roman_Δ Base-model SWE-Gym Ours Δ Δ \Delta roman_Δ 7B 1.0 ( ± 1.0 plus-or-minus 1.0 \pm 1.0 ± 1.0 ) 10.0 ( ± 2.4 plus-or-minus 2.4 \pm 2.4 ± 2.4…

**Conclusion.** Conclusion A Dataset Details B SFT Training C Inference Time Scaling C.1 Execution-Based Testing Agents C.2 Execution-Free Verifiers C.3 Execution-Based Analysis C.4 Execution-Free Analysis D Example Testing Agent Outputs D.1 Example 1: SymPy Relational Parsing Tests D.2 Example 2: Django Model Choice Field Validation Tests E Agent Trajectory Example R2E-Gym: Scaling Open-Weights Software Engineering Agents with Procedural Synthetic Data and Agentic Tests Naman Jain 1 ⋆ Jaskirat Singh 2 ⋆ Manish Shetty 1 Liang Zheng 2 Koushik Sen 1 Ion Stoica 1 1 UC Berkeley 2 Australian National University { naman_jain@berkeley.edu jaskirat.singh@anu.edu.au } R2E-Gym: Synthetic Data and…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2504.07164v1.md` · `raw/arxiv/2504.07164v1.fulltext.md`
