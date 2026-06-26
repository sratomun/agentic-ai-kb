---
type: source
source_type: blog
title: "Connect the dots: Build with built-in and custom MCPs in Studio"
author: Mistral AI
outlet: Mistral AI news
url: https://mistral.ai/news/connectors
resource: https://mistral.ai/news/connectors
date: 2026-05-22
stake: Vendor release post — Mistral is shipping a paid platform feature (Connectors in Studio) and marketing its MCP governance story; "human-in-the-loop", "governed & monitored" framing is product positioning.
ingested: 2026-06-22
tags: [perspective, mcp, tool-use, agentic-ai, agent-security]
---

# Connect the dots: Build with built-in and custom MCPs in Studio

**Blog** · Mistral AI · 2026-05-22 · [link](https://mistral.ai/news/connectors)

**The take (attributed):** Mistral argues the hard part of enterprise agents isn't the model, it's the integration layer — so it's moving [[mcp|MCP]] connectors *into the platform* (registered, reusable, governed) rather than re-implemented in app code, and adding human-in-the-loop approval as a first-class control.

**Stake:** Product launch (Public Preview). The "set up once, run everywhere," observability and governance claims are Mistral selling Studio.

## Argument
A year after the [[2025-05-27-blog-mistral-agents-api|Agents API]], Mistral generalizes MCP into **Connectors** available via API/SDK across all model and agent calls:
- **Connectors = MCP integrations packaged as reusable entities.** Register a custom MCP server (or OAuth-backed connector like Salesforce) once; it becomes discoverable, governed and monitored in Studio and a native tool for any conversation, agent or workflow — no re-implementing auth, no duplicating integration code across teams. Mistral's stated pain point: teams rebuild the same integration layer repeatedly, causing "security risks, lack of traffic observability, and duplication."
- **Direct tool calling** — call a connector's tool deterministically (`call_tool_async`) without the model deciding when/how, for debugging and pipeline-style automation.
- **Human-in-the-loop** — `requires_confirmation` pauses execution and hands control back to the application before a tool runs. "The model proposes, the user application decides." `tool_configuration` can include/exclude specific tools (e.g. exclude `delete_file`).
- Golden-path demo: an open-source-software-auditor agent wiring built-in GitHub + web search + a custom DeepWiki MCP server.

## Why it matters / where it cuts
This is the maturing of the [[mcp]] story from "we support the protocol" (2025 Agents API) to "we govern it as enterprise infra" — registration, observability, scoped tool permissions, and explicit approval gates. That governance framing is exactly the seam the [[agent-security]] research flags: MCP makes mixing tools trivial, which is also how the lethal-trifecta / tool-poisoning risks enter. Mistral selling *governed* MCP is a tacit acknowledgement of that. So what: the include/exclude + requires_confirmation pattern is the concrete control surface to ask any agent-platform vendor about.

## Graph
- **Author:** [[mistral]]
- **Concepts:** [[mcp|MCP]] · [[tool-use]] · [[agentic-ai]] · [[agent-security]]
- **Entities:** [[mcp]] · [[mistral-agents-api]] · [[mistral]]
- **Raw:** `raw/blogs/2026-05-22-mistral-connectors-mcp-studio.md`
