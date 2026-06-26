---
type: source
source_type: arxiv
title: "ET-Agent: Incentivizing Effective Tool-Integrated Reasoning Agent via Behavior Calibration"
authors: Yifei Chen, Guanting Dong, Zhicheng Dou
url: https://arxiv.org/abs/2601.06860v2
date: 2026-01-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [self-evolving-agents, tool-use, arxiv, auto-ingested]
---

# ET-Agent: Incentivizing Effective Tool-Integrated Reasoning Agent via Behavior Calibration

**arXiv:** [2601.06860v2](https://arxiv.org/abs/2601.06860v2) · 2026-01-11 · cs.AI
**Authors:** Yifei Chen, Guanting Dong, Zhicheng Dou

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) can extend their parameter knowledge limits by adopting the Tool-Integrated Reasoning (TIR) paradigm. However, existing LLM-based agent training framework often focuses on answers' accuracy, overlooking specific alignment for behavior patterns. Consequently, agent often exhibits ineffective actions during TIR tasks, such as redundant and insufficient tool calls. How to calibrate erroneous behavioral patterns when executing TIR tasks, thereby exploring effective trajectories, remains an open-ended problem. In this paper, we propose ET-Agent, a training framework for calibrating agent's tool-use behavior through two synergistic perspectives: Self-evolving Data Flywheel and Behavior Calibration Training. Specifically, we introduce a self-evolutionary data flywheel to generate enhanced data, used to fine-tune LLM to improve its exploration ability. Based on this, we implement an two-phases behavior-calibration training framework. It is designed to progressively calibrate erroneous behavioral patterns to optimal behaviors. Further in-depth experiments confirm the superiority of \ourmodel{} across multiple dimensions, including correctness, efficiency, reasoning conciseness, and tool execution accuracy. Our ET-Agent framework provides practical insights for research in the TIR field. Codes can be found in https://github.com/asilverlight/ET-Agent

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.06860v2)
