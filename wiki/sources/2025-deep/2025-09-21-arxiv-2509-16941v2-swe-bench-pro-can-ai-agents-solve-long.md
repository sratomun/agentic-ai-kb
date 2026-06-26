---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks?"
authors: Xiang Deng, Jeff Da, Edwin Pan, Yannis Yiming He et al.
url: https://arxiv.org/abs/2509.16941v2
date: 2025-09-21
citationCount: 120
influentialCitationCount: 20
velocity: 13.33
ingested: 2026-06-22
tags: [coding-agents, agent-reliability, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks?

**arXiv [2509.16941v2](https://arxiv.org/abs/2509.16941v2)** · 2025-09-21 · **120 citations** (20 influential · 13.33/mo) · Xiang Deng, Jeff Da, Edwin Pan, Yannis Yiming He et al.

## Abstract
We introduce SWE-Bench Pro, a substantially more challenging benchmark that builds upon the best practices of SWE-BENCH [25], but is explicitly designed to capture realistic, complex, enterprise-level problems beyond the scope of SWE-BENCH. SWE-BENCH PRO contains 1,865 problems sourced from a diverse set of 41 actively maintained repositories spanning business applications, B2B services, and developer tools. The benchmark is partitioned into a public set with open access to problems sourced from 11 repositories, a held-out set of 12 repositories and a commercial set of 18 proprietary repositories where we have formal partnership agreements with early-stage startups. Problems in the held-out and the commercial set are not publicly accessible, but we release results on the commercial set. Our benchmark features long-horizon tasks that may require hours to days for a professional software engineer to complete, often involving patches across multiple files and substantial code modifications. All tasks are human-verified and augmented with sufficient context to ensure resolvability. To better understand these limitations, we cluster the failure modes observed in the collected agent trajectories for a clearer characterization of the error patterns exhibited by current models. Overall, SWE-BENCH PRO provides a contamination-resistant testbed that more faithfully captures the complexity and diversity of real-world software development, advancing the pursuit of truly autonomous software engineering agents at a professional level.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Code and Software Engineering Benchmarks 2.2 Software Engineering Agents 3 Dataset Overview 3.1 Characteristics of SWE-Bench Pro 3.2 Task Specification 3.3 Public, Commercial, and Held-Out SWE-Bench Pro 4 Dataset Creation 4.1 Sourcing Problems 4.2 Creating Task Descriptions 4.3 Creating Environments 5 Results 6 Analysis 6.1 Analysis on Model Performance on SWE-Bench Pro 6.2 Ablation: Removing Human Augmentations 6.3 Trajectory Failure Modes 7 Limitations and Future Work 7.1 Limitations 7.2 Future Work 8 Conclusion Appendix A Failure Mode Category Descriptions B Example Task Instance B.1 Problem Statement B.1.1 Example B.2 Requirements B.2.1 Example B.3 Interface B.3.1 Example C Trajectory Failure Mode Analysis C.1 LLM-as-a-judge Prompt \UseRawInputEncoding SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks? Xiang Deng Jeff Da* Edwin Pan Yannis Yiming He Charles Ide Kanak Garg Niklas Lauffer Andrew Park Nitin Pasar…

**Method / approach.** methodology for curating a benchmark in the research community. The three subsets are made available under different access policies. The public set provides both problems and evaluation results openly. The held-out set remains private, preserving it for future overfitting checks against the public set. Finally, for the commercial set, we release evaluation results while keeping the underlying codebases private. The second contribution of SWE-Bench Pro is its emphasis on challenging, diverse, and industrially relevant tasks. To ensure task complexity, we exclude trivial edits (1–10 lines of code) and retain only problems requiring substantial, multi-file modifications. On average, the reference solutions span 107.4 lines of code across 4.1 files. Every problem involves at least 10 lines of change, and over 100 tasks demand more than 100 lines of modification. In addition to complexity, we prioritize diversity and representativeness. The curated repositories are all actively mainta…

**Results.** evaluation of widely used coding models, under a unified scaffold, we observe that their performance on SWE-Bench Pro remains below 45% (Pass@1). To better understand these limitations, we cluster the failure modes observed in the collected agent trajectories for a clearer characterization of the error patterns exhibited by current models. Overall, SWE-Bench Pro provides a contamination-resistant testbed that more faithfully captures the complexity and diversity of real-world software development, advancing the pursuit of truly autonomous software engineering agents at a professional level. 1 Introduction Large Language Model (LLM) agents have been widely adopted in modern software development workflows. SWE-bench [ jimenez2024swebench ] and related works [ yang2024swebenchmm , zan2024multiswe , yang2024sweagent , zhang2025swebench , swebenchverified ] establish the task of issue resolution as a de-facto standard for assessin…

**Conclusion.** Conclusion Appendix A Failure Mode Category Descriptions B Example Task Instance B.1 Problem Statement B.1.1 Example B.2 Requirements B.2.1 Example B.3 Interface B.3.1 Example C Trajectory Failure Mode Analysis C.1 LLM-as-a-judge Prompt \UseRawInputEncoding SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks? Xiang Deng Jeff Da* Edwin Pan Yannis Yiming He Charles Ide Kanak Garg Niklas Lauffer Andrew Park Nitin Pasari Chetan Rane Karmini Sampath Maya Krishnan Srivatsa Kundurthy Sean Hendryx Zifan Wang Vijay Bharadwaj Jeff Holm Raja Aluri Chen Bo Calvin Zhang Noah Jacobson Bing Liu Brad Kenstler # jeffrey.da@scale.com https://scale.co…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2509.16941v2.md` · `raw/arxiv/2509.16941v2.fulltext.md`
