---
type: source
source_type: blog
title: "How we built our multi-agent research system"
author: Jeremy Hadfield, Barry Zhang, Kenneth Lien, et al. (Anthropic)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/multi-agent-research-system
resource: https://www.anthropic.com/engineering/multi-agent-research-system
date: 2025-06-13
stake: Anthropic (sells Claude + the Agent SDK) — markets multi-agent orchestration on its own models
ingested: 2026-06-22
tags: [perspective, multi-agent-systems, agentic-ai, agent-evaluation]
---

# How we built our multi-agent research system

**Blog** · Jeremy Hadfield, Barry Zhang, Kenneth Lien et al. ([[anthropic|Anthropic]] Engineering) · 2025-06-13 · [link](https://www.anthropic.com/engineering/multi-agent-research-system)

**The take (attributed):** Anthropic argues that for **breadth-first, open-ended research**, an **orchestrator-worker multi-agent** system (a lead agent spawning parallel subagents with isolated context windows) beats a single agent — chiefly because it lets you *spend more tokens in parallel*, which they find explains most of the performance.

**Stake:** Anthropic sells Claude and the Agent SDK and ships this as the Claude Research feature — they're showcasing their own orchestration on their own models. Note the candid against-interest caveats: multi-agent burns ~15× the tokens of chat, and is a *bad* fit for coding and for tasks with heavy inter-agent dependencies.

## Argument
- **Why multi-agent:** research is dynamic and path-dependent; you can't hardcode the steps. Subagents do *compression* — each explores an aspect in its own context window and returns only distilled tokens to the lead agent, giving separation of concerns and reduced path dependency.
- **The headline number:** a multi-agent system (Claude Opus 4 lead + Claude Sonnet 4 subagents) **outperformed single-agent Opus 4 by 90.2%** on their internal research eval.
- **Tokens explain performance:** on BrowseComp, three factors explained 95% of variance — **token usage alone explained 80%**, plus number of tool calls and model choice. This validates distributing work across separate context windows.
- **The cost:** agents use ~4× chat tokens; multi-agent ~15× → only viable for high-value tasks. Poor fit where agents must share context or coordinate in real time (e.g., most coding).
- **Architecture:** orchestrator-worker. LeadResearcher plans → saves plan to memory (context truncates past 200K tokens) → spawns subagents (interleaved thinking) → synthesizes → a CitationAgent attributes claims to sources.
- **Prompt-engineering heuristics:** think like your agents (simulate); teach the orchestrator to delegate with explicit objectives/boundaries; scale effort to complexity (1 agent / 3–10 calls for simple; >10 subagents for complex); a tool-testing agent that rewrites bad MCP tool descriptions cut task time 40%; start wide then narrow; parallel tool-calling cut research time up to 90%.
- **Evals:** start with ~20 real queries; LLM-as-judge on a rubric (factual/citation accuracy, completeness, source quality, tool efficiency); human eval caught a bias toward SEO content farms over authoritative sources.
- **Production:** errors compound in stateful agents → resumable execution, retries, checkpoints, rainbow deployments, full tracing (without reading conversation contents).

## Why it matters / where it cuts
The most concrete practitioner account of *production* multi-agent orchestration, with real numbers (90.2% lift, 15× token cost, the 80% token-variance finding). It both validates multi-agent for high-value parallel research **and** explicitly bounds it — coding and tightly-coupled tasks need not apply. Useful counterweight to "multi-agent everything" hype, and a direct input to [[debate-agents-vs-workflows]] (here Anthropic endorses *more* autonomy/agents where the task fits).

## Graph
- **Author:** [[anthropic|Anthropic]] (Applied/Research)
- **Entities:** [[anthropic]] · [[mcp]] · [[claude]]
- **Concepts:** [[multi-agent-systems]] · [[agentic-ai]] · [[agent-evaluation]] · [[agent-memory]] · [[tool-use]] · [[harness-engineering]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2025-06-13-anthropic-multi-agent-research-system.md`
