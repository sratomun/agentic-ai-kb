---
type: source
source_type: blog
title: "Agents"
author: Chip Huyen
outlet: huyenchip.com (adapted from *AI Engineering*, O'Reilly 2025)
url: https://huyenchip.com/2025/01/07/agents.html
resource: https://huyenchip.com/2025/01/07/agents.html
date: 2025-01-07
stake: Author of *AI Engineering* (O'Reilly, 2025) — post excerpts/markets the book; vendor-neutral practitioner-educator lens. Now building in robotics
ingested: 2026-06-22
tags: [perspective, agentic-ai, tool-use, agent-evaluation, multi-agent-systems]
---

# Agents

**Blog** · Chip Huyen (huyenchip.com — adapted from *AI Engineering*, O'Reilly 2025) · 2025-01-07 · [link](https://huyenchip.com/2025/01/07/agents.html)

**The take (attributed):** Huyen argues an agent is just **"anything that can perceive its environment and act upon it"** — defined by its *environment* and its *tool inventory* — so the agentic pattern is **inevitable** but unglamorous: ChatGPT and RAG are already agents. The hard parts are **planning, tool selection, and a discipline of failure-mode evaluation**, not the "agent" label.

**Stake:** This is the canonical public version of the **Agents** chapter of her book *AI Engineering* — so it markets the book, but she sells no model or framework (vendor-neutral). Read it as a practitioner's reference framework, not a product pitch.

## Argument
- **Definition first, hype later.** An agent = environment + action set; the action set is augmented by **[[tool-use|tools]]**. There's a tight coupling: the environment determines available tools; the tool inventory restricts the workable environment. By this definition "ChatGPT is an agent … RAG systems are agents."
- **Why agents need stronger models — two reasons, one of them quantified.** *Compound mistakes*: at 95% per-step accuracy, 10 steps → 60%, 100 steps → **0.6%**. *Higher stakes*: tool access raises the blast radius of any failure. (This compounding-error math is the post's most-cited line and a core argument for [[agent-reliability]].)
- **Tools come in three buckets:** knowledge augmentation (retrievers, SQL, web browsing — "prevents a model from going stale"), capability extension (calculator, code interpreter, OCR/transcription — Chameleon: GPT-4 + 13 tools beats GPT-4 alone, +11.37% ScienceQA / +17% TabMWP), and **write actions** (send email, initiate transfer) — which she flags as the dangerous ones ("you shouldn't allow an unreliable AI to initiate bank transfers").
- **Decouple planning from execution.** Generate a plan → **validate it** (heuristics or an AI judge) → only then execute, so a bad 1,000-step plan can't burn hours of API spend. This split yields plan-generator / validator / executor components — and her notable framing: *"most agents are multi-agent"* because most agentic workflows are complex enough to need several components. (Feeds [[multi-agent-systems]].)
- **On the LeCun "LLMs can't plan" claim — she pushes back.** Planning is fundamentally a *search* problem; autoregressive models *can* backtrack (revise or restart a path), and may be poor planners mainly because they lack the **tooling** to predict action outcomes (a world model). "Even if AI can't plan, it can still be *part of* a planner." Predicts FM-agents and RL-agents will eventually merge. (Direct counter to [[yann-lecun]].)
- **Practitioner mechanics:** function-calling (`required`/`none`/`auto`; APIs guarantee valid function *names* but not correct *params*); prefer **natural-language plans + a translator** over hard-coded function names (robust to tool-API churn); hierarchical planning to dodge the granularity tradeoff; control flows beyond sequential (parallel / if = "routing" / loop). Reflection via **[[react|ReAct]]** (Thought/Act/Observation) and **Reflexion** (evaluator + self-reflection) — cheap, big gains, but token/latency heavy.
- **Tool selection is empirical:** ablate each tool (drop it; if no perf drop, remove it), plot tool-call distributions; different models have different tool preferences (Gorilla pushed to 1,645 APIs — usually too many).
- **Evaluation = detecting failure modes.** Three agent-specific families: **planning failures** (invalid tool / valid-tool-invalid-params / wrong param values; goal failure; overlooked **time** constraint; *reflection error* — agent insists it's done when it isn't), **tool failures** (right tool, wrong output; translation errors — test each tool independently, print every call), and **efficiency** (avg steps / cost / time per task vs a human or agent baseline). Concrete metric recipe: build a (task, tool-inventory) dataset, generate K plans, measure % valid plans and tool-call error rates.

## Why it matters / where it cuts
This is the **practitioner's canonical reference** for what an agent actually is and how to evaluate one — pre-dating most of the 2025-26 arxiv eval literature but anticipating it (her failure taxonomy maps cleanly onto the radar's [[agent-evaluation]] and [[agent-reliability]] work). Two stances make it load-bearing for the radar's debates:
- Her **"most agents are multi-agent"** decomposition is a useful counterweight to the radar's research finding that multi-agent often *doesn't* beat a single strong agent — she means *components*, not competing autonomous agents, which dissolves part of the apparent disagreement in [[debate-agents-vs-workflows]].
- Her **compound-error math** (0.6% over 100 steps) is the cleanest one-line argument for why long-horizon reliability — not raw capability — is the binding constraint on agents.
She explicitly aligns with Anthropic's "Building Effective Agents" but claims her piece covers *why and how* things work (planning, tool selection, failure modes) vs Anthropic's isolated patterns.

## Graph
- **Author:** [[chip-huyen]]
- **Concepts:** [[agentic-ai]] · [[tool-use]] · [[agent-evaluation]] · [[multi-agent-systems]] · [[agent-reliability]] · [[agent-memory]] · [[reasoning-models]]
- **Entities:** [[react|ReAct]] · [[anthropic]] · [[yann-lecun]]
- **Debate:** [[debate-agents-vs-workflows]] (ally of the simplicity / "components not frameworks" camp)
- **Raw:** `raw/blogs/2025-01-07-chip-huyen-agents.md`
