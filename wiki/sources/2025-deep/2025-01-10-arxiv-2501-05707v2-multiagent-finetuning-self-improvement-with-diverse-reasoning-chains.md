---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains"
authors: Vighnesh Subramaniam, Yilun Du, Joshua B. Tenenbaum, Antonio Torralba et al.
url: https://arxiv.org/abs/2501.05707v2
date: 2025-01-10
citationCount: 86
influentialCitationCount: 10
velocity: 4.96
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-ai, arxiv, 2025, cited]
---

# Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains

**arXiv [2501.05707v2](https://arxiv.org/abs/2501.05707v2)** · 2025-01-10 · **86 citations** (10 influential · 4.96/mo) · Vighnesh Subramaniam, Yilun Du, Joshua B. Tenenbaum, Antonio Torralba et al.

## Abstract
Large language models (LLMs) have achieved remarkable performance in recent years but are fundamentally limited by the underlying training data. To improve models beyond the training data, recent works have explored how LLMs can be used to generate synthetic data for autonomous self-improvement. However, successive steps of self-improvement can reach a point of diminishing returns. In this work, we propose a complementary approach towards self-improvement where finetuning is applied to a multiagent society of language models. A group of language models, all starting from the same base model, are independently specialized by updating each one using data generated through multiagent interactions among the models. By training each model on independent sets of data, we illustrate how this approach enables specialization across models and diversification over the set of models. As a result, our overall system is able to preserve diverse reasoning chains and autonomously improve over many more rounds of fine-tuning than single-agent self-improvement methods. We quantitatively illustrate the efficacy of the approach across a wide suite of reasoning tasks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Multiagent Finetuning of Language Models 2.1 Multiagent Debate 2.2 Finetuning Models on Generated Data 2.3 Finetuning Multiple Generation and Critic Models 2.4 Multiple Iterations of Finetuning 2.5 Inference 3 Experiments 3.1 Language Reasoning Tasks 3.2 Baselines 3.3 Quantitative Results 3.4 Multiple Iterations of Finetuning 4 Analysis 4.1 Ablation Studies 4.2 Agent Response Diversity 4.3 Zero-shot Generalization 5 Related Work 6 Conclusion and Limitations A Appendix Summary B Methodology Details B.1 Summarization details B.2 Inference details B.3 Experimental Details C Diversity Metrics C.1 Consensus C.2 KL-Divergence C.3 KL-Divergence Across Models C.4 Embedding Dissimilarity D Cooperative Finetuning E Additional Comparisons E.1 Modulating Temperatures E.2 Unique ID for Agents F Additional Agents in Debate G Mathematical Model of Diversity Over Rounds of Finetuning H Additional Evaluations H.1 Larger MATH Evaluation H.2 MMLU H.3 Zero-Shot Generalization Evaluation…

**Method / approach.** Methodology Details B.1 Summarization details B.2 Inference details B.3 Experimental Details C Diversity Metrics C.1 Consensus C.2 KL-Divergence C.3 KL-Divergence Across Models C.4 Embedding Dissimilarity D Cooperative Finetuning E Additional Comparisons E.1 Modulating Temperatures E.2 Unique ID for Agents F Additional Agents in Debate G Mathematical Model of Diversity Over Rounds of Finetuning H Additional Evaluations H.1 Larger MATH Evaluation H.2 MMLU H.3 Zero-Shot Generalization Evaluation Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains Vighnesh Subramaniam MIT CSAIL vsub851@mit.edu Yilun Du † † footnotemark: Harvard University ydu@seas.harvard.edu Joshua B. Tenenbaum MIT CSAIL, BCS, CBMM jbt@mit.edu Antonio Torralba MIT CSAIL torralba@mit.edu Shuang Li Stanford University lishuang@stanford.edu Igor Mordatch 2 2 footnotemark: 2 UC Berkeley mordatch@berkeley.edu Equal Contrib…

**Results.** Experiments 3.1 Language Reasoning Tasks 3.2 Baselines 3.3 Quantitative Results 3.4 Multiple Iterations of Finetuning 4 Analysis 4.1 Ablation Studies 4.2 Agent Response Diversity 4.3 Zero-shot Generalization 5 Related Work 6 Conclusion and Limitations A Appendix Summary B Methodology Details B.1 Summarization details B.2 Inference details B.3 Experimental Details C Diversity Metrics C.1 Consensus C.2 KL-Divergence C.3 KL-Divergence Across Models C.4 Embedding Dissimilarity D Cooperative Finetuning E Additional Comparisons E.1 Modulating Temperatures E.2 Unique ID for Agents F Additional Agents in Debate G Mathematical Model of Diversity Over Rounds of Finetuning H Additional Evaluations H.1 Larger MATH Evaluation H.2 MMLU H.3 Zero-Shot Generalization Evaluation Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains Vighnesh Subramania…

**Conclusion.** Conclusion and Limitations A Appendix Summary B Methodology Details B.1 Summarization details B.2 Inference details B.3 Experimental Details C Diversity Metrics C.1 Consensus C.2 KL-Divergence C.3 KL-Divergence Across Models C.4 Embedding Dissimilarity D Cooperative Finetuning E Additional Comparisons E.1 Modulating Temperatures E.2 Unique ID for Agents F Additional Agents in Debate G Mathematical Model of Diversity Over Rounds of Finetuning H Additional Evaluations H.1 Larger MATH Evaluation H.2 MMLU H.3 Zero-Shot Generalization Evaluation Multiagent Finetuning: Self Improvement with Diverse Reasoning Chains Vighnesh Subramaniam MIT CSAIL vsub851@mit.edu Yilun Du † † footn…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2501.05707v2.md` · `raw/arxiv/2501.05707v2.fulltext.md`
