---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents"
authors: Haoran Tan, Zeyu Zhang, Chen Ma, Xu Chen et al.
url: https://arxiv.org/abs/2506.21605v1
date: 2025-06-20
citationCount: 56
influentialCitationCount: 3
velocity: 4.64
ingested: 2026-06-22
tags: [agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents

**arXiv [2506.21605v1](https://arxiv.org/abs/2506.21605v1)** · 2025-06-20 · **56 citations** (3 influential · 4.64/mo) · Haoran Tan, Zeyu Zhang, Chen Ma, Xu Chen et al.

## Abstract
Recent works have highlighted the significance of memory mechanisms in LLM-based agents, which enable them to store observed information and adapt to dynamic environments. However, evaluating their memory capabilities still remains challenges. Previous evaluations are commonly limited by the diversity of memory levels and interactive scenarios. They also lack comprehensive metrics to reflect the memory capabilities from multiple aspects. To address these problems, in this paper, we construct a more comprehensive dataset and benchmark to evaluate the memory capability of LLM-based agents. Our dataset incorporates factual memory and reflective memory as different levels, and proposes participation and observation as various interactive scenarios. Based on our dataset, we present a benchmark, named MemBench, to evaluate the memory capability of LLM-based agents from multiple aspects, including their effectiveness, efficiency, and capacity. To benefit the research community, we release our dataset and project at https://github.com/import-myself/Membench.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 3 Dataset Construction 3.1 Pipeline of Data Generation 3.2 Multi-scenario Memory 3.3 Multi-level Memory 3.4 Multi-metric Evaluation 3.5 Dataset Statistics 4 Benchmark 4.1 Experimental Settings 4.2 Evaluations on Factual Memory 4.3 Evaluations on Reflective Memory 4.4 Evaluations on Memory Capacity 4.5 Comparison of Different Inference Models 5 Conclusion A Case Studies A.1 User Relation Graph Example A.2 FM-RM Directionary Example A.3 Question Description A.4 Participation Example A.5 Observation Example B Detail Data Statics C Data Creation Prompt C.1 Profile Prompt C.2 Self-dialogue Prompt C.3 Observation Prompt D Result Details D.1 Reflective Result D.2 Facutal Result MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents Haoran Tan 1 1 1 1 Co-first authors. 3 3 3 Beijing Key Laboratory of Research on Large Models and Intelligent Governance 4 4 4 Engineering Research Center of Next-Generation Intelligent Search and Recommendation, MOE , Zeyu Zh…

**Method / approach.** methods that do not align with the agent’s memory process. Moreover, the evaluation metrics used with these datasets are not comprehensive. Compared with previous works, our work is the first study that emphasizes reflective memory, puts forward observation scenarios, adopts evaluation methods that are better suited to the agent’s memory process, with more comprehensive metrics. Figure 1: An example of generating dialogue data. First, the event "Build Start 2024" is extracted with the time "next week Mon 7:00 PM," which is then used to generate evidence dialogues and questions. It’s merged with dialogues generated from other attributes to form a complete dialogue, and an answer is generated based on the provided time label "2024-10-07 Monday 19:00". 3 Dataset Construction 3.1 Pipeline of Data Generation Inspired by MemSim Zhang et al. ( 2024b ) , we expand the dataset for memory evaluation based on this framework. Building upon the question types of factual memory inc…

**Results.** Experimental Settings 4.2 Evaluations on Factual Memory 4.3 Evaluations on Reflective Memory 4.4 Evaluations on Memory Capacity 4.5 Comparison of Different Inference Models 5 Conclusion A Case Studies A.1 User Relation Graph Example A.2 FM-RM Directionary Example A.3 Question Description A.4 Participation Example A.5 Observation Example B Detail Data Statics C Data Creation Prompt C.1 Profile Prompt C.2 Self-dialogue Prompt C.3 Observation Prompt D Result Details D.1 Reflective Result D.2 Facutal Result MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents Haoran Tan 1 1 1 1 Co-first authors. 3 3 3 Beijing Key Laboratory of Research on Large Models and Intelligent Governance 4 4 4 Engineering Research Center of Next-Generation Intelligent Search and Recommendation, MOE , Zeyu Zhang 1 1 1 1 Co-first authors. 3 3 3 Beijing Key Laboratory of Research on L…

**Conclusion.** Conclusion A Case Studies A.1 User Relation Graph Example A.2 FM-RM Directionary Example A.3 Question Description A.4 Participation Example A.5 Observation Example B Detail Data Statics C Data Creation Prompt C.1 Profile Prompt C.2 Self-dialogue Prompt C.3 Observation Prompt D Result Details D.1 Reflective Result D.2 Facutal Result MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents Haoran Tan 1 1 1 1 Co-first authors. 3 3 3 Beijing Key Laboratory of Research on Large Models and Intelligent Governance 4 4 4 Engineering Research Center of Next-Generation Intelligent Search and Recommendation, MOE , Zeyu Zhang 1 1 1 1 Co-first authors. 3 3 3 Beijing Key Laboratory of…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2506.21605v1.md` · `raw/arxiv/2506.21605v1.fulltext.md`
