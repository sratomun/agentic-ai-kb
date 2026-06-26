---
type: source
source_type: arxiv
title: "SQL-Trail: Multi-Turn Reinforcement Learning with Interleaved Feedback for Text-to-SQL"
authors: Harper Hua, Zhen Han, Zhengyuan Shen, Jeremy Lee et al.
url: https://arxiv.org/abs/2601.17699v1
date: 2026-01-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [data-query-agents, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# SQL-Trail: Multi-Turn Reinforcement Learning with Interleaved Feedback for Text-to-SQL

**arXiv:** [2601.17699v1](https://arxiv.org/abs/2601.17699v1) · 2026-01-25 · cs.AI
**Authors:** Harper Hua, Zhen Han, Zhengyuan Shen, Jeremy Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While large language models (LLMs) have substantially improved Text-to-SQL generation, a pronounced gap remains between AI systems and human experts on challenging benchmarks such as BIRD-SQL. We argue this gap stems largely from the prevailing single-pass paradigm, which lacks the iterative reasoning, schema exploration, and error-correction behaviors that humans naturally employ. To address this limitation, we introduce SQL-Trail, a multi-turn reinforcement learning (RL) agentic framework for Text-to-SQL. Rather than producing a query in one shot, SQL-Trail interacts with the database environment and uses execution feedback to iteratively refine its predictions. Our approach centers on two key ideas: (i) an adaptive turn-budget allocation mechanism that scales the agent's interaction depth to match question difficulty, and (ii) a composite reward panel that jointly incentivizes SQL correctness and efficient exploration. Across benchmarks, SQL-Trail sets a new state of the art and delivers strong data efficiency--up to 18x higher than prior single-pass RL state-of-the-art methods. Notably, our 7B and 14B models outperform substantially larger proprietary systems by 5% on average, underscoring the effectiveness of interactive, agentic workflows for robust Text-to-SQL generation.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17699v1)
