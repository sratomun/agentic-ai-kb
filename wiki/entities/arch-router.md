---
type: entity
entity_type: model
tags: [agents, model, routing]
created: 2026-06-23
updated: 2026-06-23
---

# Arch-Router

*A 1.5B preference-aligned router that matches queries to natural-language Domain-Action policies — fast, accurate, reconfigurable without retraining.*

## What it is
Arch-Router (Qwen2.5-1.5B, by [[katanemo|Katanemo Labs]]) is a compact generative router that selects a route policy described in natural language, decoupling route selection from model assignment. Open-weighted on HuggingFace.

## Why it matters
It is the proof that intent-based routing can beat frontier models at routing while staying cheap: **93.17% routing score (+7.71%), ~51ms (~28× faster)**. The reference design for production [[intent-routing]].

## Relationships
- introduced by [[katanemo]]
- system for [[intent-routing]]
- consumes [[intent-understanding]]
- evaluated on [[clinc150]]
- open-source cousin of [[semantic-router]] · [[vllm-semantic-router]]

## Cited by
- [[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences]]
