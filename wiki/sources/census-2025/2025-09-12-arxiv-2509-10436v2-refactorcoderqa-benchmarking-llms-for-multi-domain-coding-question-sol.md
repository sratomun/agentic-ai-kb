---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "RefactorCoderQA: Benchmarking LLMs for Multi-Domain Coding Question Solutions in Cloud and Edge Deployment"
authors: Shadikur Rahman et al.
url: https://arxiv.org/abs/2509.10436v2
date: 2025-09-12
score: 5
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, reasoning-models, multi-agent-systems]
---

# RefactorCoderQA: Benchmarking LLMs for Multi-Domain Coding Question Solutions in Cloud and Edge Deployment

**arXiv:** [2509.10436v2](https://arxiv.org/abs/2509.10436v2) · 2025-09-12 · cs.CL
**Authors:** Shadikur Rahman et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
To optimize the reasoning and problem-solving capabilities of Large Language Models (LLMs), we propose a novel cloud-edge collaborative architecture that enables a structured multi-agent prompting framework. This framework comprises three specialized components: GuideLLM, a lightweight model deployed at the edge to provide methodological guidance; SolverLLM, a more powerful model hosted in the cloud and responsible for generating code solutions; and JudgeLLM, an automated evaluator for assessing solution correctness and quality. To evaluate and demonstrate the effectiveness of this architecture in realistic settings, we introduce RefactorCoderQA, a comprehensive benchmark designed to evaluate and enhance the performance of LLMs across multi-domain coding tasks. Motivated by the limitations of existing benchmarks, RefactorCoderQA systematically covers multiple technical domains, including Software Engineering, Data Science, Machine Learning, and Natural Language Processing, using authentic coding challenges sourced from Stack Overflow. We propose RefactorCoder-MoE, a fine-tuned mixture-of-experts (MoE) code language model based on DeepSeek-Coder-7B-Instruct, adapted to the RefactorCoderQA benchmark using QLoRA for domain-specific coding question answering. Extensive experiments demonstrate that RefactorCoder-MoE achieves strong and competitive performance, significantly outperforming all evaluated open-source and commercial baselines, with an overall accuracy of 76.84%.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]] · [[multi-agent-systems]]
- **Entities:** [[deepseek]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2509.10436v2)
