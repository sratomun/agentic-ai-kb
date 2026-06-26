---
type: entity
entity_type: method
tags: [agents, method, data]
created: 2026-06-22
updated: 2026-06-22
---

# Tokenization

*How raw text is chopped into the discrete units a model actually trains and runs on — usually subword pieces via BPE or SentencePiece.*

## What it is
The pre-processing step that converts text into tokens (subword units) before [[pretraining]]. The dominant schemes are byte-pair encoding (BPE) and SentencePiece. The tokenizer is a quiet but consequential design choice: it sets vocabulary, sequence length, multilingual fairness, and how efficiently a model represents code, numbers, and non-English scripts.

## Why it matters
Tokenization is an underrated lever with outsized downstream effects — context-window economics, non-English performance, and arithmetic/coding quirks all trace back to it. For the exec it's mostly a "know it exists" node: when a model is oddly bad at a language or at digits, the tokenizer is often why, and it's effectively frozen once pre-training starts.

## Relationships
- precedes [[pretraining]]; part of the [[pretraining-data]] pipeline
- stage input to [[frontier-model-training]]

## Key papers (full-text ingested)
- [[2015-08-31-arxiv-1508-07909-bpe-subword-units|BPE Subword Units]] — byte-pair encoding for open-vocabulary models; the dominant scheme
- [[2018-08-19-arxiv-1808-06226-sentencepiece|SentencePiece]] — language-independent subword tokenizer; ~380x faster segmentation
