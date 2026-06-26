---
type: source
source_type: arxiv
title: "HyFunc: Accelerating LLM-based Function Calls for Agentic AI through Hybrid-Model Cascade and Dynamic Templating"
authors: Weibin Liao, Jian-guang Lou, Haoyi Xiong
url: https://arxiv.org/abs/2602.13665v1
date: 2026-02-14
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [intent-routing, tool-use, distillation, arxiv, auto-ingested]
---

# HyFunc: Accelerating LLM-based Function Calls for Agentic AI through Hybrid-Model Cascade and Dynamic Templating

**arXiv:** [2602.13665v1](https://arxiv.org/abs/2602.13665v1) · 2026-02-14 · cs.AI
**Authors:** Weibin Liao, Jian-guang Lou, Haoyi Xiong

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
While agentic AI systems rely on LLMs to translate user intent into structured function calls, this process is fraught with computational redundancy, leading to high inference latency that hinders real-time applications. This paper identifies and addresses three key redundancies: (1) the redundant processing of a large library of function descriptions for every request; (2) the redundant use of a large, slow model to generate an entire, often predictable, token sequence; and (3) the redundant generation of fixed, boilerplate parameter syntax. We introduce HyFunc, a novel framework that systematically eliminates these inefficiencies. HyFunc employs a hybrid-model cascade where a large model distills user intent into a single "soft token." This token guides a lightweight retriever to select relevant functions and directs a smaller, prefix-tuned model to generate the final call, thus avoiding redundant context processing and full-sequence generation by the large model. To eliminate syntactic redundancy, our "dynamic templating" technique injects boilerplate parameter syntax on-the-fly within an extended vLLM engine. To avoid potential limitations in generalization, we evaluate HyFunc on an unseen benchmark dataset, BFCL. Experimental results demonstrate that HyFunc achieves an excellent balance between efficiency and performance. It achieves an inference latency of 0.828 seconds, outperforming all baseline models, and reaches a performance of 80.1%, surpassing all models with a comparable parameter scale. These results suggest that HyFunc offers a more efficient paradigm for agentic AI. Our code is publicly available at https://github.com/MrBlankness/HyFunc.

## Graph
- **Concepts:** [[intent-routing|Intent routing]] · [[tool-use|Tool use]] · [[distillation|Distillation]]
- **Entities:** [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13665v1)
