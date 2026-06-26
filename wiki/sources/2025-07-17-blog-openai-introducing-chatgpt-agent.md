---
type: source
source_type: blog
title: "Introducing ChatGPT agent: bridging research and action"
author: OpenAI
outlet: OpenAI news
url: https://openai.com/index/introducing-chatgpt-agent/
resource: https://openai.com/index/introducing-chatgpt-agent/
date: 2025-07-17
stake: Vendor product launch — OpenAI unifying Operator + deep research into one agentic ChatGPT with its own virtual computer. HLE 41.6, FrontierMath 27.4%, BrowseComp 68.9%, SpreadsheetBench 45.5% are OpenAI's own elicited results (some third-party graded); SOTA claims are self-reported.
ingested: 2026-06-22
tags: [perspective, agentic-ai, computer-use-agents, deep-research-agents, tool-use, agent-security, agent-evaluation]
---

# Introducing ChatGPT agent: bridging research and action

**Blog** · OpenAI · 2025-07-17 · [link](https://openai.com/index/introducing-chatgpt-agent/)

**The take (attributed):** OpenAI argues the next step is a single agentic system that both *thinks and acts* — merging Operator's web interaction, deep research's synthesis, and ChatGPT's conversation onto one virtual computer — so ChatGPT can take real actions on the web end-to-end, with the user able to interrupt and take over.

**Stake:** Product launch and a capability-frontier claim. Every benchmark here is OpenAI's own elicitation; the "first time ChatGPT takes actions on the web" framing and the SOTA numbers are marketing the product. Notably, OpenAI also escalated its *own* risk rating (see below), which cuts against pure hype.

## Argument
ChatGPT agent is a unified agentic system folding three prior efforts into one: [[computer-use-agents|Operator]]'s website interaction, [[deep-research-agents|deep research]]'s synthesis, and ChatGPT's conversational layer — "a natural evolution of Operator and deep research." It carries a toolbox on its own virtual computer: a **visual browser** (GUI), a **text-based browser** (reasoning queries), a **terminal**, **direct API access**, and ChatGPT **connectors** (Gmail, GitHub), shifting fluidly between reasoning and action while preserving context ([[tool-use|tool use]] + [[harness-engineering|harness]] in one system).

Benchmarks (OpenAI's framing of SOTA):
- **Humanity's Last Exam:** pass@1 41.6 (44.4 with 8-attempt parallel rollout).
- **FrontierMath:** 27.4% with terminal/tool use.
- **[[browsecomp|BrowseComp]]:** 68.9%, +17.4 pts over deep research.
- **SpreadsheetBench:** 45.5% with direct .xlsx editing vs Copilot in Excel's 20.0%.
- Also claims wins on DSBench, [[webarena|WebArena]], internal IB modeling, and "economically valuable knowledge-work tasks."

On [[agent-security|safety]], OpenAI is unusually direct: this is "the first time users can ask ChatGPT to take actions on the web," raising the risk profile. Mitigations: prompt-injection defenses (training + monitoring + explicit confirmation), Watch Mode active supervision, proactive refusal of high-risk tasks (e.g. bank transfers). It treats the model as **High Biological and Chemical capabilities** under the Preparedness Framework — activating its "most comprehensive safety stack to date."

## Why it matters / where it cuts
This is the consolidation moment — OpenAI collapsing its separate agent products into one "thinks-and-acts" ChatGPT, and sunsetting the standalone Operator. So what: the SpreadsheetBench and IB-modeling claims are the ones that touch knowledge-work directly (a 45.5%-vs-20% spreadsheet gap, if it holds, is a real productivity wedge). The bigger signal is OpenAI voluntarily declaring **High** bio/chem capability and bolting on its heaviest safeguards — a self-reported escalation that's worth more than the benchmark theatre, and a data point for the [[agent-security|prompt-injection]] and [[debate-prompt-injection-solvable|"is prompt injection solvable"]] debate (a web-acting agent is exactly the lethal-trifecta surface skeptics warn about).

## Graph
- **Author:** [[openai]]
- **Concepts:** [[agentic-ai]] · [[computer-use-agents]] · [[deep-research-agents]] · [[tool-use]] · [[agent-security]] · [[agent-evaluation]] · [[harness-engineering]]
- **Entities:** [[openai]] · [[browsecomp]] · [[webarena]]
- **Debate:** [[debate-prompt-injection-solvable]]
- **Raw:** `raw/blogs/2025-07-17-openai-introducing-chatgpt-agent.md`
