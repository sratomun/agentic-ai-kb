---
type: concept
tags: [agents, skills, capabilities, security]
created: 2026-06-21
updated: 2026-06-22
source_count: 3
---

# Agent skills

*The abstraction layer above tool calls: reusable, callable modules that package procedural knowledge — and a new software supply chain to secure.*

## What it is
Skills are composable units of *how to do something* — instructions + code + resources an agent loads on demand (the SKILL.md pattern), with applicability conditions, execution policies, and interfaces. They let an agent extend capability without retraining, and they can be discovered, distilled from experience, distributed, and reused.

## Why it matters
Skills are how agent capability becomes **composable and distributable** — and therefore how it becomes **attackable**. The same property that lets agents share a growing skill library lets a poisoned skill spread. This is the layer where the "agents that improve themselves" story ([[self-evolving-agents]]) meets the "agents as a supply chain" risk ([[agent-security]]).

## What the evidence shows
**2025 foundations.** The breakthrough was agents that *grow their own* skills. **SkillWeaver** had web agents self-improve by discovering and honing reusable skills through environment exploration, with relative success-rate gains of **31–54%** and transfer across agents (→ [[2025-04-09-arxiv-2504-07079v1-skillweaver-web-agents-can-self-improve-by-discovering]]). **Inducing Programmatic Skills (ASI)** showed *code* skills beat text skills — outperforming a static baseline on WebArena by **23%** while cutting steps (→ [[2025-04-09-arxiv-2504-06821v2-inducing-programmatic-skills-for-agentic-tasks]]). By year-end the loop was being baked into RL (Skill-Augmented GRPO for self-Evolution → [[2025-12-18-arxiv-2512-17102v2-reinforcement-learning-for-self-improving-agent-with-skill]]).

**2026 developments.** The field formalized the layer and confronted its risk: a SoK mapped the skill lifecycle and documented the **ClawHavoc** campaign (~1,200 malicious skills exfiltrating keys/wallets/credentials → [[2026-02-24-arxiv-2602-20867v1-sok-agentic-skills-beyond-tool-use]]); a companion survey found **26.1% of community skills carry vulnerabilities** and proposed four-tier trust governance (→ [[2026-02-12-arxiv-2602-12430v4-agent-skills-architecture-acquisition-security]]). Caveat from the SoK: *curated* skills lift success rates, but *self-generated* ones can degrade them — quality control is first-order.

## Relationships
- complements [[mcp]] and [[tool-use]]
- security overlaps [[agent-security]]
- acquisition overlaps [[self-evolving-agents]], [[agentic-rl]]
- benchmarks: [[swe-bench]], [[osworld]], [[webarena]]
- a capability layer of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **85** · [[2025-04-09-arxiv-2504-07079v1-skillweaver-web-agents-can-self-improve-by-discovering|SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills]]
- **62** · [[2025-04-09-arxiv-2504-06821v2-inducing-programmatic-skills-for-agentic-tasks|Inducing Programmatic Skills for Agentic Tasks]]
- **47** · [[2025-12-18-arxiv-2512-17102v2-reinforcement-learning-for-self-improving-agent-with-skill|Reinforcement Learning for Self-Improving Agent with Skill Library]]
