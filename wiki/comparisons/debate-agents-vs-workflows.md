---
type: comparison
kind: debate
tags: [debate, perspective, multi-agent-systems, agentic-ai]
created: 2026-06-22
updated: 2026-06-22
status: converging
---

# Debate: Simple workflows, or autonomous agents?

*How much autonomy should you actually build? The practitioner consensus and the hype point in different directions.*

## The question
For a given task, do you build a **workflow** (LLMs/tools on predefined code paths) or an **autonomous agent** (the LLM directs its own process)? And how often is the right answer "neither — just a single augmented LLM call"?

## Positions

### "Simplicity first — workflows, maybe no agent at all"
- **Who:** [[anthropic]] (Erik Schluntz & Barry Zhang) — *stake: sells Claude + an Agent SDK, yet argues against frameworks (against-interest).*
- **Argument:** the most successful systems use **simple, composable patterns, not frameworks**; "find the simplest solution… this might mean not building agentic systems at all." Add autonomy only when it demonstrably pays for its latency/cost/error risk. → [[2024-12-19-blog-anthropic-building-effective-agents]]
- **Allies:** [[simon-willison]] (constrain agents for security); [[nathan-lambert]] (long-horizon behavior is *scaffolded*, not learned → [[2025-06-09-blog-lambert-what-comes-next-rl]]); [[chip-huyen]] ("don't use an agentic framework when direct API calls work" → [[2025-01-16-blog-huyen-ai-engineering-pitfalls]]).

### "Autonomy is the point — long-horizon agents"
- **Who:** [[sonya-huang]] (Sequoia) — *stake: VC, talking the agent-application book.*
- **Argument:** long-horizon **autonomous** agents are the breakthrough (functionally AGI); the application-layer **harness** + RL are what unlock value; build agents that sell work. → [[2026-01-14-blog-sonya-huang-2026-this-is-agi]]
- **Allies:** [[swyx]] (Agent Engineering / "Agent Labs" — autonomy is "the point" and where frontier value appears, *though he concedes via the Bitter Lesson that workflows win short-term until the next intelligence jump* → [[2025-03-24-blog-swyx-agent-engineering]] · [[2025-11-18-blog-swyx-agent-labs-thesis]]); the framework ecosystems ([[langgraph]], [[autogen]], [[crewai]]) and the AutoGPT-era maximalist tradition.

## Where it stands
*Converging toward "task-dependent, simplest-that-works" — and the research leans to the simplicity camp:*
- **Multi-agent often doesn't beat a single well-built agent:** the MAS failure taxonomy found minimal gains and mostly *coordination* failures across 7 frameworks (→ [[2025-03-17-arxiv-2503-13657v3-why-do-multi-agent-llm-systems-fail|via]] [[multi-agent-systems]] / [[agent-reliability]]).
- **More orchestration can *hurt*:** a negative ablation showed expanded orchestration failed to improve accuracy while raising cost/failures (ChromaFlow → [[agent-evaluation]]).
- **But autonomy is where the frontier value is appearing** — coding agents and [[deep-research-agents]] are genuinely autonomous loops, not workflows. Even Anthropic says agents win for "open-ended problems where you can't hardcode the path."

Honest read: **most production value today is workflows + a constrained agent**, with full autonomy reserved for verifiable, sandboxed domains. The hype/practice gap is real and closing.

## Relationships
- concerns [[multi-agent-systems]], [[agentic-ai]], [[agent-reliability]]
- participants: [[anthropic]] · [[sonya-huang]] · [[swyx]] · [[simon-willison]] · [[nathan-lambert]] · [[chip-huyen]]
