---
type: source
source_type: blog
title: "A Guide to Which AI to Use in the Agentic Era"
author: Ethan Mollick
outlet: One Useful Thing
url: https://www.oneusefulthing.org/p/a-guide-to-which-ai-to-use-in-the
resource: https://www.oneusefulthing.org/p/a-guide-to-which-ai-to-use-in-the
date: 2026-02-18
stake: Wharton/UPenn associate professor; Co-Intelligence author — adoption-optimist; heavy Anthropic favorability here
ingested: 2026-06-22
tags: [perspective, agent-adoption, agentic-ai, agent-evaluation]
---

# A Guide to Which AI to Use in the Agentic Era

**Blog** · Ethan Mollick (One Useful Thing) · 2026-02-18 · [link](https://www.oneusefulthing.org/p/a-guide-to-which-ai-to-use-in-the)

**The take (attributed):** Mollick argues "using AI" has fundamentally changed — you now choose along three axes, **Models, Apps, and Harnesses** — and increasingly "the app and harness matter more than the model." "An AI that does things is fundamentally more useful than an AI that says things."

**Stake:** Wharton/UPenn professor; Co-Intelligence author. This guide leans notably pro-Anthropic (detailed praise for Claude Code / Cowork / Excel; he gets early access) — discount the product enthusiasm; weight the taxonomy and the "pick the right model" advice.

## Argument
- His new mental model for choosing AI (a break from 7 prior guides):
  - **Models** = the brains (GPT-5.2/5.3, [[claude|Claude Opus 4.6]], [[gemini|Gemini 3 Pro]]) — "what the benchmarks measure."
  - **Apps** = products you use a model through (websites, phone apps, Codex, Claude Code, Claude Cowork).
  - **Harnesses** = "what let the power of AI models do real work" — the system giving the model tools/actions/multi-step autonomy. The same model behaves very differently by harness (Claude Opus 4.6 in a chat window vs inside Claude Code).
- **Practitioner advice (from-the-user's-seat [[agent-evaluation|model evaluation]]):** pay ≥$20/mo; free models are tuned for chat, not accuracy — most "AI did something stupid" examples are free/weak models. "The single most important thing… is pick the right model": manually select **GPT-5.2 Thinking Extended/Heavy** (or Pro), **Gemini 3 Pro/Thinking**, or **Claude Opus 4.6** with extended thinking on.
- **Harness gap:** OpenAI and Anthropic lead Google on chatbot harnesses — Claude.ai and ChatGPT produce working spreadsheets/PowerPoints with citations; Gemini's site can't yet, despite an equally good model.
- **Apps/harnesses beyond chat:** [[coding-agents|Claude Code / OpenAI Codex / Google Antigravity]] (coder-aimed but broadly capable — the 80-volume paper-GPT-1 anecdote); Claude for Excel/PowerPoint (in-app harnesses, "a junior analyst"); **Claude Cowork** ("Claude Code for non-technical work," runs in a VM with default-deny networking, "largely built *by* Claude Code in ~two weeks"); **NotebookLM** (sense-making); **OpenClaw** (viral local open-source agent — "a serious security risk… you almost definitely shouldn't use").

## Why it matters / where it cuts
The cleanest exec-readable framework for the agentic era: separating **model / app / harness** is exactly the distinction leaders need when deciding what to deploy, and his "pick the right model, the harness matters more" guidance is directly actionable. Feeds [[agent-adoption]] and the user-seat thread of [[agent-evaluation]]. Note this is also a useful primary-source snapshot of the early-2026 tool landscape (Cowork, OpenClaw, Manus→Meta).

## Graph
- **Author:** [[ethan-mollick]]
- **Concepts:** [[agent-adoption]] · [[agentic-ai]] · [[agent-evaluation]] · [[coding-agents]]
- **Entities:** [[claude]] · [[anthropic]] · [[gpt-5]] · [[gemini]] · [[google]]
- **Raw:** `raw/blogs/2026-02-18-mollick-guide-to-which-ai-agentic-era.md`
