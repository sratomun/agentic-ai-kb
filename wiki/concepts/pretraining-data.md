---
type: concept
tags: [agents, frontier-models, data]
created: 2026-06-22
updated: 2026-06-22
kind: domain
---

# Pre-training Data

*The corpus that makes the model: web-scale text, curated, filtered, deduplicated, and mixed — the most secretive and arguably highest-leverage input at a frontier lab.*

## What it is
The trillions of tokens a base model learns from, and the pipeline that produces them: sourcing (web crawl, code, books), quality filtering, deduplication, and domain mixing. The field's recurring lesson is that *curation beats raw quantity* — well-filtered web data can match or beat hand-curated corpora at scale. Borders [[synthetic-data]] (model-generated rather than scraped) and [[tokenization]] (how the text is chunked before training). Folds in data curation, dedup, and data-mixture work.

## Why it matters
Data is the input labs disclose least and guard most, which makes it the hardest part of the frontier to replicate and the most exposed to legal risk (copyright, licensing). For the exec the signal is twofold: data quality and mixture now drive more differentiation than raw scale, and the open datasets (FineWeb, DCLM) are closing the gap on the data side even as compute stays concentrated. Where a lab gets its data — and whether it can defend that legally — is a real strategic and risk variable, not a footnote.

## What the evidence shows
**Foundations.** The open-data lineage runs from The Pile (arXiv:2101.00027) and C4/T5 (arXiv:1910.10683) through RefinedWeb showing web-only data can beat curated corpora (arXiv:2306.01116), to FineWeb (arXiv:2406.17557) and DataComp-LM (arXiv:2406.11794) making curation itself the benchmark. Deduplication was shown to materially improve models (arXiv:2107.06499), and DoReMi established that *domain mixture weights* measurably change pre-training efficiency (arXiv:2305.10429).

**Recent developments.** This is new territory for the radar — local coverage is thin and arrives mostly as agent-flavored offshoots (data-mixing agents). The canonical data literature above carries the node; flag for the scanner to track the copyright/licensing strand, which is governance-adjacent → [[frontier-model-governance]].

## Relationships
- input to [[pretraining]]; stage of [[frontier-model-training]]
- complemented by [[synthetic-data]]; precedes [[tokenization]]
- legal/governance exposure tracked in [[frontier-model-governance]]

## Key papers (full-text ingested)
- [[2020-12-31-arxiv-2101-00027-the-pile-800gb-dataset|The Pile]] — 825GB / 22 curated subsets
- [[2019-10-23-arxiv-1910-10683-t5-c4-transfer-learning|T5 / C4]] — ~750GB cleaned Common Crawl; unfiltered CC markedly degrades quality
- [[2023-06-01-arxiv-2306-01116-refinedweb-falcon|RefinedWeb]] — web-only ~5T tokens; a 7B matches GPT-3 zero-shot
- [[2024-06-25-arxiv-2406-17557-fineweb-datasets|FineWeb]] — 15T tokens; FineWeb-Edu lifts MMLU 33→37% at ~10x fewer tokens
- [[2024-06-17-arxiv-2406-11794-datacomp-lm-dclm|DataComp-LM (DCLM)]] — 7B at 64% MMLU, ~Llama-3-8B at 6.6x less compute
- [[2023-05-17-arxiv-2305-10429-doremi-data-mixtures|DoReMi]] — learned domain weights: +6.5pt avg, 2.6x faster, ~8% of FLOPs
- [[2021-07-14-arxiv-2107-06499-deduplicating-training-data|Deduplicating Training Data]] — cuts verbatim memorization ~10x; C4 had 3% near-dupes
