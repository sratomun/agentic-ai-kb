---
type: entity
entity_type: product
tags: [agents, protocol, standard, tool-use, interoperability]
created: 2026-06-21
updated: 2026-06-22
---

# MCP

*Model Context Protocol — the open standard for how agents discover and call external tools and services.*

## What it is
An open protocol that standardizes the agent→tool interface: how an agent finds available tools, reads their schemas, and invokes them. It's become the de-facto connective layer for production agents — Forrester projects 30% of application vendors will ship MCP servers in 2026 — and is paired in the literature with peer-coordination protocols [[a2a-protocol|A2A]] and [[acp-protocol|ACP]] (agent→agent) as the two halves of the interoperability substrate.

## Why it matters
MCP is likely the standard you'll build or buy against, so its two liabilities are the ones to plan around: it's a **measured efficiency cost** (the "MCP tax" — eager schema injection runs ~10k–60k tokens/turn) and a **named attack surface** ([[tool-description-poisoning]], benchmarked by [[mcp-tdp-bench]]). Hardening the tool layer — effect typing, retry safety, schema compilation — matters before agents touch production.

## Relationships
- Anthropic "code execution with MCP" cuts tool-token bloat ~98.7% → [[2025-11-04-blog-anthropic-code-execution-with-mcp]]; tool ergonomics → [[2025-09-11-blog-anthropic-writing-tools-for-agents]]; OpenAI Connector Registry → [[2025-10-06-blog-openai-introducing-agentkit]]
- standard for [[tool-use]]; part of [[agent-protocols]]
- complemented by [[a2a-protocol]], [[acp-protocol]]
- efficiency fix: [[tscg]] (schema compilation)
- attacked via [[tool-description-poisoning]] (benchmark: [[mcp-tdp-bench]]); relevant to [[agent-security]]
- relates to [[agentic-ai]]
- adopted by [[mistral-agents-api]] (Studio Connectors → [[2026-05-22-blog-mistral-connectors-mcp-studio]]); commentary by [[simon-willison]]

## Cited by (2025 deep notes)
- **167** · [[2025-04-28-arxiv-2504-19678v2-from-llm-reasoning-to-autonomous-ai-agents-a|From LLM Reasoning to Autonomous AI Agents: A Comprehensive Review]]
- **116** · [[2025-05-04-arxiv-2505-02279v2-a-survey-of-agent-interoperability-protocols-model-context|A survey of agent interoperability protocols: Model Context Protocol (MCP), A...]]
- **107** · [[2025-06-22-arxiv-2506-18096v2-deep-research-agents-a-systematic-examination-and-roadmap|Deep Research Agents: A Systematic Examination And Roadmap]]
- **99** · [[2025-05-26-arxiv-2505-20286v1-alita-generalist-agent-enabling-scalable-agentic-reasoning-with|Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Pred...]]
- **77** · [[2025-08-20-arxiv-2508-14704v1-mcp-universe-benchmarking-large-language-models-with-real|MCP-Universe: Benchmarking Large Language Models with Real-World Model Contex...]]
- **77** · [[2025-04-02-arxiv-2504-03767v2-mcp-safety-audit-llms-with-the-model-context|MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security E...]]
- **74** · [[2025-08-28-arxiv-2508-20453v1-mcp-bench-benchmarking-tool-using-llm-agents-with|MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks v...]]
- **73** · [[2025-06-29-arxiv-2506-23260v2-from-prompt-injections-to-protocol-exploits-threats-in|From Prompt Injections to Protocol Exploits: Threats in LLM-Powered AI Agents...]]
