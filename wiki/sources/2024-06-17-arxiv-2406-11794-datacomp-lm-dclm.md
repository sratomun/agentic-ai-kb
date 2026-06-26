---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DataComp-LM: In search of the next generation of training sets for language models"
authors: Jeffrey Li et al.
url: https://arxiv.org/abs/2406.11794
date: 2024-06-17
citationCount: 348
ingested: 2026-06-22
tags: [arxiv, pretraining-data, data]
---

# DataComp-LM: In search of the next generation of training sets for language models

**arXiv [2406.11794](https://arxiv.org/abs/2406.11794)** · 2024-06-17 · 348 citations · Jeffrey Li et al.

**Significance.** Turned data curation itself into a controlled benchmark: fix the model and compute, vary only the data. Its big result — model-based filtering with a simple fastText classifier — produced an open-data 7B that rivals Llama 3 8B at a fraction of the compute.

## Abstract
We introduce DataComp for Language Models (DCLM), a testbed for controlled dataset experiments with the goal of improving language models. As part of DCLM, we provide a standardized corpus of 240T tokens extracted from Common Crawl, effective pretraining recipes based on the OpenLM framework, and a broad suite of 53 downstream evaluations. Participants in the DCLM benchmark can experiment with data curation strategies such as deduplication, filtering, and data mixing at model scales ranging from 412M to 7B parameters. As a baseline for DCLM, we conduct extensive experiments and find that model-based filtering is key to assembling a high-quality training set. The resulting dataset, DCLM-Baseline, enables training a 7B parameter language model from scratch to 64% 5-shot accuracy on MMLU with 2.6T training tokens. Compared to MAP-Neo, the previous state-of-the-art in open-data language models, DCLM-Baseline represents a 6.6 percentage point improvement on MMLU while being trained with 40% less compute. Our baseline model is also comparable to Mistral-7B-v0.3 and Llama 3 8B on MMLU (63% & 66%), and performs similarly on an average of 53 natural language understanding tasks while being trained with 6.6x less compute than Llama 3 8B. Our results highlight the importance of dataset design for training language models and offer a starting point for further research on data curation.

## From the paper (full-text)
**Contribution / method.** DCLM-POOL is **240T tokens** from Common Crawl, extracted with **resiliparse** (chosen over WET/trafilatura — better quality, **8x faster** than trafilatura). Fixed OpenLM training recipe across five scales (412M/8.2B → 7B/276B tokens) and 53 downstream evals (MMLU 5-shot, CORE, EXTENDED). DCLM-BASELINE built via ablations on extraction, dedup (Bloom filter ≈ MinHash+SuffixArray but more scalable), and model-based filtering.
**Results.** Model-based filtering is the key lever — different filter models span **35%→44% MMLU** at 7B. A simple fastText classifier trained on instruction-formatted positives (OpenHermes 2.5 + high-scoring ELI5 posts) gave **+3.5pt CORE** over Wikipedia-sourced positives; keeping the top **10%** by score was best. DCLM-BASELINE 7B on **2.6T tokens** hits **64% MMLU** — **+6.6pt over MAP-Neo** with **40% less compute**, comparable to Llama 3 8B (66%) with **6.6x less compute**, and **+5pt over Llama 2 7B** at 280B tokens with **7x less compute**. Mixing in "high-quality" curated sources surprisingly *hurt*; human quality judgments correlated poorly with LM gains.
**Takeaway.** With model fixed, the data is the model — and the reference data used to train a cheap filter matters more than filter complexity.

## Graph
- **Concepts:** [[pretraining-data|Pre-training data]]
- **Raw:** `raw/arxiv/2406.11794.fulltext.md`
