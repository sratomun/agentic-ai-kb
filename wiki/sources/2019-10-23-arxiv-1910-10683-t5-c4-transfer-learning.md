---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer"
authors: Colin Raffel et al.
url: https://arxiv.org/abs/1910.10683
date: 2019-10-23
citationCount: 26155
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer

**arXiv [1910.10683](https://arxiv.org/abs/1910.10683)** · 2019-10-23 · 26155 citations · Colin Raffel et al.

**Significance.** The paper that introduced C4 (~750 GB cleaned Common Crawl), the open web corpus that became the baseline every later data paper (RefinedWeb, FineWeb, DCLM) measures against — and proved that cleaning web data is non-optional.

## Abstract
Transfer learning, where a model is first pre-trained on a data-rich task before being fine-tuned on a downstream task, has emerged as a powerful technique in natural language processing (NLP). The effectiveness of transfer learning has given rise to a diversity of approaches, methodology, and practice. In this paper, we explore the landscape of transfer learning techniques for NLP by introducing a unified framework that converts all text-based language problems into a text-to-text format. Our systematic study compares pre-training objectives, architectures, unlabeled data sets, transfer approaches, and other factors on dozens of language understanding tasks. By combining the insights from our exploration with scale and our new "Colossal Clean Crawled Corpus", we achieve state-of-the-art results on many benchmarks covering summarization, question answering, text classification, and more. To facilitate future work on transfer learning for NLP, we release our data set, pre-trained models, and code.

## From the paper (full-text)
**Contribution / method.** A unified text-to-text framework (every task framed as text-in/text-out via task prefixes) plus a systematic "coordinate ascent" study over objectives, architectures, datasets, and fine-tuning. Introduces C4, a ~750 GB cleaned Common Crawl corpus built with heuristics: keep lines ending in terminal punctuation, drop pages with too few sentences, remove bad words / JavaScript / "lorem ipsum" / curly brackets / boilerplate, dedup 3-sentence spans, and keep English at >0.99 language-ID probability.
**Results.** Cleaning is essential — unfiltered Common Crawl markedly degraded performance. Training on a too-small repeated corpus (repeated thousands of times) hurt performance via memorization, motivating large datasets. The baseline span-corruption denoising objective (15% corruption, single sentinel token, predict only corrupted spans) was best and most efficient. Encoder-decoder beat decoder-only/prefix-LM; parameter sharing halved params at matched quality. Scaling to 11B params on ~1 trillion tokens gave SOTA on 18 of 24 tasks (GLUE, SuperGLUE, SQuAD, CNN/DM), with T5-11B near human SuperGLUE performance.
**Takeaway.** A clean, large web corpus (C4) plus systematic choices and scale — cleaning the web is a hard requirement, not a nicety.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/1910.10683.fulltext.md`
