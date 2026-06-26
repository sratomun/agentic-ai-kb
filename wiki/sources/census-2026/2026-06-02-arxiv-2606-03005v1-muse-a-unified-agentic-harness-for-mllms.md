---
type: source
source_type: arxiv
title: "MUSE: A Unified Agentic Harness for MLLMs"
authors: Jianglin Lu, Hailing Wang, Xu Ma, Qihua Dong et al.
url: https://arxiv.org/abs/2606.03005v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CV
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# MUSE: A Unified Agentic Harness for MLLMs

**arXiv:** [2606.03005v1](https://arxiv.org/abs/2606.03005v1) · 2026-06-02 · cs.CV
**Authors:** Jianglin Lu, Hailing Wang, Xu Ma, Qihua Dong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Despite rapid progress, multimodal large language models (MLLMs) still fail on tasks that humans solve effortlessly, such as navigating a grid maze from a screenshot or selecting the correct puzzle piece. Rather than retraining the model, we ask a complementary question: how much capability can be elicited from a frozen MLLM purely by improving the execution scaffold around it? We introduce MUSE, a multimodal unified structured execution harness that wraps any off-the-shelf MLLM with composable modules for task representation, visual processing, perception tool use, structured parsing, deterministic verification, and verifier-guided repair, without any model retraining. We evaluate MUSE across diverse benchmarks spanning visual spatial planning, visual perception, multimodal reasoning, and fine-grained visual discrimination, using multiple state-of-the-art MLLMs. MUSE delivers consistent gains over the bare model in all settings, with the largest jumps on challenging instances. Further analysis reveals that many MLLM failures arise from harness-level shortcomings rather than fundamental model deficits, and can be addressed through verifier-guided repair without touching the model. These findings highlight the agentic multimodal harness as a critical yet underexplored design dimension, offering an orthogonal avenue for improving MLLMs beyond model-centric optimization.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03005v1)
