---
type: source
source_type: blog
title: "Building effective agents"
author: Erik Schluntz, Barry Zhang (Anthropic)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/building-effective-agents
resource: https://www.anthropic.com/engineering/building-effective-agents
date: 2024-12-19
stake: Anthropic (sells Claude + Agent SDK) — but argues against over-engineering, an against-interest stance
ingested: 2026-06-22
tags: [perspective, multi-agent-systems, agentic-ai]
---

# Building effective agents

**Blog** · Erik Schluntz & Barry Zhang ([[anthropic|Anthropic]] Engineering) · 2024-12-19 · [link](https://www.anthropic.com/engineering/building-effective-agents)

**The take (attributed):** Anthropic argues the **most successful agent systems use simple, composable patterns, not frameworks** — and you should "find the simplest solution possible… this might mean not building agentic systems at all."

**Stake:** Anthropic sells Claude and an Agent SDK — yet the post is notably *anti*-complexity, recommending raw APIs over frameworks (against-interest).

## Argument
- Draws the now-canonical line: **workflows** (LLMs/tools on predefined code paths) vs **agents** (LLMs dynamically directing their own process). Both are "agentic systems."
- **Simplicity first:** often a single augmented LLM call suffices; agents trade latency/cost for performance — only worth it sometimes.
- Five workflow patterns (prompt chaining, routing, parallelization, orchestrator-workers, evaluator-optimizer); autonomous agents = "LLMs using tools in a loop on environmental feedback," with compounding-error risk → sandbox + guardrails.
- Three principles: **simplicity, transparency, well-crafted agent-computer interface (ACI)**; frameworks add abstraction that obscures prompts.

## Why it matters / where it cuts
The single most-cited practitioner doc on agent architecture, and the steel-manned **"don't over-build" / workflows-first** position — a direct counterweight to autonomous-agent maximalism. Anchors the debate below.

## Graph
- **Entities:** [[anthropic]] · [[mcp]]
- **Concepts:** [[multi-agent-systems]] · [[agentic-ai]] · [[tool-use]] · [[agent-reliability]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2024-12-19-anthropic-building-effective-agents.md`
