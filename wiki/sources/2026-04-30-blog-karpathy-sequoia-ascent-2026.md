---
type: source
source_type: blog
title: "Sequoia Ascent 2026 summary — Software 3.0, Agentic Engineering, Jagged Intelligence"
author: Andrej Karpathy
outlet: karpathy.bearblog.dev
url: https://karpathy.bearblog.dev/sequoia-ascent-2026/
resource: https://karpathy.bearblog.dev/sequoia-ascent-2026/
date: 2026-04-30
stake: Educator/communicator. Written ~weeks before joining Anthropic's pre-training team (announced May 19 2026); at time of writing still independent (Eureka Labs). The piece is itself an artifact of his thesis — he generated it with Codex 5.5 and reviewed it.
ingested: 2026-06-22
tags: [perspective, coding-agents, vibe-coding, agent-evaluation, llm-wiki, agentic-ai]
---

# Sequoia Ascent 2026: Software 3.0, Agentic Engineering, and Jagged Intelligence

**Blog** · Andrej Karpathy (karpathy.bearblog.dev) · 2026-04-30 · [link](https://karpathy.bearblog.dev/sequoia-ascent-2026/)
*(Karpathy's own write-up of his Sequoia Ascent fireside chat with Stephanie Zhan. He fed an LLM his blogs/tweets + the talk transcript to generate the summary and a cleaned transcript, then reviewed both — a meta-demonstration of the thesis. The talk itself is video; this captures the WRITTEN post.)*

**The take (attributed):** Karpathy argues we crossed a threshold around **December 2025** ("I have never felt more behind as a programmer") where coding agents got reliable enough that the unit of programming shifted from typing code to **delegating macro-actions** — and that this generalizes to **Software 3.0**: programming LLMs through the context window, with [[vibe-coding|vibe coding]] raising the floor and **agentic engineering** raising the ceiling.

**Stake:** Educator/communicator with no model or fund to sell at writing — but note this is partly a Sequoia (VC) stage and is pitched at founders ("that is a startup wedge"). Weeks later he joined [[anthropic]]'s pre-training team. The framings (Software 3.0, verifiability, jaggedness, agentic engineering) are his coinages and are doing taxonomy work for the field.

## Argument
- **Software 3.0:** Software 1.0 = humans write code; 2.0 = humans curate datasets/objectives and the program is learned into weights; **3.0 = humans program LLMs through prompts, context, tools, memory, instructions.** The context window is "the new program"; the LLM is an interpreter over it. Example: an install becomes a paste-able block of agent instructions instead of a brittle shell script.
- **Some apps should disappear:** his MenuGen app (photo of menu → OCR → image-gen → UI) collapses in the 3.0 version to "give the photo to a multimodal model, ask it to render dish images onto the menu directly." The app stack was scaffolding around a transformation the model now does directly.
- **The LLM-wiki pattern as the marquee example** of newly-possible information work: an agent incrementally compiles messy raw sources into a persistent Markdown wiki — summaries, entity pages, concept pages, contradictions, cross-links, logs, evolving synthesis — which "no classical program could robustly maintain." (This is the pattern [[llm-wiki|this radar itself runs on]].)
- **Verifiability + jaggedness (two axes):** traditional software automates what you can *specify*; LLMs/RL automate what you can *verify*. But capability also depends on **training attention**: `capability spike ~= verifiability × training attention × data coverage × economic value`. Chess improved at GPT-4 partly because chess data was added to the mix, not from smooth general gains. Frontier models "do not come with a manual" — the founder question is "are you on the model's rails?"
- **Vibe coding vs agentic engineering:** [[vibe-coding|vibe coding]] raises the floor (anyone can build); **agentic engineering** raises the ceiling — the discipline of coordinating fallible agents while preserving correctness, security, taste, maintainability (specs, plan supervision, diff review, tests, eval loops, permissions, isolated worktrees). The MenuGen Stripe-vs-Google-email bug is his canonical "human judgment still required" example (use persistent user IDs, not email matching). "The 10x engineer" may become far more extreme.
- **Hiring should change:** replace coding puzzles with "build a substantial project with agents, deploy it, secure it, then have adversarial agents try to break it."
- **Agent-native infrastructure:** most software is built for humans clicking screens, but increasingly "the user is the human's agent." Products need agent-native surfaces — Markdown docs, CLIs, APIs, [[mcp|MCP]] servers, structured logs, machine-readable schemas, copy-pasteable instructions, safe permissioning, auditable actions, headless flows. He frames this as **sensors and actuators**.
- **Ghosts, not animals:** LLMs are statistical simulations of human artifacts, not animal intelligences — jagged, alien tools demanding empirical familiarity (his *Animals vs Ghosts* post, Oct 2025; enumerated in [[andrej-karpathy]]).
- **Education:** "You can outsource your thinking, but you can't outsource your understanding." Understanding stays the bottleneck for directing agents; LLM knowledge bases are tools to build it.

## Why it matters / where it cuts
This is the densest single statement of Karpathy's worldview and the radar's clearest perspective-layer anchor for [[coding-agents]] and the agentic inflection. Two things make it unusually decision-relevant for the exec: (1) the **LLM-wiki pattern he champions IS the architecture this radar runs on** ([[llm-wiki]]) — external validation of the build; (2) the **agentic-engineering vs vibe-coding split** gives a clean policy line for an org — vibe coding for prototyping/enablement, agentic engineering (review, tests, evals, permissioning) for anything serious. The "are you on the model's rails?" / verifiability-times-training-attention framing is a practical lens for predicting where agents will fly vs fail in a given domain. Discount lightly for the founder-pitch venue.

## Graph
- **Author:** [[andrej-karpathy]]
- **Concepts:** [[coding-agents]] · [[vibe-coding]] · [[agent-evaluation]] · [[llm-wiki]] · [[agent-adoption]] · [[agentic-ai]]
- **Entities:** [[anthropic]] · [[mcp]] · [[claude]]
- **Related:** [[2025-04-07-blog-karpathy-power-to-the-people]]
- **Raw:** `raw/blogs/2026-04-30-karpathy-sequoia-ascent-2026.md`
