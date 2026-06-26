---
type: source
source_type: blog
title: "Why MCP Won"
author: swyx (Shawn Wang)
outlet: Latent.Space
url: https://www.latent.space/p/why-mcp-won
resource: https://www.latent.space/p/why-mcp-won
date: 2025-03-10
stake: Founder/CEO of AI Engineer + Latent Space — his AIE Summit hosted the viral MCP workshop he credits with the protocol's tipping point, so he has reputational skin in MCP's narrative.
ingested: 2026-06-22
tags: [perspective, agent-protocols, tool-use]
---

# Why MCP Won

**Blog** · swyx (Shawn Wang) · 2025-03-10 · [link](https://www.latent.space/p/why-mcp-won)

**The take (attributed):** swyx argues [[mcp|MCP]] is *already* the de facto winner of the "agent open standard wars" — not on technical merit but on **adoption mechanics**: an AI-native standard from a trusted big backer, modeled on a proven protocol (LSP), that reified patterns agents were already converging on.

**Stake:** His AI Engineer Summit hosted the MCP workshop that went viral (~300k views); he admits "we merely poured fuel on a fire," but he benefits from being seen as the venue that called it.

## Argument
Six reasons, in rough descending order:
1. **"AI-Native" version of an old idea.** Technically MCP overlaps OpenAPI/GraphQL/SOAP, but dismissing it on technical grounds "neglects the sociological context." MCP was "born from lessons in Claude Sonnet's #1 SWE-Bench result and Building Effective Agents," and puts "dynamic context access at the center of its universe" — the Tools (model-controlled) / Resources (app-controlled) / Prompts (user-controlled) split. → wins over OpenAPI *and* [[langgraph|LangChain]].
2. **An open standard with a big backer.** "If the standard backer seems too big to really care about locking you in... I will adopt it." Plus a genuinely good spec. → wins over startup standards (Composio) and even OpenAI function calling (docs fall short of a real spec).
3. **[[anthropic|Anthropic]] has the best developer AI brand.** "If you're going to build a developer standard, it helps to be beloved by developers." MCP enables far more tools per call.
4. **Based on LSP** (Microsoft's Language Server Protocol) — adapted a proven protocol, kept JSON-RPC, client/server fungibility.
5. **Dogfooded** with a complete 1st-party client + 19 reference servers + tooling + SDKs (and later a second client in Claude Code). → wins over Meta's llama-stack.
6. **Minimal base, frequent roadmap updates.**
General law he draws out: standards convert "exploding MxN problems into tractable M+N ecosystem solutions" and only have value through adoption — "they only have value because they can get adoption." Postscript: OpenAI (3/27) and Google (4/9) adopted MCP after this post.

## Why it matters / where it cuts
The clearest practitioner account of *why* [[mcp|MCP]] became the agent-tooling standard — useful as the opinion-layer companion to the radar's [[agent-protocols]] research. It's also a generalizable handbook for how developer standards win (adoption > technical merit), and it under-weights the security cost that [[simon-willison]] flags ([[mcp|MCP]] makes mixing tools easy → the lethal trifecta).

## Graph
- **Author:** [[swyx]]
- **Concepts:** [[agent-protocols]] · [[tool-use]]
- **Entities:** [[mcp]] · [[anthropic]] · [[langgraph]] · [[openai]]
- **Raw:** `raw/blogs/2025-03-10-swyx-why-mcp-won.md`
