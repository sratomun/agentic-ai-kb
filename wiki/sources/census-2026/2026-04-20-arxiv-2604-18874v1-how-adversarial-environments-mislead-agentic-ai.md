---
type: source
source_type: arxiv
title: "How Adversarial Environments Mislead Agentic AI?"
authors: Zhonghao Zhan, Huichi Zhou, Zhenhao Li, Peiyuan Jing et al.
url: https://arxiv.org/abs/2604.18874v1
date: 2026-04-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [embodied-agents, agent-reliability, agent-security, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# How Adversarial Environments Mislead Agentic AI?

**arXiv:** [2604.18874v1](https://arxiv.org/abs/2604.18874v1) · 2026-04-20 · cs.AI
**Authors:** Zhonghao Zhan, Huichi Zhou, Zhenhao Li, Peiyuan Jing et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-integrated agents are deployed on the premise that external tools ground their outputs in reality. Yet this very reliance creates a critical attack surface. Current evaluations benchmark capability in benign settings, asking "can the agent use tools correctly" but never "what if the tools lie". We identify this Trust Gap: agents are evaluated for performance, not for skepticism. We formalize this vulnerability as Adversarial Environmental Injection (AEI), a threat model where adversaries compromise tool outputs to deceive agents. AEI constitutes environmental deception: constructing a "fake world" of poisoned search results and fabricated reference networks around unsuspecting agents. We operationalize this via POTEMKIN, a Model Context Protocol (MCP)-compatible harness for plug-and-play robustness testing. We identify two orthogonal attack surfaces: The Illusion (breadth attacks) poison retrieval to induce epistemic drift toward false beliefs, while The Maze (depth attacks) exploit structural traps to cause policy collapse into infinite loops. Across 11,000+ runs on five frontier agents, we find a stark robustness gap: resistance to one attack often increases vulnerability to the other, demonstrating that epistemic and navigational robustness are distinct capabilities.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.18874v1)
