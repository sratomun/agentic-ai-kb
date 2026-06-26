---
type: source
source_type: arxiv
title: "When Do Multi-Agent Systems Outperform? Analysing the Learning Efficiency of Agentic Systems"
authors: Junwei Su, Chuan Wu
url: https://arxiv.org/abs/2602.08272v1
date: 2026-02-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.LG
tags: [agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# When Do Multi-Agent Systems Outperform? Analysing the Learning Efficiency of Agentic Systems

**arXiv:** [2602.08272v1](https://arxiv.org/abs/2602.08272v1) · 2026-02-09 · cs.LG
**Authors:** Junwei Su, Chuan Wu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement Learning (RL) has emerged as a crucial method for training or fine-tuning large language models (LLMs), enabling adaptive, task-specific optimizations through interactive feedback. Multi-Agent Reinforcement Learning (MARL), in particular, offers a promising avenue by decomposing complex tasks into specialized subtasks learned by distinct interacting agents, potentially enhancing the ability and efficiency of LLM systems. However, theoretical insights regarding when and why MARL outperforms Single-Agent RL (SARL) remain limited, creating uncertainty in selecting the appropriate RL framework. In this paper, we address this critical gap by rigorously analyzing the comparative sample efficiency of MARL and SARL within the context of LLM. Leveraging the Probably Approximately Correct (PAC) framework, we formally define SARL and MARL setups for LLMs, derive explicit sample complexity bounds, and systematically characterize how task decomposition and alignment influence learning efficiency. Our results demonstrate that MARL improves sample complexity when tasks naturally decompose into independent subtasks, whereas dependent subtasks diminish MARL's comparative advantage. Additionally, we introduce and analyze the concept of task alignment, quantifying the trade-offs when enforcing independent task decomposition despite potential misalignments. These theoretical insights clarify empirical inconsistencies and provide practical criteria for deploying MARL strategies effectively in complex LLM scenarios.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.08272v1)
