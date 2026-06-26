---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer"
authors: Noam Shazeer et al.
url: https://arxiv.org/abs/1701.06538
date: 2017-01-23
ingested: 2026-06-22
tags: [arxiv, mixture-of-experts]
---

# Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer

**arXiv [1701.06538](https://arxiv.org/abs/1701.06538)** · 2017-01-23 · Noam Shazeer, Azalia Mirhoseini, Krzysztof Maziarz, Andy Davis, Quoc Le, Geoffrey Hinton, Jeff Dean

**Significance.** The paper that made conditional computation work in practice, introducing the sparsely-gated MoE layer that lets a network carry >1000x more capacity for only minor compute cost — the architectural ancestor of modern sparse-expert LLMs.

## Abstract
The capacity of a neural network to absorb information is limited by its number of parameters. Conditional computation, where parts of the network are active on a per-example basis, has been proposed in theory as a way of dramatically increasing model capacity without a proportional increase in computation. In practice, however, there are significant algorithmic and performance challenges. In this work, we address these challenges and finally realize the promise of conditional computation, achieving greater than 1000x improvements in model capacity with only minor losses in computational efficiency on modern GPU clusters. We introduce a Sparsely-Gated Mixture-of-Experts layer (MoE), consisting of up to thousands of feed-forward sub-networks. A trainable gating network determines a sparse combination of these experts to use for each example. We apply the MoE to the tasks of language modeling and machine translation, where model capacity is critical for absorbing the vast quantities of knowledge available in the training corpora. We present model architectures in which a MoE with up to 137 billion parameters is applied convolutionally between stacked LSTM layers. On large language modeling and machine translation benchmarks, these models achieve significantly better results than state-of-the-art at lower computational cost.

## From the paper (full-text)
**Contribution / method.** Introduces the Sparsely-Gated Mixture-of-Experts (MoE) layer: a set of n feed-forward expert sub-networks plus a trainable gating network whose output is a sparse n-dimensional vector (`y = Σ G(x)_i E_i(x)`). The key mechanism is **Noisy Top-K Gating** — add tunable Gaussian noise to the softmax logits, keep only the top k values (rest set to −∞ → gate value 0), so only a handful of experts compute per example while the noise term aids load balancing. The MoE is applied **convolutionally between stacked LSTM layers**, called once per text position. For very large expert counts they use a **two-level hierarchical MoE**. Two auxiliary losses (`L_importance` and `L_load`, each the squared coefficient of variation of importance/load) keep expert utilization balanced. Performance engineering: mix data + model parallelism (combine synchronous batches so each expert gets a `kbd/n` batch over d devices), exploit convolutionality, and keep one shared copy of each stationary expert to limit network-bandwidth costs.

**Results.** Language modeling, MoE inserted between two LSTM layers, all at ~8M ops/timestep: flat MoEs of 4/32/256 experts and hierarchical MoEs of 256/1024/4096 experts (each expert ~1M params, 4 active per input). On the **1B Word benchmark** the 4096-expert model cut test perplexity 24% vs the compute-matched baseline; higher-compute MoE models reached test perplexity **28.0** vs the best published **34.7/30.6**, while needing only **6%** of the computation. On the **100B Word Google News corpus** they trained MoE layers up to **131072 experts**, corresponding to **up to 137 billion parameters** in the MoE layer (largest model 137577.6M params). Perplexity improved up to **65536 experts (68 billion parameters)**, dropping **39% lower** than the compute-matched baseline (degraded at 131072 experts, likely too much sparsity); even at 65536 experts (99.994% layer sparsity) efficiency held at 0.72 TFLOPS/GPU. **Machine translation** used a modified GNMT with MoE layers (up to 2048 experts, ~2M params each, ~8B added params): on **WMT'14 En→Fr** the 2048-expert MoE hit **BLEU 40.56** (test perplexity 2.63), and on **WMT'14 En→De** **BLEU 26.03** — gains of **+1.34** and **+1.12 BLEU** over the strong GNMT baselines, at lower ops/timestep (85M vs 214M). Multilingual MoE: 19% lower dev perplexity than multilingual GNMT and beat it on 11 of 12 language pairs (by up to 5.84 BLEU). Trained on clusters of 16-128 Tesla K40 GPUs in TensorFlow.

**Takeaway.** Conditional computation finally pays off: a sparse top-k gate over thousands of experts buys >1000x model capacity for near-constant per-example compute, beating dense state-of-the-art at a fraction of the cost.

## Graph
- **Concepts:** [[mixture-of-experts|Mixture-of-Experts]]
- **Raw:** `raw/arxiv/1701.06538.fulltext.md`
