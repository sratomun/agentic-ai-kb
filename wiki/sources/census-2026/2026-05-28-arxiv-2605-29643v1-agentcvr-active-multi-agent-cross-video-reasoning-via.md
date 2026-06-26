---
type: source
source_type: arxiv
title: "AgentCVR: Active Multi-Agent Cross-Video Reasoning via Script-Simulated Reinforcement Learning"
authors: Yilun Qiu, Jiahe Wang, Cilin Yan, Jiayin Cai et al.
url: https://arxiv.org/abs/2605.29643v1
date: 2026-05-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CV
tags: [agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AgentCVR: Active Multi-Agent Cross-Video Reasoning via Script-Simulated Reinforcement Learning

**arXiv:** [2605.29643v1](https://arxiv.org/abs/2605.29643v1) · 2026-05-28 · cs.CV
**Authors:** Yilun Qiu, Jiahe Wang, Cilin Yan, Jiayin Cai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cross-Video Reasoning (CVR) has emerged as a critical frontier in multimodal intelligence, requiring models to retrieve, align, and aggregate evidence distributed across multiple videos. Current Multimodal Large Language Models (MLLMs) often struggle with CVR, as simple single-pass strategies encode multiple videos into a shared compressed context, potentially obscuring rare but critical evidence. In this paper, we propose AgentCVR, a multi-agent framework that treats CVR as an active evidence-acquisition task. AgentCVR employs a Master Agent to iteratively coordinate specialized Visual and Audio Agents for targeted evidence extraction. To ensure efficient training, we introduce Script-Simulated RL, which optimizes the agent's policy with LLM-generated semantic scripts and a lightweight text-based simulator, bypassing costly multimodal inference during online exploration. Experimental results on a comprehensive CVR benchmark show that AgentCVR outperforms single-pass baselines and achieves comparable performance to state-of-the-art closed-source systems, particularly in complex cross-video alignment and localization. To ensure reproducibility, our code is available at https://github.com/wang-jh24/AgentCVR.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.29643v1)
