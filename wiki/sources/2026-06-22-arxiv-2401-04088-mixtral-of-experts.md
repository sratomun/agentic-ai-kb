---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Mixtral of Experts"
authors: Albert Q. Jiang et al.
url: https://arxiv.org/abs/2401.04088
date: 2024-01-08
ingested: 2026-06-22
tags: [arxiv, mixture-of-experts]
---

# Mixtral of Experts

**arXiv [2401.04088](https://arxiv.org/abs/2401.04088)** · 2024-01-08 · Albert Q. Jiang, Alexandre Sablayrolles, Arthur Mensch, Guillaume Lample, et al. (Mistral AI)

**Significance.** First open-weights sparse MoE to reach SOTA among open models — matches/beats Llama 2 70B and GPT-3.5 while activating only 13B params per token.

## Abstract
We introduce Mixtral 8x7B, a Sparse Mixture of Experts (SMoE) language model. Mixtral has the same architecture as Mistral 7B, with the difference that each layer is composed of 8 feedforward blocks (i.e. experts). For every token, at each layer, a router network selects two experts to process the current state and combine their outputs. Even though each token only sees two experts, the selected experts can be different at each timestep. As a result, each token has access to 47B parameters, but only uses 13B active parameters during inference. Mixtral was trained with a context size of 32k tokens and it outperforms or matches Llama 2 70B and GPT-3.5 across all evaluated benchmarks. In particular, Mixtral vastly outperforms Llama 2 70B on mathematics, code generation, and multilingual benchmarks. We also provide a model fine-tuned to follow instructions, Mixtral 8x7B – Instruct, that surpasses GPT-3.5 Turbo, Claude-2.1, Gemini Pro, and Llama 2 70B – chat model on human benchmarks. Both the base and instruct models are released under the Apache 2.0 license.

## From the paper (full-text)
**Contribution / method.** A decoder-only transformer (32 layers, dim 4096, hidden_dim 14336) where each FFN sub-block is replaced by a sparse MoE layer of 8 experts. A router computes `G(x) = Softmax(TopK(x·W_g))` with K=2, so each token is routed to 2 of 8 SwiGLU experts and their outputs are combined additively. Increasing the expert count n while holding K fixed grows total ("sparse") parameters while keeping per-token compute ("active" parameters) roughly constant. Trained at 32k context; runs efficiently via Megablocks sparse-matmul CUDA kernels and Expert Parallelism.

**Results.** 8 experts per layer, top-2 routing → **47B total parameters but only 13B active per token** (≈5x fewer active params than Llama 2 70B). On the head-to-head benchmark table Mixtral hits MMLU 70.6%, GSM8K 74.4%, MATH 28.4%, HumanEval 40.2%, MBPP 60.7% — beating Llama 2 70B (MMLU 69.9, GSM8K 69.6, MATH 13.8, HumanEval 29.3, MBPP 49.8) on almost every metric. Vs GPT-3.5: MMLU 70.6 vs 70.0, MBPP 60.7 vs 52.2, GSM-8K 58.4 vs 57.1. 100% passkey retrieval accuracy across the full 32k context. Mixtral 8x7B – Instruct scores **8.30 on MT-Bench** and reaches Arena Elo 1121, ahead of GPT-3.5-Turbo (1117), Claude-2.1 (1117), Gemini Pro (1111), and Llama-2-70b-chat (1077). Less bias than Llama 2 70B (BBQ 56.0% vs 51.5%).

**Takeaway.** Sparse routing decouples capacity from inference cost: you can ship 70B-class quality at 13B-class active compute, with open weights under Apache 2.0.

## Graph
- **Concepts:** [[mixture-of-experts|Mixture-of-Experts]]
- **Entities:** [[mistral]]
- **Raw:** `raw/arxiv/2401.04088.fulltext.md`
