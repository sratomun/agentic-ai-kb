---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Arch-Router: Aligning LLM Routing with Human Preferences"
authors: Co Tran et al. (Katanemo Labs)
url: https://arxiv.org/abs/2506.16655
date: 2025-06-19
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-routing, intent-understanding, harness-engineering]
---

# Arch-Router: Aligning LLM Routing with Human Preferences

**arXiv [2506.16655](https://arxiv.org/abs/2506.16655)** · 2025-06-19 · Katanemo Labs

**Significance.** The production face of intent-based routing: a 1.5B model that reads the user's intent against natural-language route policies and beats frontier models at routing, at ~50ms. The keystone for [[intent-routing]].

## Abstract
Arch-Router reframes LLM routing as preference alignment. A compact 1.5B generative router (fine-tuned from Qwen2.5-1.5B) matches a query to a user-defined **Domain-Action** policy described in natural language, then a separate table maps the policy to a model — decoupling route selection from model assignment so models can be swapped without retraining.

## From the paper (full-text)
**Contribution / method.** Routing = $R = T \circ F$: $F$ picks a route policy $c$ for query $q$ from policy set $C$; $T$ maps $c$→model. Policies are `(name, natural-language description)` pairs in a two-level **Domain** (e.g. legal, finance) × **Action** (summarize, code-gen) taxonomy. The full policy set is passed in the prompt, so **new/edited routes are honored at inference time without retraining**. Trained by SFT on a two-phase synthetic pipeline (clean policy-grounded dialogues, then augmentation with irrelevance injection, policy modification, scenario mixing for multi-turn realism).
**Results.** Overall routing score **93.17%**, **+7.71% over the best average competitor**, beating Claude-sonnet-3.7 (92.79%), GPT-4o (89.74%), Gemini-2.0-flash (85.63%); base Qwen2.5-1.5B scored 20.69%. Span/conversation accuracy rose with context length (strong multi-turn intent tracking). Irrelevance detection 96.49%. **Latency 51±12 ms on an L40S — ~28× faster** than the closest proprietary model (510–1450 ms). Evaluated on CLINC-150, MANtIS, SGD, LMSYS-1M. Failures cluster on the first turn (initial-query ambiguity), then it's robust on follow-ups.
**Takeaway.** Intent classification as a routing primitive: small, fast, interpretable (NL policies are auditable), and reconfigurable without retraining — exactly the shape production teams want.

## Graph
- **Concepts:** [[intent-routing|Intent routing]] · [[intent-understanding|Intent understanding]] · [[harness-engineering]]
- **Entities:** [[arch-router]] · [[katanemo]] · [[clinc150]] · [[semantic-router]]
- **Raw:** abstract + full-text report (alphaXiv) read 2026-06-23
