---
type: source
source_type: blog
title: "Agent Engineering"
author: swyx (Shawn Wang)
outlet: Latent.Space
url: https://www.latent.space/p/agent
resource: https://www.latent.space/p/agent
date: 2025-03-24
stake: Founder/CEO of AI Engineer + Latent Space — this essay elaborates his AIE Summit keynote and frames "Agent Engineering" as the discipline his conferences sell tickets to.
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-memory, tool-use, agent-evaluation]
---

# Agent Engineering

**Blog** · swyx (Shawn Wang) · 2025-03-24 · [link](https://www.latent.space/p/agent)

**The take (attributed):** swyx argues "agent" is best defined **descriptively, not prescriptively**, and distills 250+ practitioner definitions into **six elements (IMPACT)** an agent needs — and that Agent Engineering is "the hottest thing in AI Engineering" right now.

**Stake:** He named and now sells the discipline (AIE went "All In on Agent Engineering"); the essay doubles as a curated preview of his conference's agent talks.

## Argument
- On defining agents: "nobody agrees, and therefore debates about agent problems and frameworks are near-impossible since you can set the bar as low or as high as you want." Even within OpenAI definitions disagree (the SDK's "TRIM" = model + instructions + tools + runtime *forgets planning and memory* vs Lilian Weng's "LLM + memory + planning + tool use").
- **The Six Elements of Agent Engineering (IMPACT)**, ranked by commonality:
  - LLMs with **Tools** ([[tool-use]]) — the universally agreed core (Big 3: RAG/search, sandboxes, browsers/CUA).
  - Encoded **Intent** — multimodal I/O, goals, verified via [[agent-evaluation|evals]] in environments.
  - LLM-driven **Control Flow** — "the more agentic an application is, the more an LLM decides the control flow" (Harrison Chase); the workflow↔agent dividing line.
  - Multi-step **Planning** — SOTA is editable plans ([[deep-research-agents|Deep Research]], [[devin|Devin]], Manus).
  - Long-running **Memory** ([[agent-memory]]) — MemGPT/MCP memory plus Voyager/SteP reusable workflows and skill libraries.
  - Delegated **Authority** — "trust is the most overlooked element and yet the oldest" (principal-agent problem); "stutter-step agents" that confirm every action "get old fast."
- "You can FEEL when an agent forgets one of these 6 things."
- Chronicles the agent **sentiment cycle** (2023 AutoGPT hype → 2024 "AI winter" / "agents became a bad word" → 2024-25 reasoning-model resurgence), arguing the resurgence is real and on-trend (METR: agent task horizon doubles every 3-7 months).
- A cited footnote frames workflow-vs-agent as a **Bitter Lesson**: "workflows get you far in the short term, but often get steamrolled by the next order of magnitude gain in intelligence."

## Why it matters / where it cuts
The canonical practitioner taxonomy of what an agent *is* — a useful spine for the radar's [[agentic-ai]] and [[multi-agent-systems]] nodes, and a more agnostic counterweight to vendor-specific definitions. It feeds the **autonomy** debate: swyx leans pro-autonomy (Agent Engineering is "the point") but via that Bitter-Lesson footnote concedes workflows win short-term → [[debate-agents-vs-workflows]].

## Graph
- **Author:** [[swyx]]
- **Concepts:** [[agentic-ai]] · [[agent-memory]] · [[tool-use]] · [[agent-evaluation]] · [[deep-research-agents]]
- **Entities:** [[devin]] · [[mcp]] · [[anthropic]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2025-03-24-swyx-agent-engineering.md`
