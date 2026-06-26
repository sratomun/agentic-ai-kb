---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-smith: Scaling Data for Software Engineering Agents"
authors: John Yang, Kilian Lieret, Carlos E. Jimenez, Alexander Wettig et al.
url: https://arxiv.org/abs/2504.21798v2
date: 2025-04-30
citationCount: 170
influentialCitationCount: 24
velocity: 12.38
ingested: 2026-06-22
tags: [coding-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SWE-smith: Scaling Data for Software Engineering Agents

**arXiv [2504.21798v2](https://arxiv.org/abs/2504.21798v2)** · 2025-04-30 · **170 citations** (24 influential · 12.38/mo) · John Yang, Kilian Lieret, Carlos E. Jimenez, Alexander Wettig et al.

## Abstract
Despite recent progress in Language Models (LMs) for software engineering, collecting training data remains a significant pain point. Existing datasets are small, with at most 1,000s of training instances from 11 or fewer GitHub repositories. The procedures to curate such datasets are often complex, necessitating hundreds of hours of human labor; companion execution environments also take up several terabytes of storage, severely limiting their scalability and usability. To address this pain point, we introduce SWE-smith, a novel pipeline for generating software engineering training data at scale. Given any Python codebase, SWE-smith constructs a corresponding execution environment, then automatically synthesizes 100s to 1,000s of task instances that break existing test(s) in the codebase. Using SWE-smith, we create a dataset of 50k instances sourced from 128 GitHub repositories, an order of magnitude larger than all previous works. We train SWE-agent-LM-32B, achieving 40.2% Pass@1 resolve rate on the SWE-bench Verified benchmark, state of the art among open source models. We open source SWE-smith (collection procedure, task instances, trajectories, models) to lower the barrier of entry for research in LM systems for automated software engineering. All assets available at https://swesmith.com.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 \bugs : Software Task Generation at Scale 2.1 Collection 2.2 Features 3 Experiments 4 Results 4.1 Ablations of \bugs 4.2 Analysis of Agent Behavior 5 Related Work 6 Discussion A Infrastructure A.1 \bugs Task Instance A.2 Repository Selection A.3 Validation, Evaluation Harnesses B Bug Generation Strategies B.1 Generating with an LM B.2 Procedural Modification B.3 Combine Bug Patches B.4 Pull Request Mirroring C Dataset Statistics C.1 Bug Generation Statistics C.2 Case Study: SWE-bench \bugs D Issue Generation E Difficulty Rating F Experiments F.1 Training Details F.2 Evaluation Datasets F.3 Trajectory Dataset Breakdown F.4 Training Analyses F.5 Agent Behavioral Studies F.5.1 Turn counts and cost F.5.2 Analysis of agent action space F.5.3 Failure mode analysis F.5.4 Mitigating repetitive actions G Miscellaneous \bugs : Scaling Data for Software Engineering Agents John Yang 1 , Kilian Lieret 2 , Carlos E. Jimenez 2 , Alexander Wettig 2 , Kabir Khandpur 3 , \And Yanzhe…

**Method / approach.** methods relying on LMs, PR Mirrors are more expensive because the task entails rewriting entire files, as opposed to individual functions for LM Modify and LM Rewrite. Yield rates are limited by either lack of test coverage for the change or because the bug candidate did not actually introduce relevant issues. For example, for LM Rewrite, the LM is asked to re-implement the function; it is not explicitly asked for bugs. When requested outright (LM Modify), the yield is higher. Dataset # Tasks # Repos Exec? Source Env. Size R2E (Jain et al., 2024 ) 0.25 0.25 0.25 0.25 k 137 137 137 137 Synth 270 270 270 270 GBs R2E-gym (Subset) (Jain et al., 2025 ) 4.6 4.6 4.6 4.6 k 10 10 10 10 Synth 4 4 4 4 TBs SWE-bench-extra (Badertdinov et al., 2024 ) 6.38 6.38 6.38 6.38 k 2 2 2 2 k Real - SWE-bench-train (Jimenez et al., 2024b ) 19 19 19 19 k 37 37 37 37 Real - SWE-fixer (Xie et al., 2025a ) 115 115 115 115…

**Results.** Experiments 4 Results 4.1 Ablations of \bugs 4.2 Analysis of Agent Behavior 5 Related Work 6 Discussion A Infrastructure A.1 \bugs Task Instance A.2 Repository Selection A.3 Validation, Evaluation Harnesses B Bug Generation Strategies B.1 Generating with an LM B.2 Procedural Modification B.3 Combine Bug Patches B.4 Pull Request Mirroring C Dataset Statistics C.1 Bug Generation Statistics C.2 Case Study: SWE-bench \bugs D Issue Generation E Difficulty Rating F Experiments F.1 Training Details F.2 Evaluation Datasets F.3 Trajectory Dataset Breakdown F.4 Training Analyses F.5 Agent Behavioral Studies F.5.1 Turn counts and cost F.5.2 Analysis of agent action space F.5.3 Failure mode analysis F.5.4 Mitigating repetitive actions G Miscellaneous \bugs : Scaling Data for Software Engineering Agents John Yang 1 , Kilian Lieret 2 , Carlos E. Jimenez 2 , Alex…

**Conclusion.** Conclusion. We introduce \bugs , a dataset of 50 50 50 50 k software engineering task instances from across 128 128 128 128 real world GitHub repositories. \bugs collection pipeline allows us to scale up task instances, environments, and trajectories at a fraction of prior costs without sacrificing faithfulness to open source software development practices. Using \bugs , we train SWE-agent-LM-32B , achieving a state-of-the-art 40.2 40.2 40.2 40.2 % on SWE-bench Verified. Our experiments show how \bugs can be used to identify fundamental trends about developing SWE-agents. We believe \bugs provides the foundational data and infrastructure needed to train software engineering agents in a truly scalable manner. Acknowledgments We than…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2504.21798v2.md` · `raw/arxiv/2504.21798v2.fulltext.md`
