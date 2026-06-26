---
type: source
source_type: arxiv
title: "LAP: An Agent-to-Instrument Protocol for Autonomous Science"
authors: Linwu Zhu, Liqiang Gao, Yan Chen, Dan Zhu et al.
url: https://arxiv.org/abs/2606.03755v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [autonomous-driving-agents, embodied-agents, agent-security, agent-protocols, arxiv, auto-ingested]
---

# LAP: An Agent-to-Instrument Protocol for Autonomous Science

**arXiv:** [2606.03755v1](https://arxiv.org/abs/2606.03755v1) · 2026-06-02 · cs.AI
**Authors:** Linwu Zhu, Liqiang Gao, Yan Chen, Dan Zhu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous science is moving from demonstration to infrastructure. Large language model agents now plan experiments, and self-driving laboratories execute them. Yet every such system rebuilds the link between the reasoning agent and the physical instrument from scratch, against fragmented vendor SDKs and standards built for deterministic software clients rather than probabilistic, goal-directed agents. Recent agent-interoperability protocols clarify two of the three edges of an agentic ecosystem (Anthropic's Model Context Protocol (MCP) standardizes the agent-to-tool edge, and Google's Agent2Agent (A2A) the agent-to-agent edge), but neither models the agent-to-instrument edge, where operations are stateful, safety-critical, exclusively owned, physically embodied, and produce measurements with units, calibration, and uncertainty. We present the Lab Agent Protocol (LAP), a protocol design that fills this gap. LAP retains A2A's peer-to-peer, discovery-first, task-lifecycle structure and adds four physical-world primitives: (i) the InstrumentCard, a signed capability and physical-limit description; (ii) first-class reservation for exclusive instrument and sample locking; (iii) a safety-fence handshake with operator-confirmation tokens cryptographically bound to a specific task and its parameters, gating hazardous and irreversible operations; and (iv) a MeasurementResult schema that makes every result physically typed (QUDT/UCUM), calibration-anchored, uncertainty-bearing, and reproducible by construction. We specify roles, a six-layer architecture, the JSON-RPC method set, the task and safety state machines, the error model, and cross-laboratory federation, and walk a closed-loop autonomous campaign through the protocol end-to-end. LAP is transport-compatible with the A2A/MCP ecosystem and encapsulates rather than replaces existing device standards such as SiLA 2 and OPC-UA.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]] · [[a2a-protocol]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03755v1)
