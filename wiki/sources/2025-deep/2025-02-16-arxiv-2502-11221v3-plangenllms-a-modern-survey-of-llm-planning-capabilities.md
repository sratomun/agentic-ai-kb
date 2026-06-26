---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PlanGenLLMs: A Modern Survey of LLM Planning Capabilities"
authors: Hui Wei, Zihao Zhang, Shenghua He, Tian Xia et al.
url: https://arxiv.org/abs/2502.11221v3
date: 2025-02-16
citationCount: 87
influentialCitationCount: 2
velocity: 5.39
ingested: 2026-06-22
tags: [data-query-agents, computer-use-agents, embodied-agents, agentic-ai, arxiv, 2025, cited]
---

# PlanGenLLMs: A Modern Survey of LLM Planning Capabilities

**arXiv [2502.11221v3](https://arxiv.org/abs/2502.11221v3)** · 2025-02-16 · **87 citations** (2 influential · 5.39/mo) · Hui Wei, Zihao Zhang, Shenghua He, Tian Xia et al.

## Abstract
LLMs have immense potential for generating plans, transforming an initial world state into a desired goal state. A large body of research has explored the use of LLMs for various planning tasks, from web navigation to travel planning and database querying. However, many of these systems are tailored to specific problems, making it challenging to compare them or determine the best approach for new tasks. There is also a lack of clear and consistent evaluation criteria. Our survey aims to offer a comprehensive overview of current LLM planners to fill this gap. It builds on foundational work by Kartam and Wilkins (1990) and examines six key performance criteria: completeness, executability, optimality, representation, generalization, and efficiency. For each, we provide a thorough analysis of representative works and highlight their strengths and weaknesses. Our paper also identifies crucial future directions, making it a valuable resource for both practitioners and newcomers interested in leveraging LLM planning to support agentic workflows.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 LLM Planning Foundations (Tables 1 - 3 ) Task Decomposition LLM + Classical Planner Search Algorithm Fine-tuning 3 Criterion I: Completeness (Table 4 ) 4 Criterion II: Executability (Tables 5 - 6 ) 5 Criterion III: Optimality (Table 7 ) 6 Criterion IV: Representation (Tab. 8 - 9 ) LLM-as-a-Translator LLM-as-a-Planner 7 Criterion V: Generalization (Table 10 ) Generalized Planning Skill Storage 8 Criterion VI: Efficiency (Table 11 ) Reduced LLM and World Model Calls Shorter Inputs and Outputs Smaller Model Sizes 9 Evaluation Datasets Methods Metrics 10 Discussion Datasets and Baselines Representation Hallucination Human Preference Alignment Cost Effectiveness Multi-Agent Planning Reasoning, Tool Use, and Memory 11 Conclusion 12 Limitations 13 Appendix PlanGenLLMs: A Modern Survey of LLM Planning Capabilities Hui Wei, † Zihao Zhang, ‡ Shenghua He, § Tian Xia, § Shijia Pan, † Fei Liu ‡ † University of California, Merced ‡ Emory University § PAII Inc. {huiwei2, span24}@…

**Method / approach.** Methods Metrics 10 Discussion Datasets and Baselines Representation Hallucination Human Preference Alignment Cost Effectiveness Multi-Agent Planning Reasoning, Tool Use, and Memory 11 Conclusion 12 Limitations 13 Appendix PlanGenLLMs: A Modern Survey of LLM Planning Capabilities Hui Wei, † Zihao Zhang, ‡ Shenghua He, § Tian Xia, § Shijia Pan, † Fei Liu ‡ † University of California, Merced ‡ Emory University § PAII Inc. {huiwei2, span24}@ucmerced.edu {zihao.zhang, fei.liu}@emory.edu {shenghh2015, TianXia0209}@gmail.com Abstract LLMs have immense potential for generating plans, transforming an initial world state into a desired goal state. A large body of research has explored the use of LLMs for various planning tasks, from web navigation to travel planning and database querying. However, many of these systems are tailored to specific problems, making it challenging to compare them or determine the best approach for new tasks. Ther…

**Results.** experiments. Hallucination LLMs often experience hallucinations Huang et al. ( 2023 ) , which present two major challenges in planning. First, they might struggle to assess if a plan is achievable given a specific problem description Aghzal et al. ( 2023 ); Kambhampati ( 2024 ) . Second, they can generate inadmissible actions and non-existent objects, requiring translation or expert intervention to correct them Huang et al. ( 2022a ); Raman et al. ( 2022 ) . This increases the cost of planning systems. Further research is needed to understand the root causes and improve LLMs’ ability to accurately identify unachievable plans. Evaluating the impact of these hallucinations remains an important research direction. Human Preference Alignment There is a gap in understanding whether system generated plans align with human preferences. It is crucial for open-ended problems where humans execute the plans. Ensuring alignment with h…

**Conclusion.** Conclusion 12 Limitations 13 Appendix PlanGenLLMs: A Modern Survey of LLM Planning Capabilities Hui Wei, † Zihao Zhang, ‡ Shenghua He, § Tian Xia, § Shijia Pan, † Fei Liu ‡ † University of California, Merced ‡ Emory University § PAII Inc. {huiwei2, span24}@ucmerced.edu {zihao.zhang, fei.liu}@emory.edu {shenghh2015, TianXia0209}@gmail.com Abstract LLMs have immense potential for generating plans, transforming an initial world state into a desired goal state. A large body of research has explored the use of LLMs for various planning tasks, from web navigation to travel planning and database querying. However, many of these systems are tailored to specific problems, making it challenging to compare them or determ…

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.11221v3.md` · `raw/arxiv/2502.11221v3.fulltext.md`
