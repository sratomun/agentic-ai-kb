---
type: entity
entity_type: product
aliases: [Mistral Agents API, Mistral Connectors, Mistral Studio Connectors]
tags: [agents, product, agent-protocols]
created: 2026-06-22
updated: 2026-06-22
url: https://mistral.ai/news/agents-api
---

# Mistral Agents API

*Mistral's production framework for building tool-using, stateful, multi-agent applications — the agent-platform layer on top of its LLMs, with [[mcp|MCP]] as the open integration path.*

## What it is
A dedicated API (launched May 2025) that adds to Mistral's chat-completions three things bare LLM calls lack: **built-in connectors** (code execution, web search, image generation, document-library RAG, and MCP tools), **persistent stateful conversations** (branching, streaming), and **agent orchestration** via handoffs (agents delegate to one another). By May 2026 it generalized into **Connectors in Studio** — MCP integrations packaged as reusable, registered, governed entities, plus direct tool calling and human-in-the-loop (`requires_confirmation`) approval flows.

## Why it matters
It's a European frontier lab betting on [[mcp|MCP]] as the open standard rather than a proprietary tool format — a meaningful ratification of MCP's [[agent-protocols|protocol]] position. The 2026 Connectors release is the maturation from "we support MCP" to "we govern MCP as enterprise infra" (registration, observability, scoped tool permissions, approval gates) — which tacitly answers the [[agent-security]] concerns MCP raises. The concrete control surface (include/exclude tools, requires_confirmation) is a useful benchmark to hold other agent platforms to.

## Relationships
- made by [[mistral]]
- uses [[mcp]]
- supports [[tool-use]], [[multi-agent-systems]] (handoffs)
- relates to [[agent-security]] (human-in-the-loop, scoped tool permissions)
- competes with OpenAI Agents/Responses tooling, [[langgraph]]

## Cited by
- [[2025-05-27-blog-mistral-agents-api]]
- [[2026-05-22-blog-mistral-connectors-mcp-studio]]
