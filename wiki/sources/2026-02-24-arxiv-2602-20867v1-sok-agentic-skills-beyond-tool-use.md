---
type: source
source_type: arxiv
title: "SoK: Agentic Skills -- Beyond Tool Use in LLM Agents"
authors: Yanna Jiang, Delong Li, Haiyu Deng, Baihe Ma et al.
url: https://arxiv.org/abs/2602.20867v1
date: 2026-02-24
ingested: 2026-06-21
depth: full-text
tags: [agent-skills, agent-security, tool-use, arxiv]
---

# SoK: Agentic Skills -- Beyond Tool Use in LLM Agents

**Why it matters:** Formalizes the 'skill' layer that sits above tool calls — the abstraction Anthropic's SKILL.md popularized — and documents a real supply-chain attack (ClawHavoc) where ~1,200 malicious skills hit a marketplace.

## Takeaways
- Maps the skill lifecycle (discovery→practice→distillation→storage→composition→evaluation→update) and gives seven design patterns plus a representation×scope taxonomy.
- Security core: supply-chain risk, prompt injection via skill payloads, trust-tiered execution — grounded in the ClawHavoc campaign (~1,200 malicious skills exfiltrating API keys, crypto wallets, credentials).
- Benchmark evidence: curated skills lift success rates, but self-generated skills can degrade them.

## Graph
- **Concepts:** [[agent-skills|Agent skills]] · [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Raw:** `raw/arxiv/2602.20867v1.md` · `raw/arxiv/2602.20867v1.fulltext.md`
