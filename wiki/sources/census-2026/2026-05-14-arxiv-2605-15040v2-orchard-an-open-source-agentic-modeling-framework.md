---
type: source
source_type: arxiv
title: "Orchard: An Open-Source Agentic Modeling Framework"
authors: Baolin Peng, Wenlin Yao, Qianhui Wu, Hao Cheng et al.
url: https://arxiv.org/abs/2605.15040v2
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 25
primary: cs.AI
tags: [coding-agents, computer-use-agents, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Orchard: An Open-Source Agentic Modeling Framework

**arXiv:** [2605.15040v2](https://arxiv.org/abs/2605.15040v2) · 2026-05-14 · cs.AI
**Authors:** Baolin Peng, Wenlin Yao, Qianhui Wu, Hao Cheng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic modeling aims to transform LLMs into autonomous agents capable of solving complex tasks through planning, reasoning, tool use, and multi-turn interaction with environments. Despite major investment, open research remains constrained by infrastructure and training gaps. Many high-performing systems rely on proprietary codebases, models, or services, while most open-source frameworks focus on orchestration and evaluation rather than scalable agent training. We present Orchard, an open-source framework for scalable agentic modeling. At its core is Orchard Env, a lightweight environment service providing reusable primitives for sandbox lifecycle management across task domains, agent harnesses, and pipeline stages. On top of Orchard Env, we build three agentic modeling recipes. Orchard-SWE targets coding agents. We distill 107K trajectories from MiniMax-M2.5 and Qwen3.5-397B, introduce credit-assignment SFT to learn from productive segments of unresolved trajectories, and apply Balanced Adaptive Rollout for RL. Starting from Qwen3-30B-A3B-Thinking, Orchard-SWE achieves 64.3% on SWE-bench Verified after SFT and 67.5% after SFT+RL, setting a new state of the art among open-source models of comparable size. Orchard-GUI trains a 4B vision-language computer-use agent using only 0.4K distilled trajectories and 2.2K open-ended tasks. It achieves 74.1%, 67.0%, and 64.0% success rates on WebVoyager, Online-Mind2Web, and DeepShop, respectively, making it the strongest open-source model while remaining competitive with proprietary systems. Orchard-Claw targets personal assistant agents. Trained with only 0.2K synthetic tasks, it achieves 59.6% pass@3 on Claw-Eval and 73.9% when paired with a stronger ZeroClaw harness. Collectively, these results show that a lightweight, open, harness-agnostic environment layer enables reusable agentic data, training recipes, and evaluations across domains.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]] · [[swe-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15040v2)
