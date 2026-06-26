---
type: source
source_type: arxiv
title: "Towards Verifiable Multimodal Deep Research: A Multi-Agent Harness for Interleaved Report Generation"
authors: Chenghao Zhang, Guanting Dong, Yufan Liu, Tong Zhao et al.
url: https://arxiv.org/abs/2605.29861v2
date: 2026-05-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.CL
tags: [agent-reliability, agent-protocols, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Towards Verifiable Multimodal Deep Research: A Multi-Agent Harness for Interleaved Report Generation

**arXiv:** [2605.29861v2](https://arxiv.org/abs/2605.29861v2) · 2026-05-28 · cs.CL
**Authors:** Chenghao Zhang, Guanting Dong, Yufan Liu, Tong Zhao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have advanced autonomous agents from deep search, which retrieves concise factual answers, to deep research, which synthesizes scattered evidence into long-form reports. However, verifiable multimodal deep research remains challenging due to open-ended synthesis without deterministic ground truth and the need to interleave textual arguments with visual evidence. We propose Ptah, a multi-agent harness for interleaved report generation. Ptah orchestrates the lifecycle from user query to rendered web report through planning, research, and writing stages, where specialized agents construct visual-aware plans, collect claim-grounded evidence, maintain source-aligned images in a Visual Working Memory, and compose reports through declarative multimodal tool use. A verifier agent serves as the harness's acceptance function, enforcing factual grounding, citation fidelity, and cross-modal consistency throughout the workflow. We further introduce PtahEval, an evaluation protocol that augments existing benchmarks with image-level and presentation-level assessments. Experiments on deep research benchmarks show that Ptah produces more reliable, visually informative, and usable human-facing multimodal reports than strong baselines. Our code is released at https://github.com/SnowNation101/Ptah

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.29861v2)
