---
type: source
source_type: blog
title: "Build AI agents with the Mistral Agents API"
author: Mistral AI
outlet: Mistral AI news
url: https://mistral.ai/news/agents-api
resource: https://mistral.ai/news/agents-api
date: 2025-05-27
stake: Vendor release post — Mistral is launching and marketing its own paid Agents API; benchmark figures and "backbone of enterprise agentic platforms" framing are self-reported product marketing.
ingested: 2026-06-22
tags: [perspective, agentic-ai, tool-use, agent-protocols, mcp]
---

# Build AI agents with the Mistral Agents API

**Blog** · Mistral AI · 2025-05-27 · [link](https://mistral.ai/news/agents-api)

**The take (attributed):** Mistral pitches the Agents API as the production framework that turns its LLMs from text generators into "active problem-solvers" — the move from chat-completions to a stateful, tool-using, multi-agent runtime, with [[mcp|MCP]] as a first-class integration path.

**Stake:** This is a product launch. Treat the SimpleQA web-search lift and "enterprise-grade backbone" claims as Mistral marketing its own API, not radar fact.

## Argument
Mistral frames the Agents API as complementing its Chat Completion API with three things ordinary LLM calls lack: built-in connectors, persistent memory, and agentic orchestration.
- **Built-in connectors (tools deployed ready to call):** code execution (sandboxed Python), image generation (Black Forest Labs FLUX1.1 [pro] Ultra), document library (built-in RAG over Mistral Cloud docs), web search, and **MCP tools**. Per Mistral, web search lifts SimpleQA accuracy dramatically — Mistral Large 23%→75%, Mistral Medium 22%→82.3% (their numbers, their benchmark).
- **MCP as the open integration layer:** the SDK leverages [[mcp|Model Context Protocol]] tools for "real-world context" — APIs, databases, user data, documents. Demos (GitHub coding agent powered by Devstral, Linear-tickets assistant, financial analyst) all lean on multi-server MCP.
- **Stateful conversations:** persistent context, conversation branching (continue or fork from any point), streaming output — so developers stop hand-managing history.
- **Orchestration via handoffs:** agents added/removed dynamically; a finance agent can delegate to a web-search or calculator agent. A single request fans out across specialized agents — Mistral's framing of [[multi-agent-systems|multi-agent]] problem-solving.

## Why it matters / where it cuts
This is Mistral planting its flag on the same agent-platform turf as the [[mistral-agents-api|Mistral Agents API]] entity, OpenAI's Responses/Agents tooling and the [[mcp]]/[[tool-use]] stack — and notably betting on MCP as the open standard rather than a proprietary tool format, which is the signal worth tracking (a European frontier lab ratifying MCP). So what: if he's evaluating non-US agent runtimes, this is the one with a real handoff/orchestration model. Discount the benchmark theatre; the architecture (connectors + memory + handoffs) is the durable part.

## Graph
- **Author:** [[mistral]]
- **Concepts:** [[agentic-ai]] · [[tool-use]] · [[agent-protocols]] · [[multi-agent-systems]]
- **Entities:** [[mistral-agents-api]] · [[mcp]] · [[mistral]]
- **Raw:** `raw/blogs/2025-05-27-mistral-agents-api.md`
