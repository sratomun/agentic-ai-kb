---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems"
authors: Shaokun Zhang, Ming Yin, Jieyu Zhang, Jiale Liu et al.
url: https://arxiv.org/abs/2505.00212v3
date: 2025-04-30
citationCount: 93
influentialCitationCount: 22
velocity: 6.77
ingested: 2026-06-22
tags: [agent-reliability, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Which Agent Causes Task Failures and When? On Automated Failure Attribution of LLM Multi-Agent Systems

**arXiv [2505.00212v3](https://arxiv.org/abs/2505.00212v3)** · 2025-04-30 · **93 citations** (22 influential · 6.77/mo) · Shaokun Zhang, Ming Yin, Jieyu Zhang, Jiale Liu et al.

## Abstract
Failure attribution in LLM multi-agent systems-identifying the agent and step responsible for task failures-provides crucial clues for systems debugging but remains underexplored and labor-intensive. In this paper, we propose and formulate a new research area: automated failure attribution for LLM multi-agent systems. To support this initiative, we introduce the Who&When dataset, comprising extensive failure logs from 127 LLM multi-agent systems with fine-grained annotations linking failures to specific agents and decisive error steps. Using the Who&When, we develop and evaluate three automated failure attribution methods, summarizing their corresponding pros and cons. The best method achieves 53.5% accuracy in identifying failure-responsible agents but only 14.2% in pinpointing failure steps, with some methods performing below random. Even SOTA reasoning models, such as OpenAI o1 and DeepSeek R1, fail to achieve practical usability. These results highlight the task's complexity and the need for further research in this area. Code and dataset are available at https://github.com/mingyin1/Agents_Failure_Attribution

## From the paper (full-text excerpts)
**Introduction.** Introduction In recent years, the reframing Large Language Models (LLMs) as agents and built agentic multi-agent systems—composed of interactive, LLM-powered agents collaborating to achieve shared goals—has garnered significant attention (Hong et al., 2023; Li et al., 2023a; Wu et al., 2023). These purposefully designed agentic systems have demon* Equal contribution 1 Pennsylvania State University 2 Duke University 3 University of Washington 4 Nanyang Technological University 5 Meta 6 Google DeepMind 7 Oregon State University 8 AG2AI, Inc.. Correspondence to: †Shaokun Zhang <shaokun.zhang@psu.edu>. Proceedings of the 42 nd International Conference on Machine Learning, Vancouver, Canada. PMLR 267, 2025. Copyright 2025 by the author(s). Previous manual efforts involve a non-straightforward way 1 Title Suppressed Due to Excessive Size to facilitate failure attribution in multi-agent systems: developing increasingly fine-grained benchmarks, with the hope that more metrics will enable quicker failure attribution (Zhuge et al., 2024). For example, DevAI (Zhuge et al., 2024) introduces…

**Method / approach.** methods, summarizing their corresponding pros and cons. The best method achieves 53.5% accuracy in identifying failure-responsible agents but only 14.2% in pinpointing failure steps, with some methods performing below random. Even SOTA reasoning models, such as OpenAI o1 and DeepSeek R1, fail to achieve practical usability. These results highlight the task’s complexity and the need for further research in this area. Code and dataset are available in the public repository. Figure 1. When developing LLMs-powered multi-agent systems, failure attribution—identifying system components responsible for task failures based on evaluation results—has received limited attention in existing research. This process is typically performed manually, demanding substantial labor and specialized expertise. In this study, we explore the potential for automating this process. strated remarkable potential across various domains, including coding (Hong et al., 2023), scientific discovery (Ghafarollahi & B…

**Results.** experiments under two distinct settings to simulate various realistic scenarios. (1) With Ground Truth: In this setting, the final ground truth of the query that the agentic system is attempting to resolve is available to the LLMs. Our focus here is on the typical AI system development cycle, where it is common practice to use a development dataset with ground truth to identify and debug potential errors in experimental systems. (2) Without Ground Truth: In the second setting, the final ground truth of the query is unavailable. In this scenario, LLMs are employed to perform failure attribution in agentic systems based on their running logs. This capability can also be viewed as a form of self-reflection (Huang et al., 2023; Shinn et al., 2024), which contributes to the improvement of multi-agent systems. Throughout this paper, unless otherwise specified, all results are reported as the average accuracy across these two scenarios. 4. Ca…

**Conclusion.** conclusions drawn from the experiments. Additionally, we employ advanced reasoning models, i.e., OpenAI o1 and DeepSeek R1, to assess the performance of reasoning models on failure attribution tasks. The results of these evaluations are provided in Appendix 4.8. 4.1. LLMs for Failure Attribution in Agentic Systems To answer the question mentioned above, we propose three judgement methods for automated failure attribution in agentic systems. Through extensive experiments, we demonstrate that each method has distinct advantages and limitations, and they can be applied either independently or in combination. Furthermore, we analyze the performance of these methods across various scenarios and constraints, highlighting their applicability in d…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2505.00212v3.md` · `raw/arxiv/2505.00212v3.fulltext.md`
