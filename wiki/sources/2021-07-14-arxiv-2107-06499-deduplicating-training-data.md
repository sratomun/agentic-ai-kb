---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Deduplicating Training Data Makes Language Models Better"
authors: Katherine Lee et al.
url: https://arxiv.org/abs/2107.06499
date: 2021-07-14
citationCount: 885
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# Deduplicating Training Data Makes Language Models Better

**arXiv [2107.06499](https://arxiv.org/abs/2107.06499)** · 2021-07-14 · 885 citations · Katherine Lee et al.

**Significance.** The paper that made deduplication a non-negotiable pipeline step: it quantified hidden duplication and train-test leakage in standard corpora and showed dedup cuts verbatim memorization 10x while improving perplexity — every later pipeline (RefinedWeb, FineWeb, DCLM) dedups heavily because of this.

## Abstract
Existing language modeling datasets contain many near-duplicate examples and long repetitive substrings. As a result, over 1% of the unprompted output of language models trained on these datasets is copied verbatim from the training data. We develop two tools that allow us to deduplicate training datasets—for example removing from C4 a single 61-word English sentence that is repeated over 60,000 times. Deduplication allows us to train models that emit memorized text ten times less frequently and require fewer training steps to achieve the same or better accuracy. We can also reduce train-test overlap, which affects over 4% of the validation set of standard datasets, thus allowing for more accurate evaluation. Code for deduplication is released.

## From the paper (full-text)
**Contribution / method.** Two scalable tools: EXACTSUBSTR (concatenate the corpus, build a parallelized suffix array, remove duplicated substrings >= **50 BPE tokens**) and NEARDUP (MinHash over 5-grams — k=9,000, r=450 buckets of b=20 — verified by edit similarity > **0.8**, cluster by connected components). Duplicates spanning splits are kept in test/val and dropped from train. Models: 1.5B "XL" and 110M "base" GPT-2-style Transformers on the T5 codebase, trained on original vs deduplicated C4.
**Results.** Duplication is pervasive: NEARDUP near-duplicate fractions are RealNews **13.63%**, LM1B **4.86%**, C4 **3.04%**, Wiki-40B **0.39%**; EXACTSUBSTR removes **7.18%** of C4 tokens and **19.4%** of RealNews tokens. Train-test leakage: **4.6%** of C4's and **14.4%** of RealNews's validation sets had train-side duplicates. Memorization drops **10x** — from over **1%** verbatim unprompted tokens to ~**0.1%**; prompted reproduction of duplicated examples falls from over **40%** to ~**3–6%**. Deduplicated models match or beat perplexity on LM1B/Wiki-40B despite less data (~3-point Wiki-40B gain) and train faster (~5 hours saved over two C4 epochs on a 128-core TPU v3).
**Takeaway.** Dedup is pure upside: less memorization, cleaner evals, comparable-or-better perplexity, faster training — exact paragraph/URL dedup alone is not enough.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2107.06499.fulltext.md`
