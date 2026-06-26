---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Efficient Skill Grounding via Code Refactoring with Small Language Models"
authors: Sera Choi et al.
url: https://arxiv.org/abs/2606.07999v1
date: 2026-06-06
score: 4
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, clinical-agents, intent-routing]
---

# Efficient Skill Grounding via Code Refactoring with Small Language Models

**arXiv:** [2606.07999v1](https://arxiv.org/abs/2606.07999v1) · 2026-06-06 · cs.AI
**Authors:** Sera Choi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Effective skill grounding is essential for deploying reusable skills in embodied agents, as even minor embodiment or environmental differences can render an entire skill incompatible. This challenge is particularly pronounced in embodied settings, where agents must operate in dynamic, partially observable environments without access to large language models (LLMs). In this setting, reliance on LLMs is impractical, while small language models (sLMs) remain insufficient for the effective skill grounding required for reliable long-horizon control. We present RECENT, a refactoring-centric agent framework that enables efficient skill grounding with sLMs by decoupling skill semantics from embodiment- and environment-specific execution binding. By representing skills as executable code, RECENT preserves the semantic intent encoded in a skill's control structure while grounding it by modifying only execution bindings through localized refactoring, rather than regenerating code from scratch. We evaluate RECENT across diverse skill grounding scenarios spanning multiple robot embodiments in dynamic environments, demonstrating robust long-horizon performance when deployed with an sLM. Across all scenarios, RECENT achieves the best performance among sLM-based Code-as-Policies (CaP) methods and matches the task performance of LLM-based CaP.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[clinical-agents]] · [[intent-routing]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.07999v1)
