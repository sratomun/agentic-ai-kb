---
type: source
source_type: arxiv
title: "DLLM-Searcher: Adapting Diffusion Large Language Model for Search Agents"
authors: Jiahao Zhao, Shaoxuan Xu, Zhongxiang Sun, Fengqi Zhu et al.
url: https://arxiv.org/abs/2602.07035v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [tool-use, arxiv, auto-ingested]
---

# DLLM-Searcher: Adapting Diffusion Large Language Model for Search Agents

**arXiv:** [2602.07035v1](https://arxiv.org/abs/2602.07035v1) · 2026-02-03 · cs.AI
**Authors:** Jiahao Zhao, Shaoxuan Xu, Zhongxiang Sun, Fengqi Zhu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recently, Diffusion Large Language Models (dLLMs) have demonstrated unique efficiency advantages, enabled by their inherently parallel decoding mechanism and flexible generation paradigm. Meanwhile, despite the rapid advancement of Search Agents, their practical deployment is constrained by a fundamental limitation, termed as 1) Latency Challenge: the serial execution of multi-round reasoning, tool calling, and tool response waiting under the ReAct agent paradigm induces severe end-to-end latency. Intuitively, dLLMs can leverage their distinctive strengths to optimize the operational efficiency of agents under the ReAct agent paradigm. Practically, existing dLLM backbones face the 2) Agent Ability Challenge. That is, existing dLLMs exhibit remarkably weak reasoning and tool-calling capabilities, preventing these advantages from being effectively realized in practice. In this paper, we propose DLLM-Searcher, an optimization framework for dLLM-based Search Agents. To solve the Agent Ability Challenge, we design a two-stage post-training pipeline encompassing Agentic Supervised Fine-Tuning (Agentic SFT) and Agentic Variance-Reduced Preference Optimization Agentic VRPO, which enhances the backbone dLLM's information seeking and reasoning capabilities. To mitigate the Latency Challenge, we leverage the flexible generation mechanism of dLLMs and propose a novel agent paradigm termed Parallel-Reasoning and Acting P-ReAct. P-ReAct guides the model to prioritize decoding tool_call instructions, thereby allowing the model to keep thinking while waiting for the tool's return. Experimental results demonstrate that DLLM-Searcher achieves performance comparable to mainstream LLM-based search agents and P-ReAct delivers approximately 15% inference acceleration. Our code is available at https://anonymous.4open.science/r/DLLM-Searcher-553C

## Graph
- **Concepts:** [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07035v1)
