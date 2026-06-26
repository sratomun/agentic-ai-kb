---
type: source
source_type: blog
title: "Writing effective tools for AI agents — using AI agents"
author: Ken Aizawa (Anthropic)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/writing-tools-for-agents
resource: https://www.anthropic.com/engineering/writing-tools-for-agents
date: 2025-09-11
stake: Anthropic (sells Claude + the Agent SDK; originated MCP) — promotes its tool-use / MCP ecosystem
ingested: 2026-06-22
tags: [perspective, tool-use, agentic-ai, mcp]
---

# Writing effective tools for AI agents — using AI agents

**Blog** · Ken Aizawa ([[anthropic|Anthropic]] Engineering) · 2025-09-11 · [link](https://www.anthropic.com/engineering/writing-tools-for-agents)

**The take (attributed):** Anthropic argues that **tools are a new kind of software** — a contract between deterministic systems and *non-deterministic* agents — so you must design them *for agents*, not copy your existing APIs. The highest-leverage workflow: build an eval, then let **Claude Code optimize the tools against it**, which beat even expert-written tools.

**Stake:** Anthropic originated MCP and sells the model + Agent SDK; this grows its tool/MCP ecosystem and positions Claude Code as the optimizer.

## Argument
- **Tools ≠ APIs.** Don't merely wrap endpoints — agents have different "affordances" (limited context vs cheap computer memory). Build a few thoughtful, high-impact tools and consolidate (e.g., `schedule_event` over `list_users`+`list_events`+`create_event`; `get_customer_context` over three separate fetches).
- **Evaluation-driven loop:** prototype tools (wrap in a local MCP server / DXT), generate realistic multi-call eval tasks paired with verifiable outcomes, run simple agentic while-loops, collect accuracy + runtime + tool-call count + tokens + errors. **Then paste eval transcripts into Claude Code to refactor the tools** — held-out test sets showed gains beyond expert-written implementations.
- **Principles:** *namespacing* (prefix by service/resource, e.g. `asana_search`) reduces tool confusion; *return meaningful context* — resolve cryptic UUIDs to semantic names (cut hallucinations), expose a `response_format` enum (`concise`/`detailed`); *token efficiency* — pagination/filtering/truncation (Claude Code caps tool responses at 25,000 tokens by default), actionable error messages; *prompt-engineer descriptions* — name params unambiguously (`user_id` not `user`). Precise tool-description refinements drove Claude Sonnet 3.5 to SOTA on SWE-bench Verified.
- Candid note: "LLMs don't always say what they mean" — read between the lines of agent feedback.

## Why it matters / where it cuts
The canonical Anthropic playbook for **tool/MCP ergonomics** — the unglamorous layer that often determines whether an agent works. The "use Claude Code to optimize your own tools" loop is a concrete, against-naive-intuition tactic (more tools ≠ better). Pairs directly with [[2025-11-04-blog-anthropic-code-execution-with-mcp]] (token bloat at scale) and feeds [[tool-use]] and [[mcp]].

## Graph
- **Author:** [[anthropic|Anthropic]] Engineering
- **Entities:** [[anthropic]] · [[mcp]] · [[swe-bench]]
- **Concepts:** [[tool-use]] · [[agentic-ai]] · [[agent-evaluation]] · [[harness-engineering]] · [[coding-agents]]
- **Raw:** `raw/blogs/2025-09-11-anthropic-writing-tools-for-agents.md`
