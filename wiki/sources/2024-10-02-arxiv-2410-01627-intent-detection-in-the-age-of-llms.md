---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Intent Detection in the Age of LLMs"
authors: Gaurav Arora et al. (Amazon, IIT Jammu)
url: https://arxiv.org/abs/2410.01627
date: 2024-10-02
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-understanding, intent-routing, distillation, human-agent-interaction]
---

# Intent Detection in the Age of LLMs

**arXiv [2410.01627](https://arxiv.org/abs/2410.01627)** · 2024-10-02 · Amazon / IIT Jammu

**Significance.** The reference point for the "don't use an LLM for every utterance" thesis: a small sentence-transformer handles the bulk, an LLM is summoned only for the uncertain tail. This is the paper the [[intent-understanding]] hybrid-default claim is grounded in.

## Abstract
Intent detection is a critical component of task-oriented dialogue systems (TODS). This work evaluates seven Claude- and Mistral-family LLMs (adaptive ICL + chain-of-thought) against contrastively fine-tuned sentence transformers (SetFit) on open-source (HINT3: SOFMattress, Curekart, Powerplay11) and internal multi-label datasets, proposes a latency-aware hybrid system, and introduces a two-step method for out-of-scope (OOS) detection.

## From the paper (full-text)
**Contribution / method.** Three parts: (1) a benchmark of LLM intent detection with retrieval-augmented in-context learning and CoT prompting; (2) a **hybrid system** that routes each query to either [[setfit|SetFit]] (cheap, low-latency) or an LLM (accurate) based on the **uncertainty of SetFit's prediction**, estimated via Monte-Carlo Dropout; (3) a **two-step OOS method** — the LLM predicts an in-scope label, then the query's representation from the LLM decoder layer is compared to training-instance clusters for that label; distant → flagged OOS. No fine-tuning required.
**Results.** The hybrid system **reduced the SetFit→LLM accuracy gap to ~2%** on datasets with consistent train/test distribution while **cutting latency ~50%** versus LLM-only. The two-step OOS method improved OOS detection **>5%** over baseline. LLMs generalized better than SetFit under distribution shift (OADP); **Claude v3 Haiku** gave the best accuracy/latency balance; CoT consistently helped. Narrower intent scopes and smaller label spaces improved OOS detection across all models.
**Takeaway.** In production, intent resolution is an economics problem: reserve the LLM for the queries a cheap classifier is unsure about. ~2% accuracy for ~50% latency is the trade everyone is now copying.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[intent-routing|Intent routing]] · [[distillation]] · [[human-agent-interaction]]
- **Entities:** [[setfit]] · [[clinc150]] · [[banking77]] · [[anthropic]]
- **Raw:** abstract + full-text report (alphaXiv) read 2026-06-23
