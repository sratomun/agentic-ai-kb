---
type: source
source_type: arxiv
title: "ASA: Backbone-Training-Free Representation Engineering for Tool-Calling Agents"
authors: Youjin Wang, Run Zhou, Yingjie Ma, Rong Fu et al.
url: https://arxiv.org/abs/2602.04935v3
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [agent-reliability, tool-use, arxiv, auto-ingested]
---

# ASA: Backbone-Training-Free Representation Engineering for Tool-Calling Agents

**arXiv:** [2602.04935v3](https://arxiv.org/abs/2602.04935v3) · 2026-02-04 · cs.SE
**Authors:** Youjin Wang, Run Zhou, Yingjie Ma, Rong Fu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Adapting LLM agents to domain-specific tool calling remains notably brittle under evolving interfaces. Prompt and schema engineering is easy to deploy but often fragile under distribution shift and strict parsers, while continual parameter-efficient fine-tuning improves reliability at the cost of training, maintenance, and potential forgetting. We identify a critical Lazy Agent failure mode where tool necessity is nearly perfectly decodable from mid-layer activations, yet the model remains conservative in entering tool mode, revealing a representation-behavior gap. We propose Activation Steering Adapter (ASA), a training-free, inference-time controller that performs a single-shot mid-layer intervention and targets tool domains via a router-conditioned mixture of steering vectors with a probe-guided signed gate to amplify true intent while suppressing spurious triggers. On MTU-Bench with Qwen2.5-1.5B, ASA improves strict tool-use F1 from 0.18 to 0.50 while reducing the false positive rate from 0.15 to 0.05, using only about 20KB of portable assets and no weight updates.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04935v3)
