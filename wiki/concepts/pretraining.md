---
type: concept
tags: [agents, frontier-models, pretraining]
created: 2026-06-22
updated: 2026-06-22
kind: domain
---

# Pre-training

*The base-model stage: self-supervised next-token prediction over a web-scale corpus, producing the raw capability everything downstream refines.*

## What it is
The first and most expensive training stage, where a model learns language, world knowledge, and latent reasoning by predicting the next token across trillions of tokens of [[pretraining-data]]. The output is a *base model* — broadly capable but not yet steerable or aligned; that's what [[post-training]] fixes. Pre-training is where [[scaling-laws]] and architecture choices like [[mixture-of-experts]] are cashed in, and where most of the compute (and most of the moat) sits.

## Why it matters
Pre-training is the capability floor: post-training sharpens what the base model already latently knows but rarely creates genuinely new ability (the same finding that haunts reasoning RL — see [[reasoning-models]]). For the exec that's the strategic tell — base-model quality caps everything above it, but the 2025–26 evidence is that pure pre-training scaling is yielding diminishing returns, which is why labs pushed compute into post-training and inference-time reasoning instead. Whoever can still move the pre-training frontier (data + compute + architecture) holds the deepest moat; everyone else competes downstream.

## What the evidence shows
**Foundations.** Pre-training as the dominant paradigm dates to GPT-3 showing that scale alone unlocks few-shot capability (arXiv:2005.14165), with the loss-vs-compute relationship quantified by the Kaplan scaling laws (arXiv:2001.08361). Modern recipes are documented in the DeepSeek-V3 technical report — a ~14.8T-token base trained with a multi-token-prediction objective and an [[mixture-of-experts]] backbone (arXiv:2412.19437).

**Recent developments.** The 2025 retrospective reads pre-training as increasingly a *base layer* whose marginal returns shifted toward post-training and inference-time scaling → [[2025-12-30-blog-raschka-state-of-llms-2025]]; the reasoning-model lineage built directly on these bases → [[2025-02-05-blog-raschka-understanding-reasoning-llms]].

## Relationships
- stage of [[frontier-model-training]]
- consumes [[pretraining-data]], [[synthetic-data]], [[tokenization]]
- governed by [[scaling-laws]]; commonly uses [[mixture-of-experts]]
- produces base models for [[post-training]], [[reasoning-models]]
- explained by [[sebastian-raschka]]

## Key papers (full-text ingested)
- [[2020-05-28-arxiv-2005-14165-gpt3-few-shot-learners|GPT-3]] — 175B params on ~400B tokens (570GB filtered); TriviaQA 71.2% few-shot
- [[2026-06-22-arxiv-2001-08361-scaling-laws-for-neural-language-models|Scaling Laws (Kaplan)]] — loss is a power law in compute/data/params
- [[2026-06-22-arxiv-2412-19437-deepseek-v3-technical-report|DeepSeek-V3 Technical Report]] — 671B/37B-active MoE, 14.8T tokens, multi-token-prediction objective
