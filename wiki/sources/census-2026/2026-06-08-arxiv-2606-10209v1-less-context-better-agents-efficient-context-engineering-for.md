---
type: source
source_type: arxiv
title: "Less Context, Better Agents: Efficient Context Engineering for Long-Horizon Tool-Using LLM Agents"
authors: Abhilasha Lodha, Mahsa Pahlavikhah Varnosfaderani, Abir Chakraborty, Abhinav Mithal
url: https://arxiv.org/abs/2606.10209v1
date: 2026-06-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [finance-agents, agent-reliability, agent-protocols, agent-memory, tool-use, arxiv, auto-ingested]
---

# Less Context, Better Agents: Efficient Context Engineering for Long-Horizon Tool-Using LLM Agents

**arXiv:** [2606.10209v1](https://arxiv.org/abs/2606.10209v1) · 2026-06-08 · cs.AI
**Authors:** Abhilasha Lodha, Mahsa Pahlavikhah Varnosfaderani, Abir Chakraborty, Abhinav Mithal

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models deployed as autonomous agents for enterprise workflows face a key challenge: verbose tool responses from enterprise systems can cause context overflow, stale-state errors, and high inference cost. We study this problem in automated expense itemization in Microsoft Dynamics 365 Finance and Operations using Model Context Protocol tools. We evaluate four GPT-5 configurations on a 50-task hotel expense benchmark: no user model, full conversation history, context pruned to the last 5 tool call/response pairs, and pruning with automated summarization. Results are averaged across 5 independent runs, with the user model held constant for the context-engineering comparison. The no-user-model baseline achieves only 8.0% complete itemization. Full-context retention improves completion to 71.0%, but consumes 1,480,996 tokens and 14.56 hours per benchmark. Pruning to the last 5 tool calls improves completion to 79.0% while reducing token use to 535,274 and runtime to 5.39 hours. Adding summarization achieves the best result: 91.6% complete itemization and 99.64% average amount itemized, with 553,374 tokens and 5.79 hours. We further report confidence intervals, effect-size analysis, sensitivity over pruning and summary windows, failure analysis, results across five expense types grouped into three categories, and cross-model evidence with Claude Sonnet 4.5. These results show that, for this class of enterprise tool-use workflow, selective retention of recent tool interactions plus compact summarization can improve both reliability and efficiency compared with full-history retention.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]] · [[claude]] · [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.10209v1)
