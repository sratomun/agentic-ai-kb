---
type: source
source_type: arxiv
title: "ChipMATE: Multi-Agent Training via Reinforcement Learning for Enhanced RTL Generation"
authors: Zhongkai Yu, Yichen Lin, Chenyang Zhou, Yuwei Zhang et al.
url: https://arxiv.org/abs/2605.12857v1
date: 2026-05-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.MA
tags: [coding-agents, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# ChipMATE: Multi-Agent Training via Reinforcement Learning for Enhanced RTL Generation

**arXiv:** [2605.12857v1](https://arxiv.org/abs/2605.12857v1) · 2026-05-13 · cs.MA
**Authors:** Zhongkai Yu, Yichen Lin, Chenyang Zhou, Yuwei Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing API-based agentic systems for RTL code generation are fundamentally misaligned with industrial practice: they assume a golden testbench is available at generation time, rely on closed-source APIs incompatible with chip vendors' air-gapped security requirements, and cannot be trained on vendors' proprietary RTL codebases, leaving valuable internal data unused. Recent self-trained models address the deployment constraint but remain single-turn generators that overlook the critical role of verification in real industrial flows. To bridge these gaps, we present ChipMATE, the first self-trained multi-agent framework for RTL generation. Inspired by industrial practice where correctness emerges from cross-comparison between independently written RTL modules and reference models, ChipMATE pairs a Verilog agent with a Python reference-model agent that mutually verify each other's outputs without any golden oracle. We design a backtrack-based inference workflow to prevent error propagation across turns, and a two-stage training pipeline that first trains each agent individually to saturate its code-generation capability, then trains the team jointly to collaborate effectively. To support the training, we further build a hybrid data-generation framework that produces 64.4K high-quality reference model training samples. ChipMATE achieves 75.0\% and 80.1\% pass@1 on VerilogEval V2 with 4B and 9B base models, outperforming all existing self-trained models and even DeepSeek V4 with 1600B parameters. Our code and model weights are publicly available in https://github.com/zhongkaiyu/ChipMATE.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12857v1)
