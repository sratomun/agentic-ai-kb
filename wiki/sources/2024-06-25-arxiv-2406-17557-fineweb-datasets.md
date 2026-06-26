---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale"
authors: Guilherme Penedo et al.
url: https://arxiv.org/abs/2406.17557
date: 2024-06-25
citationCount: 942
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale

**arXiv [2406.17557](https://arxiv.org/abs/2406.17557)** · 2024-06-25 · 942 citations · Guilherme Penedo et al.

**Significance.** The open-data corpus that closed the gap on frontier labs and made data curation a *documented, ablated science* — plus FineWeb-Edu showed LLM-graded educational filtering buys big reasoning gains for far fewer tokens.

## Abstract
The performance of a large language model (LLM) depends heavily on the quality and size of its pretraining dataset. However, the pretraining datasets for state-of-the-art open LLMs like Llama 3 and Mixtral are not publicly available and very little is known about how they were created. In this work, we introduce FineWeb, a 15-trillion token dataset derived from 96 Common Crawl snapshots that produces better-performing LLMs than other open pretraining datasets. To advance the understanding of how best to curate high-quality pretraining datasets, we carefully document and ablate all of the design choices used in FineWeb, including in-depth investigations of deduplication and filtering strategies. In addition, we introduce FineWeb-Edu, a 1.3-trillion token collection of educational text filtered from FineWeb. LLMs pretrained on FineWeb-Edu exhibit dramatically better performance on knowledge- and reasoning-intensive benchmarks like MMLU and ARC. Along with our datasets, we publicly release our data curation codebase and the models trained during our ablation experiments.

## From the paper (full-text)
**Contribution / method.** A fully documented pipeline (trafilatura WARC extraction, base filtering, per-snapshot MinHash dedup, selected C4 filters, and three custom statistically-derived heuristic filters), validated by 1.71B-param Llama-architecture ablations (>70 models, ~80,000 H100 GPU hours). FineWeb-Edu uses Llama-3-70B-Instruct to score 460,000 pages 0–5, trains a linear classifier on Snowflake-arctic-embed-m embeddings, and keeps score >= 3.
**Results.** FineWeb = **15T tokens**; base filtering alone yields ~36T tokens. Key dedup finding: **per-snapshot** MinHash (20T tokens) beat **global** dedup (4T tokens), which sometimes hurt by stripping high-quality data from older crawls. Custom filters removed 10.14% / 12.47% / 3.73% of tokens respectively and pushed FineWeb past C4. FineWeb-Edu = **1.3T tokens** and lifts MMLU from **33%→37%** and ARC from **46%→57%**, matching other large datasets' MMLU with ~**10x fewer tokens**.
**Takeaway.** Curation is a reproducible science now — and global dedup is not strictly better than per-snapshot; aggressive educational filtering trades raw size for reasoning.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2406.17557.fulltext.md`
