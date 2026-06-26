---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Distilling the Knowledge in a Neural Network"
authors: Geoffrey Hinton et al.
url: https://arxiv.org/abs/1503.02531
date: 2015-03-09
citationCount: 22238
ingested: 2026-06-22
tags: [arxiv, distillation]
---

# Distilling the Knowledge in a Neural Network

**arXiv [1503.02531](https://arxiv.org/abs/1503.02531)** · 2015-03-09 · ~22,238 citations (Semantic Scholar) · Geoffrey Hinton, Oriol Vinyals, Jeff Dean

**Significance.** The paper that named and generalized "knowledge distillation" — training a small model to match a large model's temperature-softened soft targets, the foundation for nearly all later model-compression work.

## Abstract
A very simple way to improve the performance of almost any machine learning algorithm is to train many different models on the same data and then to average their predictions. Unfortunately, making predictions using a whole ensemble of models is cumbersome and may be too computationally expensive to allow deployment to a large number of users, especially if the individual models are large neural nets. Caruana and his collaborators have shown that it is possible to compress the knowledge in an ensemble into a single model which is much easier to deploy and we develop this approach further using a different compression technique. We achieve some surprising results on MNIST and we show that we can significantly improve the acoustic model of a heavily used commercial system by distilling the knowledge in an ensemble of models into a single model. We also introduce a new type of ensemble composed of one or more full models and many specialist models which learn to distinguish fine-grained classes that the full models confuse. Unlike a mixture of experts, these specialist models can be trained rapidly and in parallel.

## From the paper (full-text)
**Contribution / method.** "Distillation": raise the temperature T of the teacher's final softmax (`q_i = exp(z_i/T) / Σ_j exp(z_j/T)`) to produce soft targets, then train the small student to match them at the same high T (deploying at T=1). The training objective is a weighted sum of two cross-entropies — soft targets at high T, plus the correct labels at T=1 with a much lower weight — and soft-target gradients are scaled by T² since they fall off as 1/T². The paper proves that matching logits is the high-temperature special case of distillation. Also introduces specialist ensembles: a generalist plus many class-specialist models trained rapidly and in parallel.

**Results.** MNIST: a large 2×1200-ReLU net got **67 test errors**; a plain 2×800-ReLU net got **146**; the small net regularized only by matching the large net's soft targets at **temperature 20** got **74 errors** — recovering most of the gap. Even with all examples of the digit "3" removed from the transfer set, after a bias correction the distilled model got **98.6% of test 3s correct**. Speech (Android voice-search acoustic model, ~85M params, 8×2560 ReLU, 14,000 HMM-state labels): baseline frame accuracy **58.9%** / WER **10.9%**; a 10-model ensemble **61.1%** / **10.7%**; the distilled single model **60.8%** / **10.7%** — transferring **>80%** of the ensemble's frame-accuracy gain into one same-size net. Soft targets as regularizer: with only **3% of the speech data**, hard-target training overfits to **44.5%** test frame accuracy while soft-target training reaches **57.0%** (vs 58.9% on full data). JFT (100M images, 15,000 labels): adding **61 specialist models** raised top-1 test accuracy from **25.0% to 26.1%**.

**Takeaway.** The "dark knowledge" in a teacher's full probability distribution — the relative weights it puts on wrong answers — is what transfers, and high-temperature softmax is the lever that exposes it.

## Graph
- **Concepts:** [[distillation|Distillation]]
- **Raw:** `raw/arxiv/1503.02531.fulltext.md`
