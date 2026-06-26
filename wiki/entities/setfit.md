---
type: entity
entity_type: method
tags: [agents, method, nlu]
created: 2026-06-23
updated: 2026-06-23
---

# SetFit

*Contrastive few-shot fine-tuning of sentence transformers — the cheap, fast intent classifier in the hybrid pattern.*

## What it is
SetFit fine-tunes a sentence-transformer with contrastive learning for few-shot text classification, no prompt or large LLM needed. It is the standard low-latency baseline for intent detection.

## Why it matters
SetFit is the "common case" half of the pragmatic hybrid: it answers the bulk of utterances in milliseconds, and an LLM is summoned only when SetFit's prediction is uncertain. That split is what delivers the **~2% accuracy gap for ~50% latency** result.

## Relationships
- baseline classifier in [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms|Intent Detection in the Age of LLMs]]
- common-case half of [[intent-understanding]]
- efficiency relative of [[distillation]]

## Cited by
- [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms]]
