---
type: source
source_type: arxiv
title: "Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading for Eliminating the MCP/Tools Tax in Scalable Agentic Workflows"
authors: Anuj Sadani, Deepak Kumar
url: https://arxiv.org/abs/2604.21816v1
date: 2026-04-23
ingested: 2026-06-21
depth: full-text
tags: [tool-use, agent-protocols, arxiv]
---

# Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Loading for Eliminating the MCP/Tools Tax in Scalable Agentic Workflows

**Why it matters:** Quantifies the 'MCP tax' — eager schema injection costs ~10k–60k tokens per turn — and proposes gated, lazy tool loading. The thesis (protocol efficiency, not context length, is the binding constraint) is a sharp exec talking point.

## Takeaways
- Names the Tools/MCP Tax: stateless eager schema injection adds ~10k–60k tokens/turn, inflating KV cache and degrading reasoning near ~70% context utilization.
- Tool Attention = intent-schema-overlap scoring + state-aware gating + two-phase lazy schema loader (summaries in context, full schemas promoted only for top-k tools).
- Simulated 120-tool/6-server benchmark: per-turn tool tokens cut 95% (47.3k→2.4k); end-to-end gains are projections, not live-agent measurements (authors flag this).

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2604.21816v1.md` · `raw/arxiv/2604.21816v1.fulltext.md`
