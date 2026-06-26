---
type: source
source_type: arxiv
title: "The Confidence Dichotomy: Analyzing and Mitigating Miscalibration in Tool-Use Agents"
authors: Weihao Xuan, Qingcheng Zeng, Heli Qi, Yunze Xiao et al.
url: https://arxiv.org/abs/2601.07264v1
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agent-reliability, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# The Confidence Dichotomy: Analyzing and Mitigating Miscalibration in Tool-Use Agents

**arXiv:** [2601.07264v1](https://arxiv.org/abs/2601.07264v1) · 2026-01-12 · cs.CL
**Authors:** Weihao Xuan, Qingcheng Zeng, Heli Qi, Yunze Xiao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous agents based on large language models (LLMs) are rapidly evolving to handle multi-turn tasks, but ensuring their trustworthiness remains a critical challenge. A fundamental pillar of this trustworthiness is calibration, which refers to an agent's ability to express confidence that reliably reflects its actual performance. While calibration is well-established for static models, its dynamics in tool-integrated agentic workflows remain underexplored. In this work, we systematically investigate verbalized calibration in tool-use agents, revealing a fundamental confidence dichotomy driven by tool type. Specifically, our pilot study identifies that evidence tools (e.g., web search) systematically induce severe overconfidence due to inherent noise in retrieved information, while verification tools (e.g., code interpreters) can ground reasoning through deterministic feedback and mitigate miscalibration. To robustly improve calibration across tool types, we propose a reinforcement learning (RL) fine-tuning framework that jointly optimizes task accuracy and calibration, supported by a holistic benchmark of reward designs. We demonstrate that our trained agents not only achieve superior calibration but also exhibit robust generalization from local training environments to noisy web settings and to distinct domains such as mathematical reasoning. Our results highlight the necessity of domain-specific calibration strategies for tool-use agents. More broadly, this work establishes a foundation for building self-aware agents that can reliably communicate uncertainty in high-stakes, real-world deployments.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.07264v1)
