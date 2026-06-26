---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Internalizing Tool Knowledge in Small Language Models via QLoRA Fine-Tuning"
authors: Yuval Shemla et al.
url: https://arxiv.org/abs/2605.17774v2
date: 2026-05-18
score: 13
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, agent-memory, llm-as-judge, post-training]
---

# Internalizing Tool Knowledge in Small Language Models via QLoRA Fine-Tuning

**arXiv:** [2605.17774v2](https://arxiv.org/abs/2605.17774v2) · 2026-05-18 · cs.CL
**Authors:** Yuval Shemla et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models are increasingly used as planning components in agentic systems, but current tool-use pipelines often require full tool schemas to be included in every prompt, creating substantial token overhead and limiting the practicality of smaller models. This paper investigates whether tool-use knowledge can be internalized into small language models through parameter-efficient fine-tuning, enabling structured planning without explicit tool descriptions at inference time. Using AssetOpsBench as the primary benchmark, we fine-tune Gemma 4 E4B and Qwen3-4B with 8-bit QLoRA on approximately 1,700 tool-use examples spanning tool knowledge, question-to-plan mappings, and execution-style traces. We evaluate the resulting models under description-free inference, where the prompt omits the tool catalog entirely. The fine-tuned models outperform an informed unfine-tuned baseline that receives full tool descriptions, reducing input length by 82.6\% while improving structural and LLM-judge planning scores. In the best Gemma run, the model achieves an AT-F1 of 0.65 and an overall judge score of 3.88, compared with 0.47 and 2.88 for the informed baseline. Qwen3-4B achieves a strong overall judge score of 3.78 while using 62\% less memory and running 2.5$\times$ faster than Gemma, though it also exhibits greater catastrophic forgetting on general multiple-choice benchmarks. Additional ablations show that LoRA rank controls a quality--retention trade-off, with $r=32$ maximizing planning quality and smaller ranks preserving more general knowledge. These results suggest that, for fixed tool catalogs, QLoRA fine-tuning can shift tool knowledge from prompt context into model weights, substantially reducing inference overhead while maintaining or improving tool-planning quality.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[agent-memory]] · [[llm-as-judge]] · [[post-training]]
- **Entities:** [[gemma]] · [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.17774v2)
