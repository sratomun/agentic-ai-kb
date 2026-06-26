---
type: source
source_type: arxiv
title: "RecThinker: An Agentic Framework for Tool-Augmented Reasoning in Recommendation"
authors: Haobo Zhang, Yutao Zhu, Kelong Mao, Tianhao Li et al.
url: https://arxiv.org/abs/2603.09843v1
date: 2026-03-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 26
primary: cs.IR
tags: [recommendation-agents, agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# RecThinker: An Agentic Framework for Tool-Augmented Reasoning in Recommendation

**arXiv:** [2603.09843v1](https://arxiv.org/abs/2603.09843v1) · 2026-03-10 · cs.IR
**Authors:** Haobo Zhang, Yutao Zhu, Kelong Mao, Tianhao Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have revolutionized recommendation agents by providing superior reasoning and flexible decision-making capabilities. However, existing methods mainly follow a passive information acquisition paradigm, where agents either rely on static pre-defined workflows or perform reasoning with constrained information. It limits the agent's ability to identify information sufficiency, often leading to suboptimal recommendations when faced with fragmented user profiles or sparse item metadata. To address these limitations, we propose RecThinker, an agentic framework for tool-augmented reasoning in recommendation, which shifts recommendation from passive processing to autonomous investigation by dynamically planning reasoning paths and proactively acquiring essential information via autonomous tool-use. Specifically, RecThinker adopts an Analyze-Plan-Act paradigm, which first analyzes the sufficiency of user-item information and autonomously invokes tool-calling sequences to bridge information gaps between available knowledge and reasoning requirements. We develop a suite of specialized tools for RecThinker, enabling the model to acquire user-side, item-side, and collaborative information for better reasoning and user-item matching. Furthermore, we introduce a self-augmented training pipeline, comprising a Supervised Fine-Tuning (SFT) stage to internalize high-quality reasoning trajectories and a Reinforcement Learning (RL) stage to optimize for decision accuracy and tool-use efficiency. Extensive experiments on multiple benchmark datasets demonstrate that RecThinker consistently outperforms strong baselines in the recommendation scenario.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.09843v1)
