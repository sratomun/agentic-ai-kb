---
type: entity
entity_type: attack
tags: [agents, attack]
created: 2026-06-21
updated: 2026-06-22
---

# Tool Description Poisoning (TDP)

*A semantic attack class hiding malicious instructions in tool metadata — the 'manual' the agent reads during planning, not its executable code.*

## What it is
Tool Description Poisoning (TDP) embeds attacker-controlled instructions inside a tool's descriptive metadata (name, description, parameter docs) rather than its executable code. The agent reads these descriptions during planning and acts on the hidden instructions. Prompt guardrails are largely ineffective and can be counterproductive — the 'Firewall Fallacy'.

## Why it matters
TDP attacks the agent's planning layer, making them nearly invisible to conventional security tooling that monitors code execution and API calls. Any enterprise MCP deployment is exposed today: the only reliable defense is vetting tool sources, not filtering prompts.

## Relationships
- threatens [[agent-security]]
- exploits [[mcp]]
- benchmarked by [[mcp-tdp-bench]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-05-22-arxiv-2605-24069v1-mcp-poisoning-tool-description-attacks]]
