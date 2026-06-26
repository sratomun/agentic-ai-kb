---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes"
authors: Cheng-Yu Hsieh et al.
url: https://arxiv.org/abs/2305.02301
date: 2023-05-03
ingested: 2026-06-22
tags: [arxiv, synthetic-data, data]
---

# Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes

**arXiv [2305.02301](https://arxiv.org/abs/2305.02301)** · 2023-05-03 · Cheng-Yu Hsieh, Chun-Liang Li, Chih-Kuan Yeh, Hootan Nakhost, Yasuhisa Fujii, Alexander Ratner, Ranjay Krishna, Chen-Yu Lee, Tomas Pfister (University of Washington / Google)

**Significance.** Reframes LLM distillation: extract the *reasoning* (chain-of-thought rationales), not just the labels. A small model trained on rationales beats a 540B teacher with a fraction of the data — a key recipe for synthetic-rationale data.

## Abstract
Deploying large language models (LLMs) is challenging because they are memory inefficient and compute-intensive for practical applications. In reaction, researchers train smaller task-specific models by either finetuning with human labels or distilling using LLM-generated labels. However, finetuning and distillation require large amounts of training data to achieve comparable performance to LLMs. We introduce Distilling step-by-step, a new mechanism that (a) trains smaller models that outperform LLMs, and (b) achieves so by leveraging less training data needed by finetuning or distillation. Our method extracts LLM rationales as additional supervision for training small models within a multi-task framework. We present three findings across 4 NLP benchmarks: First, compared to both finetuning and distillation, our mechanism achieves better performance with much fewer labeled/unlabeled training examples. Second, compared to few-shot prompted LLMs, we achieve better performance using substantially smaller model sizes. Third, we reduce both the model size and the amount of data required to outperform LLMs; our finetuned 770M T5 model outperforms the few-shot prompted 540B PaLM model using only 80% of available data on a benchmark, whereas standard finetuning the same T5 model struggles to match even by using 100% of the dataset.

## From the paper (full-text)
**Contribution / method.** Use chain-of-thought prompting to extract both a predicted label ŷ and a natural-language rationale r̂ from a teacher LLM (540B PaLM; 20B GPT-NeoX in ablations) for each example. Train a small T5 student (220M / 770M / 11B) in a multi-task setup with task prefixes: a [label] task minimizes label-prediction loss, a [rationale] task minimizes rationale-generation loss, combined as L = L_label + λ·L_rationale. Crucially, at inference only the [label] prefix is used — the student needs neither the rationale nor the teacher at deployment. The multi-task formulation beats concatenating rationale+label into a single target (the single-task version sometimes does worse than plain finetuning).

**Results.** Across e-SNLI, ANLI, CQA, SVAMP: a 220M T5 (over 2000x smaller than 540B PaLM) outperforms few-shot CoT PaLM on e-SNLI; a 770M T5 (700x smaller) beats PaLM on ANLI and SVAMP. On data efficiency, Distilling step-by-step beats standard finetuning trained on 100% of e-SNLI using only 12.5% of the data; similar reductions of 75% (ANLI), 25% (CQA), 20% (SVAMP). The headline result: a 770M T5 outperforms 540B PaLM CoT on ANLI using only 80% of the labeled data, while standard finetuning of the same 770M model fails to match PaLM even with 100% of the data. In the unlabeled setting an 11B T5 matches or exceeds the 540B teacher on 3 of 4 datasets.

**Takeaway.** Distilling the model's reasoning trace as auxiliary multi-task supervision lets far smaller models beat far larger teachers with far less data — cutting both model size and annotation cost simultaneously.

## Graph
- **Concepts:** [[synthetic-data|Synthetic data]] · [[distillation|Distillation]]
- **Entities:** [[chain-of-thought]] · [[google]]
- **Raw:** `raw/arxiv/2305.02301.fulltext.md`
