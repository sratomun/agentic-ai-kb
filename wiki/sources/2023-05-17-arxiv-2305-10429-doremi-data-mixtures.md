---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DoReMi: Optimizing Data Mixtures Speeds Up Language Model Pretraining"
authors: Sang Michael Xie et al.
url: https://arxiv.org/abs/2305.10429
date: 2023-05-17
citationCount: 372
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# DoReMi: Optimizing Data Mixtures Speeds Up Language Model Pretraining

**arXiv [2305.10429](https://arxiv.org/abs/2305.10429)** · 2023-05-17 · 372 citations · Sang Michael Xie et al.

**Significance.** Made *domain mixture weights* a first-class, optimizable input: a tiny proxy model picks the data recipe for a 30x larger model, no downstream tasks needed — the canonical reference for "mixture matters as much as filtering."

## Abstract
The mixture proportions of pretraining data domains (e.g., Wikipedia, books, web text) greatly affect language model (LM) performance. In this paper, we propose Domain Reweighting with Minimax Optimization (DoReMi), which first trains a small proxy model using group distributionally robust optimization (Group DRO) over domains to produce domain weights (mixture proportions) without knowledge of downstream tasks. We then resample a dataset with these domain weights and train a larger, full-sized model. In our experiments, we use DoReMi on a 280M-parameter proxy model to set the domain weights for training an 8B-parameter model (30x larger) more efficiently. On The Pile, DoReMi improves perplexity across all domains, even when it downweights a domain. DoReMi improves average few-shot downstream accuracy by 6.5% points over a baseline model trained using The Pile's default domain weights and reaches the baseline downstream accuracy 2.6x faster. On the GLaM dataset, DoReMi, which has no knowledge of downstream tasks, even matches the performance of using domain weights tuned on downstream tasks.

## From the paper (full-text)
**Contribution / method.** Three steps: (1) train a small reference LM (280M) on baseline weights; (2) train a same-size proxy with Group DRO to minimize the worst-case *excess loss* (proxy minus reference) across domains, keeping the trajectory-averaged domain weights; (3) train the large model (8B) on the reweighted data. The proxy model is discarded — only the weights transfer. Optimization is ~**8% of total FLOPs** for an 8B main model.
**Results.** On The Pile, DoReMi (280M proxy → 8B main) lifts average few-shot downstream accuracy by **6.5pt** over default Pile weights and reaches baseline accuracy **2.6x faster**, while *reducing perplexity across all 22 domains* (a Pareto improvement). It upweights Pile-CC and downweights ArXiv/PubMed Central/StackExchange. On GLaM, task-agnostic DoReMi matches oracle downstream-tuned weights (converging within 3 iterated rounds). Same-size proxy/main runs improve accuracy 2% and reach baseline **4x faster**; a 280M proxy helped the 8B model but a 1B proxy didn't improve further.
**Takeaway.** Optimize the mixture, not just the filter — a cheap proxy's robust domain weights transfer across a 30x scale gap and pay for themselves many times over.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2305.10429.fulltext.md`
