---
type: source
source_type: blog
title: "Components of A Coding Agent"
author: Sebastian Raschka
outlet: Ahead of AI
url: https://magazine.sebastianraschka.com/p/components-of-a-coding-agent
resource: https://magazine.sebastianraschka.com/p/components-of-a-coding-agent
date: 2026-04-04
stake: Educator/author (Build a Large Language Model / Build a Reasoning Model From Scratch); independent researcher (Raschka AI Research / RAIR Lab) — low commercial stake
ingested: 2026-06-22
tags: [perspective, coding-agents, agentic-ai, agent-memory, tool-use]
---

# Components of A Coding Agent

**Blog** · Sebastian Raschka (Ahead of AI) · 2026-04-04 · [link](https://magazine.sebastianraschka.com/p/components-of-a-coding-agent)

**The take (attributed):** Raschka's reference teardown of the **agent harness**. His load-bearing claim: with vanilla frontier LLMs now near-parity, **"the harness can often be the distinguishing factor that makes one LLM work better than another"** — "a lot of apparent 'model quality' is really context quality."

**Stake:** Independent educator/author — this accompanies his open-source [Mini Coding Agent](https://github.com/rasbt/mini-coding-agent) and his from-scratch books, not a commercial agent product. Low stake; a pedagogical "how it actually works" piece.

## Argument
- **Clean ontology:** LLM (raw next-token engine) → reasoning model (LLM trained/prompted for more inference-time compute, verification, search) → **agent** (a control loop around the model: decide what to inspect, which tools to call, when to stop) → **harness** (the software scaffold managing context, tools, prompts, state, control flow). A **coding harness** is the SWE-specific case (Claude Code, Codex).
- **Why harnesses matter:** "coding work is only partly about next-token generation. A lot of it is about repo navigation, search, function lookup, diff application, test execution, error inspection, and keeping all the relevant information in context." Speculates a strong open-weight model (GLM-5) dropped into a similar harness "could likely perform on par with GPT-5.4 in Codex or Claude Opus 4.6 in Claude Code" — though some harness-specific post-training helps (cites OpenAI's separate GPT-5.3-Codex variant).
- **Six components** (each in his from-scratch agent): (1) **Live repo context** — gather "stable facts" (git state, AGENTS.md/README) upfront; "fix the tests" isn't self-contained. (2) **Prompt shape & cache reuse** — a stable, cached prompt prefix (instructions, tool descriptions, workspace summary) vs changing per-turn state. (3) **[[tool-use|Structured tools, validation, permissions]]** — named tools with checks ("known tool? args valid? needs approval? path inside workspace?"); "the harness is giving the model less freedom, but it also improves usability and reliability." (4) **Context reduction** — clipping + recency-weighted transcript compression + dedup of repeated file reads. (5) **[[agent-memory|Structured session memory]]** — split working memory (distilled, task continuity) from a full resumable transcript (JSON on disk). (6) **[[multi-agent-systems|Delegation with bounded subagents]]** — the design problem is "not just how to spawn a subagent but also how to bind one" (read-only, bounded recursion); Claude Code long-supported, Codex added recently.
- **OpenClaw contrast:** a general local-agent platform (many long-lived agents across chats/channels), not a specialized terminal coding assistant — overlapping plumbing (instruction files, JSONL sessions, subagents), different emphasis.

## Why it matters / where it cuts
The radar's clearest practitioner anatomy of a [[coding-agents|coding agent]] / [[agentic-ai|agent harness]], and the explicit thesis that **the harness, not the model, is increasingly the differentiator** — which lands squarely on [[debate-agents-vs-workflows]] and the [[reasoning-models]]-vs-agents distinction. Concretely operationalizes [[agent-memory]], [[tool-use]], and [[multi-agent-systems|subagent delegation]]. Strong companion to [[nathan-lambert]]'s "agents push the humans up the org chart" — Raschka explains the *machinery* under that shift.

## Graph
- **Author:** [[sebastian-raschka]]
- **Concepts:** [[coding-agents]] · [[agentic-ai]] · [[agent-memory]] · [[tool-use]] · [[multi-agent-systems]]
- **Entities:** [[claude]] · [[gpt-5]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2026-04-04-sebastian-raschka-components-of-a-coding-agent.md`
