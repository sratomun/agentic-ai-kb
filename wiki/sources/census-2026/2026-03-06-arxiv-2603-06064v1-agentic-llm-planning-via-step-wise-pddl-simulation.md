---
type: source
source_type: arxiv
title: "Agentic LLM Planning via Step-Wise PDDL Simulation: An Empirical Characterisation"
authors: Kai Göbel, Pierrick Lorang, Patrik Zips, Tobias Glück
url: https://arxiv.org/abs/2603.06064v1
date: 2026-03-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, embodied-agents, agent-protocols, tool-use, arxiv, auto-ingested]
---

# Agentic LLM Planning via Step-Wise PDDL Simulation: An Empirical Characterisation

**arXiv:** [2603.06064v1](https://arxiv.org/abs/2603.06064v1) · 2026-03-06 · cs.AI
**Authors:** Kai Göbel, Pierrick Lorang, Patrik Zips, Tobias Glück

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Task planning, the problem of sequencing actions to reach a goal from an initial state, is a core capability requirement for autonomous robotic systems. Whether large language models (LLMs) can serve as viable planners alongside classical symbolic methods remains an open question. We present PyPDDLEngine, an open-source Planning Domain Definition Language (PDDL) simulation engine that exposes planning operations as LLM tool calls through a Model Context Protocol (MCP) interface. Rather than committing to a complete action sequence upfront, the LLM acts as an interactive search policy that selects one action at a time, observes each resulting state, and can reset and retry. We evaluate four approaches on 102 International Planning Competition (IPC) Blocksworld instances under a uniform 180-second budget: Fast Downward lama-first and seq-sat-lama-2011 as classical baselines, direct LLM planning (Claude Haiku 4.5), and agentic LLM planning via PyPDDLEngine. Fast Downward achieves 85.3% success. The direct and agentic LLM approaches achieve 63.7% and 66.7%, respectively, a consistent but modest three-percentage-point advantage for the agentic approach at $5.7\times$ higher token cost per solution. Across most co-solved difficulty blocks, both LLM approaches produce shorter plans than seq-sat-lama-2011 despite its iterative quality improvement, a result consistent with training-data recall rather than generalisable planning. These results suggest that agentic gains depend on the nature of environmental feedback. Coding agents benefit from externally grounded signals such as compiler errors and test failures, whereas PDDL step feedback is self-assessed, leaving the agent to evaluate its own progress without external verification.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]] · [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.06064v1)
