---
type: entity
entity_type: benchmark
tags: [benchmark, agents, security, safety-alignment, evaluation]
created: 2026-06-21
updated: 2026-06-22
---

# AgentHarm

*A benchmark of harmful agentic task requests — measuring whether a tool-using agent refuses or executes explicitly harmful multi-step instructions.*

## What it is
AgentHarm (Andriushchenko et al., 2025) presents tool-using agents with 67 explicitly harmful agentic task requests and measures refusal rates. In the over-privileged tool selection study, AgentAlign training sharply reduced AgentHarm scores (e.g. 67.4%→10.5% for Ministral) — yet over-privileged tool selection stayed flat or rose, confirming the two failure modes are independent.

## Why it matters
Standard safety alignment does optimize for AgentHarm — but safe ≠ privilege-disciplined. This decoupling means enterprises can't rely on a single safety fine-tune to address both harm and over-privilege risk simultaneously.

## Relationships
- referenced by [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]
- evaluates [[agent-security]]

## Cited by
<!-- Auto-maintained by the kg-curator skill: the highest-cited source notes that reference this node. -->
- [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]
