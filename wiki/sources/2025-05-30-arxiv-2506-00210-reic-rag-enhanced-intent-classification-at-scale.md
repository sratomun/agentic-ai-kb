---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "REIC: RAG-Enhanced Intent Classification at Scale"
authors: Ziji Zhang et al. (Amazon)
url: https://arxiv.org/abs/2506.00210
date: 2025-05-30
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-understanding, intent-routing, agentic-rag, recommendation-agents]
---

# REIC: RAG-Enhanced Intent Classification at Scale

**arXiv [2506.00210](https://arxiv.org/abs/2506.00210)** · 2025-05-30 · Amazon

**Significance.** How you keep a fixed-taxonomy classifier alive when the taxonomy is huge and changes weekly: make it retrieval-augmented so new intents are an index update, not a retrain. The production-scale anchor for [[intent-understanding]].

## Abstract
REIC does intent classification for customer-service routing at Amazon scale: dense retrieval of similar (query, intent) pairs feeds a fine-tuned LLM that scores *only* the retrieved candidates via constrained decoding — grounding the prediction and letting the intent space grow without retraining.

## From the paper (full-text)
**Contribution / method.** Three stages: (1) **index** held-out (query, intent) pairs as MPNet sentence embeddings with hierarchical labels; (2) **retrieve** top-k nearest (query, intent) pairs by cosine similarity for an incoming query; (3) **score** with a fine-tuned **Mistral-7B** using **constrained decoding** — for each retrieved candidate intent, one forward pass yields a length-normalized log-prob, and the argmax wins. Because only retrieved candidates are scored, the LLM can't hallucinate an unavailable intent, and new intents are added by inserting rows in the vector index.
**Results.** Overall **F1 0.572**, beating RoBERTa 0.516, Claude+RAG 0.419, Claude few-shot 0.329, Mistral-classification 0.255. MPNet was the best retriever (0.564 vs BM25 0.532, ColBERTv2 0.542). **top-k=10** balanced accuracy vs latency (latency rises sharply with k). In production it gave **+3.38 pp absolute** customer positive-response rate and consolidated two fine-tuned models into one.
**Takeaway.** The fixed-taxonomy classifier survives at scale by becoming retrieval-grounded: dynamic intents, no retrain, no hallucinated labels.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[intent-routing|Intent routing]] · [[agentic-rag]] · [[recommendation-agents]]
- **Entities:** [[anthropic]]
- **Raw:** abstract + full-text report (alphaXiv) read 2026-06-23
