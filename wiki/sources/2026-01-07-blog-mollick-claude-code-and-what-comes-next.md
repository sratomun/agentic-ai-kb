---
type: source
source_type: blog
title: "Claude Code and What Comes Next"
author: Ethan Mollick
outlet: One Useful Thing
url: https://www.oneusefulthing.org/p/claude-code-and-what-comes-next
resource: https://www.oneusefulthing.org/p/claude-code-and-what-comes-next
date: 2026-01-07
stake: Wharton/UPenn associate professor; Co-Intelligence author — adoption-optimist; early model access
ingested: 2026-06-22
tags: [perspective, coding-agents, agentic-ai, agent-skills]
---

# Claude Code and What Comes Next

**Blog** · Ethan Mollick (One Useful Thing) · 2026-01-07 · [link](https://www.oneusefulthing.org/p/claude-code-and-what-comes-next)

**The take (attributed):** Mollick argues coding agents made "a sudden capability leap in the past month or so" — driven not by one breakthrough but by **autonomous self-correcting models + an agentic harness** — and that the harness, not the model, is where the magic lives.

**Stake:** Wharton/UPenn professor; Co-Intelligence author; gets early access and is unabashedly enthusiastic about Anthropic's tools here. Weight the harness mechanics and capability-jump observation; discount the optimism.

## Argument
- Opening proof: one prompt ("make me $1000/month, do all the work") → Claude Code asked 3 questions, then worked **autonomously for 1h14m**, generating hundreds of files and deploying a working sales site with a live (working) Stripe link.
- The leap = **two advances combining**: (1) latest AIs do far more work autonomously while self-correcting (esp. programming — back-references [[2025-09-29-blog-mollick-real-ai-agents-and-real-work|Real AI Agents and Real Work]]); (2) an **agentic harness** of tools/approaches. Cites [[agent-evaluation|METR's]] length-of-task curve.
- The "magic tricks" — the harness mechanics he explains for a lay audience:
  - **Compacting:** when the context window fills, Claude Code takes notes on where it was, clears context, and a fresh instance resumes from the notes (the *Memento* analogy) — why it can run for hours. Touches [[agent-memory]].
  - **[[agent-skills|Skills]]:** instructions the AI decides when to invoke, bundling prompts *and* tools (Website Creator, Excel). Plain-language, AI-authorable; cites Jesse Vincent's "superpowers" skill set and Anthropic's Design Skill.
  - **Subagents:** specialized sub-AIs (own context windows), hand-off of easy tasks to cheaper models — "like a team." Touches [[multi-agent-systems]].
  - **[[acp-protocol|MCP]]:** publishers/payment/software companies expose tools to any model — "a smart generalist… can apply specialized skills on the fly."
- Because Claude Code works on your computer/files, "you have an AI that can do almost anything a human with access to your machine can do" (PowerPoint/Word "are just code") — with the attendant risks (deleting files, executing code, browser data). Recommends backups and a dedicated folder.
- Notes Claude Desktop now makes Claude Code accessible to non-CLI amateurs. Closes with **Karpathy**: "I've never felt this much behind as a programmer… failure to claim the boost feels decidedly like skill issue." Mollick: harnesses for *non-coding* knowledge work "are coming in the near future."

## Why it matters / where it cuts
The most legible explainer of *why* coding agents jumped — for a non-technical exec, it demystifies compacting / skills / subagents / MCP as the [[coding-agents|coding-agent]] stack. A from-the-practitioner's-seat capability claim that complements the research layer (and Lambert's parallel [[2026-01-09-blog-lambert-claude-code-hits-different|"Claude Code Hits Different"]] two days later). Feeds [[agent-adoption]] and [[agent-skills]].

## Graph
- **Author:** [[ethan-mollick]]
- **Concepts:** [[coding-agents]] · [[agentic-ai]] · [[agent-skills]] · [[agent-memory]] · [[multi-agent-systems]] · [[agent-adoption]]
- **Entities:** [[claude]] · [[anthropic]] · [[acp-protocol]]
- **Raw:** `raw/blogs/2026-01-07-mollick-claude-code-and-what-comes-next.md`
