---
type: source
source_type: arxiv
title: "Agentic Spatio-Temporal Grounding via Collaborative Reasoning"
authors: Heng Zhao, Yew-Soon Ong, Joey Tianyi Zhou
url: https://arxiv.org/abs/2602.13313v1
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CV
tags: [agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Agentic Spatio-Temporal Grounding via Collaborative Reasoning

**arXiv:** [2602.13313v1](https://arxiv.org/abs/2602.13313v1) · 2026-02-10 · cs.CV
**Authors:** Heng Zhao, Yew-Soon Ong, Joey Tianyi Zhou

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Spatio-Temporal Video Grounding (STVG) aims to retrieve the spatio-temporal tube of a target object or person in a video given a text query. Most existing approaches perform frame-wise spatial localization within a predicted temporal span, resulting in redundant computation, heavy supervision requirements, and limited generalization. Weakly-supervised variants mitigate annotation costs but remain constrained by the dataset-level train-and-fit paradigm with an inferior performance. To address these challenges, we propose the Agentic Spatio-Temporal Grounder (ASTG) framework for the task of STVG towards an open-world and training-free scenario. Specifically, two specialized agents SRA (Spatial Reasoning Agent) and TRA (Temporal Reasoning Agent) constructed leveraging on modern Multimoal Large Language Models (MLLMs) work collaboratively to retrieve the target tube in an autonomous and self-guided manner. Following a propose-and-evaluation paradigm, ASTG duly decouples spatio-temporal reasoning and automates the tube extraction, verification and temporal localization processes. With a dedicate visual memory and dialogue context, the retrieval efficiency is significantly enhanced. Experiments on popular benchmarks demonstrate the superiority of the proposed approach where it outperforms existing weakly-supervised and zero-shot approaches by a margin and is comparable to some of the fully-supervised methods.

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13313v1)
