---
type: source
source_type: arxiv
title: "Beyond Max Tokens: Stealthy Resource Amplification via Tool Calling Chains in LLM Agents"
authors: Kaiyu Zhou, Yongsen Zheng, Yicheng He, Meng Xue et al.
url: https://arxiv.org/abs/2601.10955v2
date: 2026-01-16
ingested: 2026-06-21
depth: full-text
tags: [agent-security, tool-use, arxiv]
---

# Beyond Max Tokens: Stealthy Resource Amplification via Tool Calling Chains in LLM Agents

**Why it matters:** A new economic-DoS attack class living at the tool layer under [[mcp]] — text-only edits to tool metadata steer agents into runaway tool-calling chains, raising per-query cost up to 658×. Prompt filters miss it.

## Takeaways
- Multi-turn economic DoS at the tool layer: edit text-visible fields + template return policy to push agents into verbose tool-calling chains while preserving signatures and the benign terminal payload.
- MCTS-optimized text-only edits maximize cost under a task-success constraint.
- Across 6 LLMs on ToolBench/BFCL: >60k-token trajectories, up to 658× per-query cost, 100–560× energy, 35–74% KV-cache occupancy — prompt filters and output monitors rarely detect it.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]] · [[bfcl]]
- **Raw:** `raw/arxiv/2601.10955v2.md` · `raw/arxiv/2601.10955v2.fulltext.md`
