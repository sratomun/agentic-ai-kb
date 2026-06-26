---
type: source
source_type: arxiv
title: "Learning When Not to Act: Mitigating Tool Abuse in Agentic Reinforcement Learning"
authors: Liuji Chen, Dianxing Tang, Xing Shi, Dingshuo Chen et al.
url: https://arxiv.org/abs/2606.02132v2
date: 2026-06-01
ingested: 2026-06-21
depth: full-text
tags: [agentic-rl, tool-use, arxiv]
---

# Learning When Not to Act: Mitigating Tool Abuse in Agentic Reinforcement Learning

**Why it matters:** Names 'tool abuse' — agents overusing tools on queries solvable by reasoning — and fixes it with difficulty-aware reward shaping instead of blunt penalties. Cost + latency relevance is obvious.

## Takeaways
- [[eapo|EAPO]] injects tool-free trajectories per rollout group, penalizes redundant calls mainly on easy queries, and reweights tokens by confidence.
- vs GRPO: +10.45%/+7.27%/+9.69% average across nine benchmarks while cutting tool calls 18–25% on Qwen2.5-3B/7B and Llama3.1-8B.
- Agents can learn when NOT to use tools without losing tool-integrated reasoning.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[eapo]] · [[grpo]]
- **Raw:** `raw/arxiv/2606.02132v2.md` · `raw/arxiv/2606.02132v2.fulltext.md`
