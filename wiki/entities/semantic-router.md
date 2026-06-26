---
type: entity
entity_type: product
tags: [agents, product, routing, open-source]
created: 2026-06-23
updated: 2026-06-23
---

# semantic-router (aurelio-labs)

*The dominant open-source embedding-based intent router — nearest-neighbor over pre-encoded example utterances.*

## What it is
An open-source library (aurelio-labs) that routes by encoding example utterances per intent/route and matching incoming queries by vector nearest-neighbor — a "superfast decision layer" for LLMs and agents.

## Why it matters
It is the most-used embedding-router pattern in production and the open-source embodiment of the "cheap classifier for the common case" half of the hybrid. Much of the deployed [[intent-routing]] reality lives in libraries like this, not in papers.

## Relationships
- open-source pattern for [[intent-routing]]
- embedding cousin of [[arch-router]] · [[vllm-semantic-router]]
- realizes the common-case half of [[intent-understanding]]

## Cited by
- [[intent-routing]]
