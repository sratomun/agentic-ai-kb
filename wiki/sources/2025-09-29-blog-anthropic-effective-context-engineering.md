---
type: source
source_type: blog
title: "Effective context engineering for AI agents"
author: Anthropic Applied AI team (Prithvi Rajasekaran, Ethan Dixon, Carly Ryan, Jeremy Hadfield)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
resource: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
date: 2025-09-29
stake: Anthropic (sells Claude + the Agent SDK) — frames context engineering around its own products (Claude Code, memory tool, Sonnet 4.5)
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-memory, harness-engineering]
---

# Effective context engineering for AI agents

**Blog** · Anthropic Applied AI team ([[anthropic|Anthropic]] Engineering) · 2025-09-29 · [link](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)

**The take (attributed):** Anthropic argues that **"context engineering" is the natural successor to prompt engineering** — for multi-turn agents the job is curating the *whole* context state (system prompt, tools, history, external data), and the guiding rule is to find the **smallest set of high-signal tokens** that yields the desired behavior, because attention is a finite, degrading budget ("context rot").

**Stake:** Anthropic sells Claude and the Agent SDK; every technique is illustrated with its own products (Claude Code's just-in-time retrieval, the Sonnet 4.5 memory tool, tool-result clearing on the Developer Platform).

## Argument
- **Context rot:** as tokens grow, recall degrades — a performance gradient, not a cliff. Transformers' n² pairwise attention plus training-distribution bias toward shorter sequences make context a finite "attention budget."
- **Anatomy of good context:** system prompts at the *right altitude* (between brittle hardcoded if-else and vague guidance); tools that are token-efficient and non-overlapping (bloated tool sets are a top failure mode — "if a human can't say which tool to use, an agent can't either"); few-shot examples that are *canonical*, not an edge-case laundry list.
- **Adopts the simple definition:** "agents = LLMs autonomously using tools in a loop" (crediting Simon Willison).
- **Just-in-time retrieval:** rather than pre-embedding everything, keep lightweight identifiers (file paths, queries, links) and load data at runtime — enabling **progressive disclosure**. Claude Code uses a *hybrid* (CLAUDE.md up front; glob/grep just-in-time).
- **Long-horizon techniques:** (1) **compaction** — summarize a near-full window and reinitiate (tool-result clearing is the safest light touch); (2) **structured note-taking / agentic memory** — persist notes outside context (Claude playing Pokémon; the Sonnet 4.5 memory tool); (3) **sub-agent architectures** — subagents burn tens of thousands of tokens but return ~1–2K-token summaries.
- Recurring counsel: "do the simplest thing that works"; smarter models need less prescriptive engineering.

## Why it matters / where it cuts
This is the post that **named and codified "context engineering"** as the dominant agent-building discipline — the through-line connecting Anthropic's tool-use, memory, and multi-agent posts. For an exec, it reframes reliability work: the bottleneck isn't the prompt, it's curating a finite attention budget. Feeds [[harness-engineering]], [[agent-memory]], and [[multi-agent-systems]].

## Graph
- **Author:** [[anthropic|Anthropic]] Applied AI
- **Entities:** [[anthropic]] · [[mcp]] · [[claude]] · [[simon-willison]]
- **Concepts:** [[agentic-ai]] · [[harness-engineering]] · [[agent-memory]] · [[tool-use]] · [[multi-agent-systems]]
- **Raw:** `raw/blogs/2025-09-29-anthropic-effective-context-engineering.md`
