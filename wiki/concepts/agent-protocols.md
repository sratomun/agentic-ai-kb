---
type: concept
tags: [agents, protocols, interoperability, standards]
created: 2026-06-21
updated: 2026-06-22
source_count: 5
---

# Agent protocols

*The interoperability substrate — how agents reach tools and how they reach each other.*

## What it is
The standards layer beneath agent systems: [[mcp]] for agent→tool access, and peer protocols ([[a2a-protocol|A2A]], [[acp-protocol|ACP]]) for agent→agent discovery, negotiation, and delegation — plus the push to make workflow commitments *executable and enforceable* rather than buried in prompts.

## Why it matters
If agents are going to interoperate across vendors, the protocol layer is the battleground — and the practical bet you place when choosing a stack. It's also where two real costs bite: **efficiency** (the "MCP tax" of schema injection) and **security** ([[tool-description-poisoning]]). The open question to track: do A2A/ACP-style standards consolidate the way MCP did for tools, or does the field stay fragmented?

## What the evidence shows
**2025 foundations.** [[mcp|MCP]] shipped (Anthropic, late 2024) and adoption was explosive — 27k+ GitHub stars within four months. The literature raced to catalog the resulting protocol zoo: surveys mapped **MCP / ACP / A2A / ANP** as addressing interoperability at different layers and argued standardized protocols reduce integration overhead and improve security (→ [[2025-05-04-arxiv-2505-02279v2-a-survey-of-agent-interoperability-protocols-model-context]], [[2025-04-23-arxiv-2504-16736v3-a-survey-of-ai-agent-protocols]]). The other half of the 2025 story was **security**: the MCP Safety Audit showed industry-leading LLMs can be coerced through MCP tools to compromise a developer's system, and introduced McpSafetyScanner (→ [[2025-04-02-arxiv-2504-03767v2-mcp-safety-audit-llms-with-the-model-context]]); a broader survey catalogued 30+ host-to-tool and agent-to-agent attack techniques (→ [[2025-06-29-arxiv-2506-23260v2-from-prompt-injections-to-protocol-exploits-threats-in]]). Realistic MCP benchmarks followed (MCP-Universe, MCP-Bench — 250+ live tools).

**2026 developments.**
- The field now treats MCP (tools) + [[a2a-protocol|A2A]] (peers) as the two halves of the substrate; ACP adds decentralized identity + automated SLAs under zero-trust (→ [[2026-01-20-arxiv-2601-13671v1-orchestration-multi-agent-protocols-enterprise]], [[2026-02-11-arxiv-2602-15055v1-acp-agent-communication-protocol-a2a]]). The protocol surveys predict a **layered, federated stack rather than one winner**.
- **Reliability comes from moving commitments out of prompts into checkable structure** — declarative task graphs (DALIA → [[2026-01-24-arxiv-2601-17435v1-dalia-declarative-agentic-layer-mcp]]) and compiled protocols (XFlow → [[2026-06-11-arxiv-2606-14790v1-xflow-executable-protocol-multi-agent]]).
- **Protocol efficiency, not raw context length, is a binding constraint:** eager schema injection costs ~10k–60k tokens/turn; gated lazy loading cuts per-turn tool tokens ~95% (→ [[2026-04-23-arxiv-2604-21816v1-tool-attention-mcp-tax]]). The 2025 security thread continues via [[tool-description-poisoning]] and [[mcp-tdp-bench]].

## Relationships
- entities: [[mcp]], [[a2a-protocol]], [[acp-protocol]]
- efficiency: schema compilation [[tscg|TSCG]] (see [[2026-05-04-arxiv-2605-04107v1-tscg-tool-schema-compilation]])
- security: [[tool-description-poisoning]], [[mcp-tdp-bench]]
- substrate for [[multi-agent-systems]], [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **116** · [[2025-05-04-arxiv-2505-02279v2-a-survey-of-agent-interoperability-protocols-model-context|A survey of agent interoperability protocols: Model Context Protocol (MCP), Age...]]
- **90** · [[2025-04-23-arxiv-2504-16736v3-a-survey-of-ai-agent-protocols|A Survey of AI Agent Protocols]]
- **77** · [[2025-08-20-arxiv-2508-14704v1-mcp-universe-benchmarking-large-language-models-with-real|MCP-Universe: Benchmarking Large Language Models with Real-World Model Context ...]]
- **77** · [[2025-04-02-arxiv-2504-03767v2-mcp-safety-audit-llms-with-the-model-context|MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exp...]]
- **74** · [[2025-08-28-arxiv-2508-20453v1-mcp-bench-benchmarking-tool-using-llm-agents-with|MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks via...]]
- **73** · [[2025-06-29-arxiv-2506-23260v2-from-prompt-injections-to-protocol-exploits-threats-in|From Prompt Injections to Protocol Exploits: Threats in LLM-Powered AI Agents W...]]
