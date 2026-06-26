---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SentencePiece: A simple and language independent subword tokenizer and detokenizer for Neural Text Processing"
authors: Taku Kudo et al.
url: https://arxiv.org/abs/1808.06226
date: 2018-08-19
ingested: 2026-06-22
tags: [arxiv, tokenization, data]
---

# SentencePiece: A simple and language independent subword tokenizer and detokenizer for Neural Text Processing

**arXiv [1808.06226](https://arxiv.org/abs/1808.06226)** · 2018-08-19 · Taku Kudo, John Richardson (Google)

**Significance.** The tokenizer library that became the de-facto standard for production LLMs (T5, LLaMA, mT5, ALBERT, XLNet and many more). Its key move: train subword models directly from raw text, no language-specific pre-tokenization, with lossless, self-contained, reproducible models.

## Abstract
This paper describes SentencePiece, a language-independent subword tokenizer and detokenizer designed for Neural-based text processing, including Neural Machine Translation. It provides open-source C++ and Python implementations for subword units. While existing subword segmentation tools assume that the input is pre-tokenized into word sequences, SentencePiece can train subword models directly from raw sentences, which allows us to make a purely end-to-end and language independent system. We perform a validation experiment of NMT on English-Japanese machine translation, and find that it is possible to achieve comparable accuracy to direct subword training from raw sentences. We also compare the performance of subword training and segmentation with various configurations. SentencePiece is available under the Apache 2 license at https://github.com/google/sentencepiece.

## From the paper (full-text)
**Contribution / method.** SentencePiece bundles four components — Normalizer, Trainer, Encoder, Decoder — and supports two subword algorithms (BPE and the unigram language model). Three design choices matter: (1) **Lossless tokenization** — treat input as a raw Unicode sequence, escape whitespace as the meta symbol _ (U+2581), so Decode(Encode(Normalize(text))) == Normalize(text); detokenization is just `''.join(tokens).replace('_',' ')`. (2) **Direct training from raw sentences** — no language-specific pre-tokenization required, important for non-segmented languages (Chinese/Japanese/Korean). (3) **Self-contained models** — the model file embeds vocabulary, segmentation parameters, and the pre-compiled finite-state transducer for NFKC-style normalization, guaranteeing reproducibility with no external dependencies. Specifies a target vocabulary size (rather than a merge count) and uses an O(N log N) heap-based BPE (vs. naive O(N^2)).

**Results.** On the KFTT English↔Japanese task (GNMT, 440k train sentences, shared 8k vocab, case-sensitive BLEU): SentencePiece beats the 80k word-model baseline — ja→en 29.55 vs. 28.24, en→ja 21.62 vs. 20.06. Pre-tokenization is not always needed: en→ja actually degrades to 20.86 with pre-tokenization. On segmentation speed (16k vocab), training subword models on raw Japanese is ~217s vs. subword-nmt's 528s, and at segmentation time SentencePiece runs about 380x faster than subword-nmt on raw Japanese (5.9s vs. 216.2s), reaching ~21k (EN) / ~74k (JA) sentences/sec — fast enough for on-the-fly processing. BPE and unigram LM give almost comparable accuracy.

**Takeaway.** Move tokenization from a brittle, language-specific offline preprocessing step into a fast, lossless, self-contained model that trains straight from raw text — the engineering foundation for language-agnostic, reproducible LLM pipelines.

## Graph
- **Concepts:** [[tokenization]]
- **Entities:** [[google]]
- **Raw:** `raw/arxiv/1808.06226.fulltext.md`
