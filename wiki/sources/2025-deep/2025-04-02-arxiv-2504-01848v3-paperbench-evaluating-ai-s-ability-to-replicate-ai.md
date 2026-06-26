---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PaperBench: Evaluating AI's Ability to Replicate AI Research"
authors: Giulio Starace, Oliver Jaffe, Dane Sherburn, James Aung et al.
url: https://arxiv.org/abs/2504.01848v3
date: 2025-04-02
citationCount: 191
influentialCitationCount: 28
velocity: 13.04
ingested: 2026-06-22
tags: [agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# PaperBench: Evaluating AI's Ability to Replicate AI Research

**arXiv [2504.01848v3](https://arxiv.org/abs/2504.01848v3)** · 2025-04-02 · **191 citations** (28 influential · 13.04/mo) · Giulio Starace, Oliver Jaffe, Dane Sherburn, James Aung et al.

## Abstract
We introduce PaperBench, a benchmark evaluating the ability of AI agents to replicate state-of-the-art AI research. Agents must replicate 20 ICML 2024 Spotlight and Oral papers from scratch, including understanding paper contributions, developing a codebase, and successfully executing experiments. For objective evaluation, we develop rubrics that hierarchically decompose each replication task into smaller sub-tasks with clear grading criteria. In total, PaperBench contains 8,316 individually gradable tasks. Rubrics are co-developed with the author(s) of each ICML paper for accuracy and realism. To enable scalable evaluation, we also develop an LLM-based judge to automatically grade replication attempts against rubrics, and assess our judge's performance by creating a separate benchmark for judges. We evaluate several frontier models on PaperBench, finding that the best-performing tested agent, Claude 3.5 Sonnet (New) with open-source scaffolding, achieves an average replication score of 21.0%. Finally, we recruit top ML PhDs to attempt a subset of PaperBench, finding that models do not yet outperform the human baseline. We open-source our code (https://github.com/openai/preparedness) to facilitate future research in understanding the AI engineering capabilities of AI agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 1 Introduction 2 PaperBench 2.1 Task 2.2 Reproduction 2.3 Grading 2.4 Requirement Types 2.5 Rules 2.6 PaperBench Code-Dev 3 Dataset 3.1 Rubrics 3.2 Dealing with Underspecification 4 LLM Judge 4.1 SimpleJudge Implementation 4.2 Evaluating Judges with JudgeEval 5 Experiments and Results 5.1 Agent and Execution Environment 5.2 Main Experiment 5.3 IterativeAgent 5.4 Human Baseline Performance 6 Related Work Evaluating ML Engineering and Research Automatic judging 7 Limitations Dataset Size Contamination Challenging dataset creation LLM-based judge performance Cost 8 Conclusion A Future Directions in AI Evaluation A.1 Exploring rubric design and creation A.2 Improving automated judges A.3 Specification gaming and adversarial agents B Paper Selection Process C Rubric and Addendum Creation Process D SimpleJudge Implementation E Monitor Implementation F Agent Implementation F.1 BasicAgent F.2 IterativeAgent F.3 Task Instructions G More on JudgeEval H Pruned Rubric…

**Method / approach.** methods. Each paper is accompanied by a manually created rubric, which specifies all the necessary outcomes for replicating the paper in detail; resulting in a total of 8,316 individually gradable outcomes across 20 papers. Each of the rubrics in PaperBench has been co-developed with one of the original authors of the paper to ensure that it is high quality and accurate in assessing replication. Rubrics are constructed in a hierarchical manner, such that outcomes can be decomposed into fine-grained sub-outcomes, allowing granular measurement of partial progress towards replicating papers. Given the complexity of ML research papers, we found that even grading a single replication attempt can take tens of hours for a human expert. To streamline the grading process, we explore LLM-based judges and introduce an auxiliary evaluation, JudgeEval, which compares the outputs of automated judges against a dataset of gold labels from human expert judges. Our best LLM-based judge, which uses o…

**Results.** Experiments and Results 5.1 Agent and Execution Environment 5.2 Main Experiment 5.3 IterativeAgent 5.4 Human Baseline Performance 6 Related Work Evaluating ML Engineering and Research Automatic judging 7 Limitations Dataset Size Contamination Challenging dataset creation LLM-based judge performance Cost 8 Conclusion A Future Directions in AI Evaluation A.1 Exploring rubric design and creation A.2 Improving automated judges A.3 Specification gaming and adversarial agents B Paper Selection Process C Rubric and Addendum Creation Process D SimpleJudge Implementation E Monitor Implementation F Agent Implementation F.1 BasicAgent F.2 IterativeAgent F.3 Task Instructions G More on JudgeEval H Pruned Rubric Grading I Full Results I.1 Results stratified by requirement type \pdfcolInitStack tcb@breakable marginparsep has been altered. topmargin has been alte…

**Conclusion.** Conclusion A Future Directions in AI Evaluation A.1 Exploring rubric design and creation A.2 Improving automated judges A.3 Specification gaming and adversarial agents B Paper Selection Process C Rubric and Addendum Creation Process D SimpleJudge Implementation E Monitor Implementation F Agent Implementation F.1 BasicAgent F.2 IterativeAgent F.3 Task Instructions G More on JudgeEval H Pruned Rubric Grading I Full Results I.1 Results stratified by requirement type \pdfcolInitStack tcb@breakable marginparsep has been altered. topmargin has been altered. marginparpush has been altered. The page layout violates the ICML style. Please do not change the page layout, or include packages like…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2504.01848v3.md` · `raw/arxiv/2504.01848v3.fulltext.md`
