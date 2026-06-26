---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Tree Search for LLM Agent Reinforcement Learning"
authors: Yuxiang Ji, Ziyu Ma, Yong Wang, Guanhua Chen et al.
url: https://arxiv.org/abs/2509.21240v3
date: 2025-09-25
citationCount: 43
influentialCitationCount: 7
velocity: 4.85
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agentic-ai, arxiv, 2025, cited]
---

# Tree Search for LLM Agent Reinforcement Learning

**arXiv [2509.21240v3](https://arxiv.org/abs/2509.21240v3)** · 2025-09-25 · **43 citations** (7 influential · 4.85/mo) · Yuxiang Ji, Ziyu Ma, Yong Wang, Guanhua Chen et al.

## Abstract
Recent advances in reinforcement learning (RL) have significantly enhanced the agentic capabilities of large language models (LLMs). In long-term and multi-turn agent tasks, existing approaches driven solely by outcome rewards often suffer from the problem of sparse supervision. To address the challenge, we propose Tree-based Group Relative Policy Optimization (Tree-GRPO), a grouped agent RL method based on tree search, where each tree node represents the complete agent interaction step. By sharing common prefixes, the tree search sampling increases the number of rollouts achievable within a fixed budget of tokens or tool calls. Moreover, we find that the tree-structured trajectory naturally allows the construction of step-wise process supervised signals even using only the outcome reward. Based on this, Tree-GRPO estimates the grouped relative advantages both on intra-tree and inter-tree levels. Through theoretical analysis, we demonstrate that the objective of intra-tree level group relative policy optimization is equivalent to that of step-level direct preference learning. Experiments across 11 datasets and 3 types of QA tasks demonstrate the superiority of the proposed tree-based RL over the chain-based RL method.

## From the paper (full-text excerpts)
**Method / approach.** method based on tree search, where each tree node represents the complete agent interaction step. By sharing common prefixes, the tree search sampling increases the number of rollouts achievable within a fixed budget of tokens or tool calls. Moreover, we find that the tree-structured trajectory naturally allows the construction of step-wise process supervised signals even using only the outcome reward. Based on this, Tree-GRPO estimates the grouped relative advantages both on intra-tree and inter-tree levels. Through theoretical analysis, we demonstrate that the objective of intra-tree level group relative policy optimization is equivalent to that of step-level direct preference learning. Experiments across 11 datasets and 3 types of QA tasks demonstrate the superiority of the proposed tree-based RL over the chain-based RL method. Higher Performance Less Rollout Budget 𝑨𝟏 Trajectory Signal 𝑨𝟐 𝑨𝟑 𝑨𝟏𝒕 + 𝑨𝟐𝒕 + 𝑨𝟑𝒕 Preference 𝑨𝟏 𝑨𝟐 𝑨𝒕𝟏 𝑨𝟑 𝑨𝒕𝟐 + 𝑨𝒕𝟑 Process Signal Preference 𝑨𝟏…

**Results.** Experiments across 11 datasets and 3 types of QA tasks demonstrate the superiority of the proposed tree-based RL over the chain-based RL method. Higher Performance Less Rollout Budget 𝑨𝟏 Trajectory Signal 𝑨𝟐 𝑨𝟑 𝑨𝟏𝒕 + 𝑨𝟐𝒕 + 𝑨𝟑𝒕 Preference 𝑨𝟏 𝑨𝟐 𝑨𝒕𝟏 𝑨𝟑 𝑨𝒕𝟐 + 𝑨𝒕𝟑 Process Signal Preference 𝑨𝟏 𝑨𝟐 𝑨𝟑 Chain-based Agent RL v.s. Tree-based Agent RL 𝑨𝟏𝒕 Process Signal 𝑨𝟐𝒕 𝑨𝒕𝟑 Figure 1: Comparison of chain-based and tree-based sampling strategies in LLM multi-turn agent RL. The tree structure brings two major advantages: (i) less rollout budget (both on tokens and toolcalls); (ii) higher performance. 1 I NTRODUCTION Reinforcement Learning (RL) has emerged as a pivotal post-training paradigm for Large Language Models (LLMs), catalyzing the development of several frontier models (DeepSeek-AI Team, 2025; Yang et al., 2025a; OpenAI, 2024). RL-tuned LLMs trained only with outcome rewards acquire complex reasoning abilities and achi…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2509.21240v3.md` · `raw/arxiv/2509.21240v3.fulltext.md`
