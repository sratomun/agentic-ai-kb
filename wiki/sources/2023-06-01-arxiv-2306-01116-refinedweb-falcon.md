---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The RefinedWeb Dataset for Falcon LLM: Outperforming Curated Corpora with Web Data, and Web Data Only"
authors: Guilherme Penedo et al.
url: https://arxiv.org/abs/2306.01116
date: 2023-06-01
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# The RefinedWeb Dataset for Falcon LLM: Outperforming Curated Corpora with Web Data, and Web Data Only

**arXiv [2306.01116](https://arxiv.org/abs/2306.01116)** · 2023-06-01 · Guilherme Penedo et al.

**Significance.** The inflection point in the data-stage story: it showed *web-only* data, properly filtered and deduplicated, can match or beat hand-curated corpora — flipping the curated-data orthodoxy and removing the data bottleneck for scaling.

## Abstract
Large language models are commonly trained on a mixture of filtered web data and curated high-quality corpora, such as social media conversations, books, or technical papers. This curation process is believed to be necessary to produce performant models with broad zero-shot generalization abilities. However, as larger models requiring pretraining on trillions of tokens are considered, it is unclear how scalable is curation and whether we will run out of unique high-quality data soon. At variance with previous beliefs, we show that properly filtered and deduplicated web data alone can lead to powerful models; even significantly outperforming models from the state-of-the-art trained on The Pile. Despite extensive filtering, the high-quality data we extract from the web is still plentiful, and we are able to obtain five trillion tokens from CommonCrawl. We publicly release an extract of 600 billion tokens from our RefinedWeb dataset, and 1.3/7.5B parameters language models trained on it.

## From the paper (full-text)
**Contribution / method.** The Macrodata Refinement (MDR) pipeline: (1) document prep — URL blocklist+scoring, Trafilatura extraction, fastText language ID; (2) filtering — repetition removal, document-wise quality heuristics, line-wise corrections; (3) deduplication — fuzzy MinHash, exact-substring suffix arrays, and URL dedup across CommonCrawl dumps. Models are decoder-only GPT-3-style (1B/3B/7B) with ALiBi, FlashAttention, multi-query attention.
**Results.** The pipeline retains only ~**11.67%** of raw CommonCrawl, yielding ~**5 trillion tokens** of English text (a **600B-token** extract released). RefinedWeb-trained models significantly outperform Pile-trained models and the 7B model matches GPT-3 on the core zero-shot aggregate using web data only. Ablations: filtering (RW-F) consistently beats unfiltered (RW-Raw) with a widening gap during training; deduplication improves performance across compute budgets; applying MDR dedup to OSCAR and C4 also lifts their downstream performance.
**Takeaway.** Curated corpora aren't required — aggressive filtering + dedup of pure web data is enough, and there's plenty of it (5T tokens).

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2306.01116.fulltext.md`
