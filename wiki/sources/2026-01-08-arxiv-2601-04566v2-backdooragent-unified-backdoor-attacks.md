---
type: source
source_type: arxiv
title: "BackdoorAgent: A Unified Framework for Backdoor Attacks on LLM-based Agents"
authors: Yunhao Feng, Yige Li, Yutao Wu, Yingshui Tan et al.
url: https://arxiv.org/abs/2601.04566v2
date: 2026-01-08
ingested: 2026-06-21
depth: full-text
tags: [agent-security, agent-memory, arxiv]
---

# BackdoorAgent: A Unified Framework for Backdoor Attacks on LLM-based Agents

**Why it matters:** First agent-centric, stage-aware view of backdoor threats — triggers planted at one stage persist and propagate across planning/memory/tool stages. High persistence rates make this a real supply-chain concern.

## Takeaways
- BackdoorAgent structures the attack surface into planning, memory, and tool-use stages and instruments execution to trace trigger activation/propagation.
- Standardized benchmark across Agent QA/Code/Web/Drive (language-only + multimodal).
- GPT-based backbone: trigger persistence 43.6% (planning), 78.0% (memory), 60.3% (tool-stage) — single-stage triggers persist across many steps.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Raw:** `raw/arxiv/2601.04566v2.md` · `raw/arxiv/2601.04566v2.fulltext.md`
