---
type: source
source_type: arxiv
title: "Agentic Large Language Models for Training-Free Neuro-Radiological Image Analysis"
authors: Ayhan Can Erdur, Daniel Scholz, Jiazhen Pan, Benedikt Wiestler et al.
url: https://arxiv.org/abs/2604.16729v1
date: 2026-04-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CV
tags: [clinical-agents, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Agentic Large Language Models for Training-Free Neuro-Radiological Image Analysis

**arXiv:** [2604.16729v1](https://arxiv.org/abs/2604.16729v1) · 2026-04-17 · cs.CV
**Authors:** Ayhan Can Erdur, Daniel Scholz, Jiazhen Pan, Benedikt Wiestler et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
State-of-the-art large language models (LLMs) show high performance in general visual question answering. However, a fundamental limitation remains: current architectures lack the native 3D spatial reasoning required for direct analysis of volumetric medical imaging, such as CT or MRI. Emerging agentic AI offers a new solution, eliminating the need for intrinsic 3D processing by enabling LLMs to orchestrate and leverage specialized external tools. Yet, the feasibility of such agentic frameworks in complex, multi-step radiological workflows remains underexplored. In this work, we present a training-free agentic pipeline for automated brain MRI analysis. Validating our methodology on several LLMs (GPT-5.1, Gemini 3 Pro, Claude Sonnet 4.5) with off-the-shelf domain-specific tools, our system autonomously executes complex end-to-end workflows, including preprocessing (skull stripping, registration), pathology segmentation (glioma, meningioma, metastases), and volumetric analysis. We evaluate our framework across increasingly complex radiological tasks, from single-scan segmentation and volumetric reporting to longitudinal response assessment requiring multi-timepoint comparisons. We analyze the impact of architectural design by comparing single-agent models against multi-agent "domain-expert" collaborations. Finally, to support rigorous evaluation of future agentic systems, we introduce and release a benchmark dataset of image-prompt-answer tuples derived from public BraTS data. Our results demonstrate that agentic AI can solve highly neuro-radiological image analysis tasks through tool use without the need for training or fine-tuning.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16729v1)
