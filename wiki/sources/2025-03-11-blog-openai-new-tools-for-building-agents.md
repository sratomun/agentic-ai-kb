---
type: source
source_type: blog
title: "New tools for building agents"
author: OpenAI
outlet: OpenAI news
url: https://openai.com/index/new-tools-for-building-agents/
resource: https://openai.com/index/new-tools-for-building-agents/
date: 2025-03-11
stake: Vendor platform launch — OpenAI is shipping and marketing the Responses API, built-in tools (web/file search, computer use), and the open-source Agents SDK. SimpleQA/OSWorld/WebArena/WebVoyager figures and customer quotes are OpenAI's own product claims, not radar fact.
ingested: 2026-06-22
tags: [perspective, agentic-ai, tool-use, computer-use-agents, multi-agent-systems, agent-protocols]
---

# New tools for building agents

**Blog** · OpenAI · 2025-03-11 · [link](https://openai.com/index/new-tools-for-building-agents/)

**The take (attributed):** OpenAI argues the gap between reasoning-capable models and production agents is an orchestration-and-tooling problem, and pitches itself as the platform that closes it — a new API primitive (Responses API), first-party built-in tools (web search, file search, computer use), and an open-source multi-agent SDK with handoffs, guardrails, and tracing.

**Stake:** This is a platform land-grab. OpenAI defines "agent" as "systems that independently accomplish tasks on behalf of users," then frames its own stack as the default way to build one. Discount the benchmark numbers (its own model/eval) and the customer logos; the durable signal is the architectural bet.

## Argument
OpenAI ships four things to make agents easier to build:
- **Responses API** — a new primitive combining Chat Completions' simplicity with the Assistants API's tool use. One call can chain multiple tools and model turns. OpenAI declares it "the future direction for building agents on OpenAI" and signals it will deprecate the [[mistral-agents-api|Assistants-style]] Assistants API with a mid-2026 sunset, pushing developers onto Responses.
- **Built-in tools** — web search (Hebbia cited; SimpleQA 90%/88% for gpt-4o/4o-mini search preview, OpenAI's number), file search (Navan; a managed RAG pipeline at $2.50/1k queries), and **computer use** powered by the same Computer-Using Agent (CUA) model behind [[computer-use-agents|Operator]]. CUA's self-reported SOTA: 38.1% OSWorld, 58.1% WebArena, 87% WebVoyager — but OpenAI itself flags 38.1% on OSWorld means "not yet highly reliable" for OS tasks and recommends human oversight.
- **Agents SDK** — open-source, the successor to OpenAI's Swarm experiment, with four primitives: configurable Agents, **Handoffs** (transfer control between agents), **Guardrails** (input/output safety checks), and **Tracing & Observability**. It works with the Responses API, Chat Completions, and any provider exposing a Chat-Completions-style endpoint (Coinbase, Box cited).

## Why it matters / where it cuts
This is the post that defines OpenAI's agent platform — the [[tool-use]] surface and [[multi-agent-systems|multi-agent]] orchestration model the rest of its 2025-26 agent stack ([[deep-research-agents|deep research]], [[coding-agents|Codex]], ChatGPT agent, AgentKit) builds on. So what: the strategic tell is that OpenAI bet on a first-party-tools + code-first SDK (web/file search, computer use bundled in) rather than ratifying [[mcp|MCP]] as the integration layer the way [[mistral-agents-api|Mistral]] did at launch — a closed-vs-open contrast worth tracking (OpenAI later added MCP support to deep research, Feb 2026). The Agents SDK's handoffs/guardrails/tracing vocabulary became the de-facto template others echo. It also feeds the [[debate-agents-vs-workflows|agents-vs-workflows]] question: OpenAI's framing is unapologetically "autonomous systems," with the reliability caveats buried in the computer-use section.

## Graph
- **Author:** [[openai]]
- **Concepts:** [[agentic-ai]] · [[tool-use]] · [[computer-use-agents]] · [[multi-agent-systems]] · [[agent-protocols]]
- **Entities:** [[openai]] · [[openai-o3]] · [[osworld]] · [[webarena]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2025-03-11-openai-new-tools-for-building-agents.md`
