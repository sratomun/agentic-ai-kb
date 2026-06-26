---
type: source
source_type: arxiv
title: "MCPShield: A Security Cognition Layer for Adaptive Trust Calibration in Model Context Protocol Agents"
authors: Zhenhong Zhou, Yuanhe Zhang, Hongwei Cai, Moayad Aloqaily et al.
url: https://arxiv.org/abs/2602.14281v3
date: 2026-02-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CR
tags: [agent-security, agent-protocols, tool-use, arxiv, auto-ingested]
---

# MCPShield: A Security Cognition Layer for Adaptive Trust Calibration in Model Context Protocol Agents

**arXiv:** [2602.14281v3](https://arxiv.org/abs/2602.14281v3) · 2026-02-15 · cs.CR
**Authors:** Zhenhong Zhou, Yuanhe Zhang, Hongwei Cai, Moayad Aloqaily et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The Model Context Protocol (MCP) standardizes tool use for LLM-based agents and enable third-party servers. This openness introduces a security misalignment: agents implicitly trust tools exposed by potentially untrusted MCP servers. However, despite its excellent utility, existing agents typically offer limited validation for third-party MCP servers. As a result, agents remain vulnerable to MCP-based attacks that exploit the misalignment between agents and servers throughout the tool invocation lifecycle. In this paper, we propose MCPShield as a plug-in security cognition layer that mitigates this misalignment and ensures agent security when invoking MCP-based tools. Drawing inspiration from human experience-driven tool validation, MCPShield assists agent forms security cognition with metadata-guided probing before invocation. Our method constrains execution within controlled boundaries while cognizing runtime events, and subsequently updates security cognition by reasoning over historical traces after invocation, building on human post-use reflection on tool behavior. Experiments demonstrate that MCPShield exhibits strong generalization in defending against six novel MCP-based attack scenarios across six widely used agentic LLMs, while avoiding false positives on benign servers and incurring low deployment overhead. Overall, our work provides a practical and robust security safeguard for MCP-based tool invocation in open agent ecosystems.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14281v3)
