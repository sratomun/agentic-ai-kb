---
type: concept
tags: [agents, hub, architectures, taxonomy]
created: 2026-06-21
updated: 2026-06-22
source_count: 3
---

# Agentic AI

*The hub of the radar: LLMs used not as text generators but as autonomous agents that perceive, reason, plan, act, and learn in a loop.*

## What it is
The umbrella concept for everything else here. An agentic system wraps a language model in a loop — perception, reasoning/planning, action (tool use), and memory — so it pursues multi-step goals instead of answering one prompt. The surveys converge on a shared decomposition (Perception · Brain · Planning · Action · [[tool-use|Tool Use]] · Collaboration) and on a shift from fixed API calls to open standards ([[mcp]], native computer use).

## Why it matters
The umbrella isn't where the decisions are — the layers are. What you actually choose about lives in [[agent-protocols]] (how agents connect), [[agent-skills]] (what they reuse), [[self-evolving-agents]] (how they improve), [[agentic-rl]] (how they're trained), [[agent-security]] (how they're contained), and [[agent-evaluation]] (how you know they work). The through-line of the recent literature: the bottleneck has moved from raw model capability to **architecture, protocols, and governance**.

## What the evidence shows
**2025 foundations.** The year drew the conceptual lines and the economic ones. A widely-cited taxonomy separated **"AI Agents"** (modular, tool-using, task-specific) from **"Agentic AI"** (multi-agent, goal-driven, a paradigm shift), giving the field shared definitions (→ [[2025-05-15-arxiv-2505-10468v5-ai-agents-vs-agentic-ai-a-conceptual-taxonomy]]). On architecture, **Plan-and-Act** showed splitting a high-level Planner from a low-level Executor (trained on synthetic plan data) is what unlocks long-horizon tasks (→ [[2025-03-12-arxiv-2503-09572v3-plan-and-act-improving-planning-of-agents-for]]), and the **foundation-agents** survey framed agents through brain-inspired modular architectures (→ [[2025-03-31-arxiv-2504-01990v2-advances-and-challenges-in-foundation-agents-from-brain]]). The most strategically useful 2025 argument: **small models are the future of agentic AI** — since agents make many repetitive, narrow calls, SLMs (e.g. Phi-3-small ~7B ≈ 70B-class on some tasks at ~15× lower cost) are often sufficient and far cheaper than routing everything to a frontier model (→ [[2025-06-02-arxiv-2506-02153v2-small-language-models-are-the-future-of-agentic]]).

**2026 developments.**
- The field is standardizing vocabulary (perceive/brain/plan/act/tool/collaborate) and interfaces ([[mcp]] + [[a2a-protocol|A2A]]) faster than it is standardizing evaluation.
- Recurring failure sets across surveys: hallucination-in-action, infinite loops, prompt injection — plus, at the enterprise layer, strategic-planning shortfalls (tracked in [[agent-evaluation]]).
- Governed execution (typed plans, compiled policy guardrails, audit traces) is emerging as the path to production for back-office/finance agents (→ [[polaris]]).
- Foundational 2026 surveys: unified architectures & taxonomy → [[2026-01-18-arxiv-2601-12560v1-agentic-ai-architectures-taxonomy]]; agentic-reasoning roadmap (foundational→self-evolving→collective) → [[2026-01-18-arxiv-2601-12538v1-agentic-reasoning-survey]]; governed enterprise automation → [[2026-01-16-arxiv-2601-11816v1-polaris-typed-planning-governed-execution]].

## Relationships
- commentary: [[demis-hassabis]] (agents are the path; continual learning the missing piece), [[jeff-dean]] ("year of agents"), [[andrej-karpathy]] ("Software 3.0")
- frontier-lab playbooks: OpenAI "practical guide to building agents" → [[2025-01-01-blog-openai-practical-guide-to-building-agents]]; Anthropic "context engineering" → [[2025-09-29-blog-anthropic-effective-context-engineering]]
- debate: [[debate-agents-vs-workflows]] (simplicity vs autonomy)
- debate: [[debate-llms-path-to-agi]] ([[yann-lecun]] vs [[sonya-huang]])
- cross-refs (methods/benchmarks/models): [[chain-of-thought]] · [[openai-o1]] · [[openai-o3]]
- sub-concepts: [[multi-agent-systems]], [[tool-use]], [[agent-memory]], [[agent-security]], [[self-evolving-agents]], [[agentic-rl]], [[agent-evaluation]], [[agent-protocols]], [[agent-skills]], [[agentic-rag]], [[intent-understanding]], [[intent-routing]]
- default model tier: [[small-language-models]] (the cheap workhorses most agent calls actually run on)
- standards: [[mcp]], [[a2a-protocol]], [[acp-protocol]]
- enterprise context: [[governance-gap]]
- cost discipline: [[agent-finops]] (what running agents costs, and how to govern it)
- adoption/practice: [[agent-adoption]] ([[ethan-mollick]])
- engineering practice: [[harness-engineering]], [[vibe-coding]]
- supply side: [[frontier-model-training]] (how the base models agents run on are made)

## Key 2025 papers (citation-ranked)
- **391** · [[2025-05-15-arxiv-2505-10468v5-ai-agents-vs-agentic-ai-a-conceptual-taxonomy|AI Agents vs. Agentic AI: A Conceptual Taxonomy, Applications and Challenges]]
- **358** · [[2025-08-08-arxiv-2508-06471v1-glm-4-5-agentic-reasoning-and-coding-arc|GLM-4.5: Agentic, Reasoning, and Coding (ARC) Foundation Models]]
- **296** · [[2025-07-28-arxiv-2507-20534v2-kimi-k2-open-agentic-intelligence|Kimi K2: Open Agentic Intelligence]]
- **277** · [[2025-06-02-arxiv-2506-02153v2-small-language-models-are-the-future-of-agentic|Small Language Models are the Future of Agentic AI]]
- **170** · [[2025-03-27-arxiv-2503-21460v1-large-language-model-agent-a-survey-on-methodology|Large Language Model Agent: A Survey on Methodology, Applications and Challenges]]
- **167** · [[2025-04-28-arxiv-2504-19678v2-from-llm-reasoning-to-autonomous-ai-agents-a|From LLM Reasoning to Autonomous AI Agents: A Comprehensive Review]]
- **162** · [[2025-03-12-arxiv-2503-09572v3-plan-and-act-improving-planning-of-agents-for|Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks]]
- **141** · [[2025-03-31-arxiv-2504-01990v2-advances-and-challenges-in-foundation-agents-from-brain|Advances and Challenges in Foundation Agents: From Brain-Inspired Intelligence ...]]
