---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Training Compute-Optimal Large Language Models"
authors: Jordan Hoffmann et al.
url: https://arxiv.org/abs/2203.15556
date: 2022-03-29
citationCount: omit
tags: [arxiv, scaling-laws]
---

# Training Compute-Optimal Large Language Models

**arXiv [2203.15556](https://arxiv.org/abs/2203.15556)** · 2022-03-29 · Jordan Hoffmann et al. (DeepMind)

**Significance.** The "Chinchilla" result: for a fixed compute budget, model size and training tokens should scale equally — most large models of the era were badly under-trained.

## Abstract
We investigate the optimal model size and number of tokens for training a transformer language model under a given compute budget. We find that current large language models are significantly under-trained, a consequence of the recent focus on scaling language models whilst keeping the amount of training data constant. By training over 400 language models ranging from 70 million to over 16 billion parameters on 5 to 500 billion tokens, we find that for compute-optimal training, the model size and the number of training tokens should be scaled equally: for every doubling of model size the number of training tokens should also be doubled. We test this hypothesis by training a predicted compute-optimal model, Chinchilla, that uses the same compute budget as Gopher but with 70B parameters and 4× more data. Chinchilla uniformly and significantly outperforms Gopher (280B), GPT-3 (175B), Jurassic-1 (178B), and Megatron-Turing NLG (530B) on a large range of downstream evaluation tasks. This also means that Chinchilla uses substantially less compute for fine-tuning and inference, greatly facilitating downstream usage. As a highlight, Chinchilla reaches a state-of-the-art average accuracy of 67.5% on the MMLU benchmark, greater than a 7% improvement over Gopher.

## From the paper (full-text)
**Contribution / method.** Estimate the compute-optimal frontier (trade-off between parameters N and training tokens D at fixed FLOPs) via three independent approaches: (1) fix model sizes, vary training tokens, take the minimum over training curves; (2) IsoFLOP profiles — vary model size at fixed FLOP counts; (3) fit a parametric loss L(N,D) = E + A/N^α + B/D^β. Over 400 models trained, 70M to >16B params, on 5–500B tokens.

**Results.** All three approaches agree that N_opt and D_opt scale with compute at roughly equal exponents — Approach 1: a=0.50, b=0.50; Approach 2: a=0.49, b=0.51; Approach 3: a=0.46, b=0.54 (versus Kaplan et al. 2020's a=0.73, b=0.27). So for every doubling of model size, training tokens should also double (≈20 tokens/param at Chinchilla scale: 70B params → 1.4T tokens). The predicted compute-optimal model, Chinchilla (70B, 1.4T tokens), uses the same FLOP budget as Gopher yet uniformly beats Gopher (280B), GPT-3 (175B), Jurassic-1 (178B), and MT-NLG (530B). MMLU 5-shot: Chinchilla 67.6% vs Gopher 60.0% vs GPT-3 43.9% (abstract cites 67.5%, a >7% gain over Gopher). BIG-bench: 65.1% vs Gopher 54.4% (+10.7%). WikiText103 perplexity 7.16 vs Gopher 7.75.

**Takeaway.** Spend a fixed compute budget on a smaller model trained on far more data — under-training, not under-sizing, was the binding constraint.

## Graph
- **Concepts:** [[scaling-laws|Scaling laws]]
- **Entities:** Chinchilla, Gopher, DeepMind, MMLU
- **Raw:** `raw/arxiv/2203.15556.fulltext.md`
