---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Xmodel-2.5: 1.3B Data-Efficient Reasoning SLM"
authors: Yang Liu et al.
url: https://arxiv.org/abs/2511.19496v1
date: 2025-11-23
score: 8
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, reasoning-models]
---

# Xmodel-2.5: 1.3B Data-Efficient Reasoning SLM

**arXiv:** [2511.19496v1](https://arxiv.org/abs/2511.19496v1) · 2025-11-23 · cs.LG
**Authors:** Yang Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models deliver strong reasoning and tool-use skills, yet their computational demands make them impractical for edge or cost-sensitive deployments. We present \textbf{Xmodel-2.5}, a 1.3-billion-parameter small language model designed as a \emph{drop-in agent core}. Training with maximal-update parameterization ($μ$P) allows hyper-parameters tuned on a 20M-parameter proxy to transfer directly to the full model, even under the parameter-tied \emph{tie-word-embedding} architecture. A 1.4T-token Warmup--Stable--Decay curriculum is used, and we further show that \textbf{switching from AdamW to Muon during the decay phase} improves the 13-task reasoning average by 4.58\,\% while keeping every other hyper-parameter fixed, verifying that early AdamW stability can be paired with late Muon sharpening for better downstream performance. FP8-mixed-precision training balances accuracy and throughput. All checkpoints, recipes, and evaluation code are released under the Apache-2.0 license.\footnote{https://huggingface.co/XiaoduoAILab/Xmodel-2.5 and https://huggingface.co/XiaoduoAILab/Xmodel-2.5-history (training checkpoints).} Training code and evaluation harness: https://github.com/XiaoduoAILab/Xmodel-2.5.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.19496v1)
