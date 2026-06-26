---
type: source
source_type: arxiv
title: "Can We Trust a Black-box LLM? LLM Untrustworthy Boundary Detection via Bias-Diffusion and Multi-Agent Reinforcement Learning"
authors: Xiaotian Zhou, Di Tang, Xiaofeng Wang, Xiaozhong Liu
url: https://arxiv.org/abs/2604.05483v1
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Can We Trust a Black-box LLM? LLM Untrustworthy Boundary Detection via Bias-Diffusion and Multi-Agent Reinforcement Learning

**arXiv:** [2604.05483v1](https://arxiv.org/abs/2604.05483v1) · 2026-04-07 · cs.AI
**Authors:** Xiaotian Zhou, Di Tang, Xiaofeng Wang, Xiaozhong Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have shown a high capability in answering questions on a diverse range of topics. However, these models sometimes produce biased, ideologized or incorrect responses, limiting their applications if there is no clear understanding of which topics their answers can be trusted. In this research, we introduce a novel algorithm, named as GMRL-BD, designed to identify the untrustworthy boundaries (in terms of topics) of a given LLM, with black-box access to the LLM and under specific query constraints. Based on a general Knowledge Graph (KG) derived from Wikipedia, our algorithm incorporates with multiple reinforcement learning agents to efficiently identify topics (some nodes in KG) where the LLM is likely to generate biased answers. Our experiments demonstrated the efficiency of our algorithm, which can detect the untrustworthy boundary with just limited queries to the LLM. Additionally, we have released a new dataset containing popular LLMs including Llama2, Vicuna, Falcon, Qwen2, Gemma2 and Yi-1.5, along with labels indicating the topics on which each LLM is likely to be biased.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]] · [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05483v1)
