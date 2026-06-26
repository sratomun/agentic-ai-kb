---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Scaling Laws for Neural Language Models"
authors: Jared Kaplan et al.
url: https://arxiv.org/abs/2001.08361
date: 2020-01-23
ingested: 2026-06-22
tags: [arxiv, scaling-laws]
---

# Scaling Laws for Neural Language Models

**arXiv [2001.08361](https://arxiv.org/abs/2001.08361)** · 2020-01-23 · Jared Kaplan, Sam McCandlish, Tom Henighan, Tom B. Brown, Benjamin Chess, Rewon Child, Scott Gray, Alec Radford, Jeffrey Wu, Dario Amodei (Johns Hopkins, OpenAI)

**Significance.** The foundational paper showing Transformer LM loss falls as a clean power law in model size, data, and compute — and that compute is best spent on bigger models, not more data.

## Abstract

We study empirical scaling laws for language model performance on the cross-entropy loss. The loss scales as a power-law with model size, dataset size, and the amount of compute used for training, with some trends spanning more than seven orders of magnitude. Other architectural details such as network width or depth have minimal effects within a wide range. Simple equations govern the dependence of overfitting on model/dataset size and the dependence of training speed on model size. These relationships allow us to determine the optimal allocation of a fixed compute budget. Larger models are significantly more sample-efficient, such that optimally compute-efficient training involves training very large models on a relatively modest amount of data and stopping significantly before convergence.

## From the paper (full-text)

**Contribution / method.** An empirical study of decoder-only Transformer language models trained on WebText2, sweeping model size (~10^3 to ~10^9 non-embedding params), dataset size, and compute. The authors fit the cross-entropy loss (in nats) against each scale factor — number of non-embedding parameters N, dataset size D in tokens, and compute C (estimated as C ≈ 6·N·B·S, quoted in PF-days) — and derive simple equations governing overfitting, training-curve shape, and the optimal way to split a fixed compute budget. Model shape (depth vs. width, number of attention heads) is shown to matter very little within a wide range.

**Results.** Loss follows a power law in each factor when the other two are not bottlenecks:
- **Model size:** L(N) = (N_c / N)^α_N, with **α_N ≈ 0.076** and N_c ≈ 8.8 × 10^13 non-embedding params (Eq. 1.1). Doubling N reduces loss by a factor 2^(−α_N) = 0.95.
- **Dataset size:** L(D) = (D_c / D)^α_D, with **α_D ≈ 0.095** and D_c ≈ 5.4 × 10^13 tokens (Eq. 1.2).
- **Compute:** L(C_min) = (C_min_c / C_min)^α_C, with **α_C ≈ 0.050** and C_min_c ≈ 3.1 × 10^8 PF-days (Eq. 1.3).

These hold across eight orders of magnitude in C_min, six in N, and over two in D. Joint N–D dependence (overfitting): L(N,D) = [ (N_c/N)^(α_N/α_D) + D_c/D ]^α_D (Eq. 1.5); the penalty tracks the ratio N^0.74/D — every 8x increase in model size needs only ~5x more data to avoid a penalty, since data should grow sublinearly as D ∝ N^(α_N/α_D) ∼ N^0.74. Training curves fit L(N,S) = (N_c/N)^α_N + (S_c/S_min)^α_S with S_c ≈ 2.1 × 10^3 and α_S ≈ 0.76 (Eq. 1.6). Critical batch size B_crit(L) = B_∗/L^(1/α_B), with B_∗ ≈ 2 × 10^8 tokens and α_B ≈ 0.21 (~1–2M tokens at convergence). Optimal allocation of a fixed compute budget: **N ∝ C_min^0.73, B ∝ C_min^0.24, S ∝ C_min^0.03**, with data requirements growing only as D ∼ C^0.27 — so extra compute should go almost entirely into bigger models, not longer training or much more data.

**Takeaway.** Within a fixed compute budget, train a very large model and stop well short of convergence — large models are more sample-efficient, and the bulk of added compute (N ∝ C^0.73) should buy model size rather than data or training steps.

## Graph
- **Concepts:** [[scaling-laws|Scaling laws]]
- **Raw:** `raw/arxiv/2001.08361.fulltext.md`
