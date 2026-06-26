---
type: source
source_type: arxiv
title: "When the Manual Lies: A Realistic Benchmark to Evaluate MCP Poisoning Attacks for LLM Agents"
authors: Shi Liu, Xuehai Tang, Xikang Yang, Liang Lin et al.
url: https://arxiv.org/abs/2605.24069v1
date: 2026-05-22
ingested: 2026-06-21
depth: full-text
tags: [agent-security, agent-protocols, arxiv]
---

# When the Manual Lies: A Realistic Benchmark to Evaluate MCP Poisoning Attacks for LLM Agents

**Why it matters:** Benchmarks [[tool-description-poisoning|Tool Description Poisoning]] — malicious instructions hidden in tool metadata, not code. GPT-4o hits ~100% attack success in six categories; common prompt guardrails are useless or worse ('Firewall Fallacy').

## Takeaways
- Tool Description Poisoning (TDP): inject malicious instructions into a tool's descriptive metadata (the 'manual' the agent plans against), not its executable code.
- MCP-TDP benchmark: 32 real-world cases across 6 risk categories; leading models (e.g. GPT-4o) show ~100% attack success in six high-risk scenarios.
- Prompt guardrails largely ineffective and sometimes counterproductive ('Firewall Fallacy'); proposes Reactive Self-Correction (agent detects and reverts its own malicious actions post-execution).

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]] · [[mcp-tdp-bench]] · [[tool-description-poisoning]]
- **Raw:** `raw/arxiv/2605.24069v1.md` · `raw/arxiv/2605.24069v1.fulltext.md`
