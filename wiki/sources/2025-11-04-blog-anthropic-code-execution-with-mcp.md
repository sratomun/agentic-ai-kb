---
type: source
source_type: blog
title: "Code execution with MCP: building more efficient agents"
author: Adam Jones, Conor Kelly (Anthropic)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/code-execution-with-mcp
resource: https://www.anthropic.com/engineering/code-execution-with-mcp
date: 2025-11-04
stake: Anthropic (originated MCP; sells Claude + the Agent SDK) — extends its own protocol's efficiency story
ingested: 2026-06-22
tags: [perspective, mcp, tool-use, agentic-ai]
---

# Code execution with MCP: building more efficient agents

**Blog** · Adam Jones & Conor Kelly ([[anthropic|Anthropic]] Engineering) · 2025-11-04 · [link](https://www.anthropic.com/engineering/code-execution-with-mcp)

**The take (attributed):** Anthropic argues that once an agent has hundreds–thousands of MCP tools, loading every tool definition up front and routing every intermediate result through the model wastes context — so agents should **write code that calls MCP tools** (presented as a filesystem of code APIs) instead of calling them directly. They report cutting a workflow from **150,000 → 2,000 tokens (98.7%)**.

**Stake:** Anthropic *originated* MCP (Nov 2024) and sells the model + Agent SDK — this both fixes a scaling pain in its own protocol and deepens lock-in to MCP. (Notably cites Cloudflare's independent "Code Mode" as corroboration.)

## Argument
- **Two token sinks at scale:** (1) all tool definitions loaded upfront overload context; (2) intermediate results flow through the model twice (e.g., a transcript copied from Google Drive to Salesforce → ~50K extra tokens for a 2-hour meeting).
- **Fix — tools as code on a filesystem:** generate `servers/<server>/<tool>.ts` files; the agent lists `./servers/` and reads only the tool files it needs (**progressive disclosure**), or uses a `search_tools` tool with a detail-level parameter.
- **Benefits:** filter/transform large results *in the execution environment* (see 5 of 10,000 rows, not all); familiar control flow (loops/conditionals) instead of chained tool calls, also cutting time-to-first-token; **privacy** — intermediate data stays in the sandbox, and the harness can tokenize PII so real values flow tool→tool but never through the model; **state persistence + Skills** — agents write reusable functions and SKILL.md files, evolving their own scaffolding.
- **Caveat:** running agent-generated code needs a secure sandbox, resource limits, monitoring — weigh against the savings.

## Why it matters / where it cuts
The clearest statement of the **"code mode"** pattern now spreading across the agent ecosystem — a structural answer to MCP's tool-bloat problem and a bridge between [[tool-use]], [[mcp]], and [[agent-skills]]. For an exec evaluating agent infra, it reframes "how many tools can I connect?" as a context-budget question with a known software-engineering fix. Pairs with [[2025-09-11-blog-anthropic-writing-tools-for-agents]] and [[2025-09-29-blog-anthropic-effective-context-engineering]].

## Graph
- **Author:** [[anthropic|Anthropic]] (MCP team)
- **Entities:** [[anthropic]] · [[mcp]]
- **Concepts:** [[mcp|Model Context Protocol]] · [[tool-use]] · [[agentic-ai]] · [[agent-skills]] · [[harness-engineering]] · [[agent-security]]
- **Raw:** `raw/blogs/2025-11-04-anthropic-code-execution-with-mcp.md`
