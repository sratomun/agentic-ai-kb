---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Sequence-Level Knowledge Distillation"
authors: Yoon Kim et al.
url: https://arxiv.org/abs/1606.07947
date: 2016-06-25
ingested: 2026-06-22
tags: [arxiv, distillation]
---

# Sequence-Level Knowledge Distillation

**arXiv [1606.07947](https://arxiv.org/abs/1606.07947)** · 2016-06-25 · Yoon Kim, Alexander M. Rush (Harvard)

**Significance.** Extends knowledge distillation from word-level (per-token) matching to the sequence level for NMT, distilling a teacher's beam-search outputs into a student — and surprisingly eliminating the need for beam search at test time.

## Abstract
Neural machine translation (NMT) offers a novel alternative formulation of translation that is potentially simpler than statistical approaches. However to reach competitive performance, NMT models need to be exceedingly large. In this paper we consider applying knowledge distillation approaches (Bucila et al., 2006; Hinton et al., 2015) that have proven successful for reducing the size of neural models in other domains to the problem of NMT. We demonstrate that standard knowledge distillation applied to word-level prediction can be effective for NMT, and also introduce two novel sequence-level versions of knowledge distillation that further improve performance, and somewhat surprisingly, seem to eliminate the need for beam search (even when applied on the original teacher model). Our best student model runs 10 times faster than its state-of-the-art teacher with little loss in performance. It is also significantly better than a baseline model trained without knowledge distillation: by 4.2/1.7 BLEU with greedy decoding/beam search. Applying weight pruning on top of knowledge distillation results in a student model that has 13× fewer parameters than the original teacher model, with a decrease of 0.4 BLEU.

## From the paper (full-text)
**Contribution / method.** Three approaches. (1) **Word-KD**: the student matches the teacher's per-token distribution via cross-entropy. (2) **Seq-KD**: match the teacher's distribution over whole sequences, `L = −Σ_t q(t|s) log p(t|s)`; since that sum is exponential, approximate q by its mode found via **beam search** over the training set, then train the student with plain cross-entropy on this teacher-generated dataset. (3) **Seq-Inter**: fine-tune toward the beam hypothesis with the highest sentence-BLEU to the gold target (local updating). These are complementary and combinable.

**Results.** Teacher = 4×1000 LSTM (**221M params**); students = 2×500 (**84M**) and 2×300 (**49M**) on WMT'14 English→German. The 2×500 Seq-KD student reaches **BLEU 18.9 greedy (+4.2 over the 14.7 baseline)** and 19.0 with beam search; Seq-KD+Seq-Inter reaches 19.3 beam (+1.7). Seq-KD sharpens the student's distribution — the argmax accounts for **16.9% of probability mass vs 0.9%** for the baseline — which is why greedy decoding suffices. Seq-Inter applied to the same-size teacher lets **greedy decoding (19.6) match the teacher's beam search (19.5)**. Speed: 2×500 greedy runs at **1051.3 source words/sec vs 101.9** for the 4×1000 teacher with beam search — a **~10x speedup** — and the student runs on a Samsung Galaxy 6 (8.8 words/sec) where the teacher would not load. **Weight pruning** on the 2×500 student: pruning 80% → **17M params (13× fewer than the teacher) at only −0.4 BLEU**; pruning 90% → 8M params (26× fewer) at −1.0 BLEU.

**Takeaway.** Distilling at the sequence level concentrates the student around the teacher's mode, transferring global structure that word-level KD misses and making cheap greedy decoding competitive with expensive beam search.

## Graph
- **Concepts:** [[distillation|Distillation]]
- **Raw:** `raw/arxiv/1606.07947.fulltext.md`
