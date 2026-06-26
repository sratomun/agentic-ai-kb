---
type: concept
aliases: [agentic-engineering, vibe-engineering, agent-harness]
tags: [agents, coding-agents, harness-engineering, practice, perspective]
created: 2026-06-22
updated: 2026-06-22
kind: crosscutting
---

# Harness Engineering

*Designing the scaffold around a model — the loop, tools, memory, context management, verification, and human process — that turns a capable LLM into a reliable agent. The discipline behind "the harness, not the model, is the differentiator."*

## What it is
The **harness** is everything around the model weights: the agentic loop, tool interfaces, context/compaction strategy, memory, sub-agent orchestration, verification and feedback control, and the senior-engineering practices (tests, CI, code review, preview environments) that make it dependable. *Harness engineering* is the practice of building and improving that scaffold. The 2026 research framing puts it sharply: **code itself is the harness** — the operational substrate for agent reasoning, acting, environment-modeling, and execution-based verification. It's the technical-and-process counterpart to [[vibe-coding]]; the disciplined end Willison named "vibe engineering" (now converging on "agentic engineering"). Borders [[coding-agents]], [[agent-evaluation]], [[agent-memory]], and [[agentic-rl]].

## Why it matters
This is where the **build-vs-buy and where-to-invest** decision actually lives. If most agentic capability comes from the harness rather than the base model (the recurring practitioner claim), then the durable edge is in scaffold design and evaluation — not waiting for the next model. So what: the harness is the part you can own, version, and differentiate on, and it's why two teams on the *same* frontier model ship agents of wildly different reliability. The open problem is that harnesses are hard to evaluate — "evaluation beyond final task success" is the named frontier.

## What the evidence shows
**The research framing.** *Code as Agent Harness* (2026) organizes the field into three layers — the **harness interface** (code connecting agents to reasoning/action/environment), **harness mechanisms** (planning, memory, tool use, feedback-driven control), and **scaling** to multi-agent shared-code coordination — and explicitly names "**open challenges for harness engineering**": evaluation beyond task success, verification under incomplete feedback, regression-free improvement, consistent shared state, and human oversight (→ [[2026-05-18-arxiv-2605-18747v1-code-as-agent-harness]]). Related work treats agentic programming *for* the harness (→ [[2026-06-14-arxiv-2606-15874v1-llm-as-code-agentic-programming-for-agent-harness]]) and "harness-engineered" autonomous research agents (→ [[2026-05-03-arxiv-2605-02092v1-nora-a-harness-engineered-autonomous-research-agent-for]]).

**The practitioner consensus (perspective layer).** [[sebastian-raschka]] dissects the coding-agent harness component-by-component and argues it, not the model, is the differentiator (→ [[2026-04-04-blog-raschka-components-of-a-coding-agent]]). [[ethan-mollick]] explains the harness mechanics — compacting, skills, sub-agents, MCP — for non-coders (→ [[2026-01-07-blog-mollick-claude-code-and-what-comes-next]]). [[swyx]] makes the "Agent Labs" thesis that frontier value appears at the harness/application layer (→ [[2025-11-18-blog-swyx-agent-labs-thesis]]). [[hamel-husain]] reframes the harness as data-science/observability work — "the agent harness is data science" (→ [[2026-03-26-blog-husain-revenge-data-scientist]]). [[simon-willison]]'s "vibe engineering" enumerates the human-process half: tests, planning, docs, review, agentic loops (→ [[2025-10-07-blog-willison-vibe-engineering]]).

*Caveat: this is a fast-emerging concept (most evidence is 2026). The term "harness" is consistent across research and practice, but the boundary with [[coding-agents]] and [[agent-evaluation]] is still fuzzy.*

## Relationships
- Anthropic context-engineering & long-running harness → [[2025-09-29-blog-anthropic-effective-context-engineering]] · [[2025-11-26-blog-anthropic-effective-harnesses-long-running-agents]]; OpenAI Agents SDK harness → [[2025-03-11-blog-openai-new-tools-for-building-agents]]
- the scaffold around [[coding-agents]]; mechanisms draw on [[agent-memory]], [[tool-use]], [[agentic-rl]], [[mcp]], [[agent-skills]]
- evaluated by [[agent-evaluation]] (the "beyond final task success" problem) — see [[debate-evals-vs-frameworks]]
- the disciplined counterpart to [[vibe-coding]]
- includes the routing layer [[intent-routing]] (model/tool/sub-agent selection)
- budget as part of the scaffold: [[agent-finops]]
- perspective voices: [[sebastian-raschka]], [[swyx]], [[ethan-mollick]], [[hamel-husain]], [[simon-willison]]

## Key sources
- **research** · [[2026-05-18-arxiv-2605-18747v1-code-as-agent-harness|Code as Agent Harness (survey)]] · [[2026-06-14-arxiv-2606-15874v1-llm-as-code-agentic-programming-for-agent-harness]]
- **practice** · [[2026-04-04-blog-raschka-components-of-a-coding-agent]] · [[2025-11-18-blog-swyx-agent-labs-thesis]] · [[2026-03-26-blog-husain-revenge-data-scientist]]
