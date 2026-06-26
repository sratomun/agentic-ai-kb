---
type: source
source_type: blog
title: "The lethal trifecta for AI agents"
author: Simon Willison
outlet: simonwillison.net
url: https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/
resource: https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/
date: 2025-06-16
stake: Independent practitioner/educator — minimal commercial stake
ingested: 2026-06-22
tags: [perspective, agent-security, agent-protocols]
---

# The lethal trifecta for AI agents

**Blog** · Simon Willison · 2025-06-16 · [link](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/)

**The take (attributed):** Willison argues prompt injection is a **structural, unsolved** risk: any agent combining three capabilities is exfiltration-ready, and **guardrails won't save you**.

**Stake:** Independent — coined "prompt injection" (2022); no vendor to sell, which is partly why the warning lands.

## Argument
- The **lethal trifecta** = (1) access to private data + (2) exposure to untrusted content + (3) ability to externally communicate. Combine all three and an attacker can trick the agent into stealing data.
- Root cause: "LLMs follow instructions in content" and can't reliably tell *whose* instructions to trust — everything is glued into one token stream.
- **Guardrails fail:** vendors touting "95% of attacks caught" — "95% is very much a failing grade" in security.
- **[[mcp|MCP]] makes it worse** by encouraging users to mix tools that hit all three legs.
- App-developer mitigations exist (CaMeL, the six design patterns: "once an agent has ingested untrusted input, it must be constrained so it can't trigger consequential actions") — but **end users mixing tools have only one option: avoid the trifecta**.

## Why it matters / where it cuts
The definitive practitioner framing of agent security, from the person who named the problem. It feeds the research debate on whether prompt injection is *solvable* (below) and is the opinion-layer counterpart to the radar's [[agent-security]] research.

## Graph
- **Author:** [[simon-willison]]
- **Concepts:** [[agent-security]] · [[tool-use]] · [[agent-protocols]]
- **Entities:** [[mcp]] · [[tool-description-poisoning]]
- **Debate:** [[debate-prompt-injection-solvable]]
- **Raw:** `raw/blogs/2025-06-16-simon-willison-lethal-trifecta.md`
