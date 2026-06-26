---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Large Language Models Often Know When They Are Being Evaluated"
authors: Joe Needham, Giles Edkins, Govind Pimpale, Henning Bartsch et al.
url: https://arxiv.org/abs/2505.23836v3
date: 2025-05-28
citationCount: 67
influentialCitationCount: 6
velocity: 5.23
ingested: 2026-06-22
tags: [recommendation-agents, computer-use-agents, agent-reliability, agent-evaluation, governance-gap, arxiv, 2025, cited]
---

# Large Language Models Often Know When They Are Being Evaluated

**arXiv [2505.23836v3](https://arxiv.org/abs/2505.23836v3)** · 2025-05-28 · **67 citations** (6 influential · 5.23/mo) · Joe Needham, Giles Edkins, Govind Pimpale, Henning Bartsch et al.

## Abstract
If AI models can detect when they are being evaluated, the effectiveness of evaluations might be compromised. For example, models could have systematically different behavior during evaluations, leading to less reliable benchmarks for deployment and governance decisions. We investigate whether frontier language models can accurately classify transcripts based on whether they originate from evaluations or real-world deployment, a capability we call evaluation awareness. To achieve this, we construct a diverse benchmark of 1,000 prompts and transcripts from 61 distinct datasets. These span public benchmarks (e.g., MMLU, SWEBench), real-world deployment interactions, and agent trajectories from scaffolding frameworks (e.g., web-browsing agents). Frontier models clearly demonstrate above-random evaluation awareness (Gemini-2.5-Pro reaches an AUC of $0.83$), but do not yet surpass our simple human baseline (AUC of $0.92$). Furthermore, both AI models and humans are better at identifying evaluations in agentic settings compared to chat settings. Additionally, we test whether models can identify the purpose of the evaluation. Under multiple-choice and open-ended questioning, AI models far outperform random chance in identifying what an evaluation is testing for. Our results indicate that frontier models already exhibit a substantial, though not yet superhuman, level of evaluation-awareness. We recommend tracking this capability in future models.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background Situational Awareness. Evaluation Awareness. 3 Methods 3.1 Data collection 3.2 Measuring Evaluation Awareness Probe Question (“PQ”) selection. Metrics. Identifying evaluation purpose. 3.3 Human baseline 4 Results 4.1 Frontier models show evaluation-awareness 4.2 Identifying evaluation purpose 4.3 Frontier models tend to over-classify transcripts as evaluations 4.4 Qualitative analysis of model evaluation-awareness Meta-Reasoning. General patterns in model explanations. 5 Discussion A Appendix / supplemental material A.1 Model versions A.2 Probe Questions (“PQs”) Binary-choice PQs. Elicitation failures. PQ selection. A.3 Benchmark construction Capabilities evaluations. Alignment evaluations. Chat-Deployment Agent-Deployment A.3.1 Chat-Evaluations A.3.2 Agent-Evaluations A.3.3 Chat-Deployment A.3.4 Agent-Deployment A.4 Bespoke datasets A.4.1 Aider coding trajectories ( aider_commit dataset) A.4.2 Open Deep Research A.4.3 Other agentic trajectories A.4.…

**Method / approach.** Methods 3.1 Data collection 3.2 Measuring Evaluation Awareness Probe Question (“PQ”) selection. Metrics. Identifying evaluation purpose. 3.3 Human baseline 4 Results 4.1 Frontier models show evaluation-awareness 4.2 Identifying evaluation purpose 4.3 Frontier models tend to over-classify transcripts as evaluations 4.4 Qualitative analysis of model evaluation-awareness Meta-Reasoning. General patterns in model explanations. 5 Discussion A Appendix / supplemental material A.1 Model versions A.2 Probe Questions (“PQs”) Binary-choice PQs. Elicitation failures. PQ selection. A.3 Benchmark construction Capabilities evaluations. Alignment evaluations. Chat-Deployment Agent-Deployment A.3.1 Chat-Evaluations A.3.2 Agent-Evaluations A.3.3 Chat-Deployment A.3.4 Agent-Deployment A.4 Bespoke datasets A.4.1 Aider coding trajectories ( aider_commit dataset) A.4.2 Open Deep Research A.4.3 Other agentic traj…

**Results.** experiments on a development subset of 100 samples, we identified a set of 5 PQs that achieves a suitable trade-off between performance and cost for GPT-4.1. For our main experiments we use the same selected five PQs across all tested models, listed in Appendix A.2 . The full PQ selection process is detailed in Appendix A.2 . Metrics. To score these binary assessments, we selected three metrics that together provide a comprehensive assessment of evaluation-awareness: 1. Area under the ROC curve (AUC): Our primary metric measures discriminative ability — how well models separate evaluations from real interactions — independent of the specific threshold used. AUC ranges from 0.5 (random guessing) to 1.0 (perfect discrimination). 2. Calibration: We quantify calibration using Expected Calibration Error (ECE), which measures the average absolute difference between predicted probabilities and true frequencies across proba…

**Conclusion.** Discussion A Appendix / supplemental material A.1 Model versions A.2 Probe Questions (“PQs”) Binary-choice PQs. Elicitation failures. PQ selection. A.3 Benchmark construction Capabilities evaluations. Alignment evaluations. Chat-Deployment Agent-Deployment A.3.1 Chat-Evaluations A.3.2 Agent-Evaluations A.3.3 Chat-Deployment A.3.4 Agent-Deployment A.4 Bespoke datasets A.4.1 Aider coding trajectories ( aider_commit dataset) A.4.2 Open Deep Research A.4.3 Other agentic trajectories A.4.4 Author Claude A.5 Judge prompts A.5.1 Identifying evaluation purpose A.5.2 Chain-of-thought categorization A.6 Identifying evaluation purpose B Qualitative chain-of-thought analysis B.1 C…

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Raw:** `raw/arxiv/2505.23836v3.md` · `raw/arxiv/2505.23836v3.fulltext.md`
