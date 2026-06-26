---
type: source
source_type: blog
title: "Selecting The Right AI Evals Tool"
author: Hamel Husain
outlet: hamel.dev
url: https://hamel.dev/blog/posts/eval-tools/
resource: https://hamel.dev/blog/posts/eval-tools/
date: 2025-10-01
stake: Independent ML consultant (Parlance Labs); the comparison is run through his paid course, and he has a stated personal preference (notebooks + custom interfaces) that colors the criteria.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, tools]
---

# Selecting The Right AI Evals Tool

**Blog** · Hamel Husain (hamel.dev) · 2025-10-01 · [link](https://hamel.dev/blog/posts/eval-tools/)

**The take (attributed):** There is no single best eval tool — Husain argues teams over-index on tooling when the process matters more, and offers *criteria* (and a live comparison of LangSmith, Braintrust, Arize Phoenix on the same task) rather than a winner. The throughline: favor tools that **empower human review and error analysis** and resist "magic" full-automation features.

**Stake:** He resists naming a winner partly on principle (tools change fast; process > tool) and partly because his own workflow (vendor as backend + Jupyter + custom annotation UIs) doesn't map onto any one vendor. Panel run inside his course.

## Argument
Husain had three dominant vendors — **LangSmith** (with LangChain CEO Harrison Chase), **Braintrust** (Wayde Gilliam), **Arize Phoenix** (SallyAnn DeLucia) — complete the *same* homework assignment (a recipe-chatbot), with a panel of Shreya Shankar, Bryan Bischof, and himself. Four assessment criteria emerged:
1. **Workflow / developer experience** — minimize time from observing a failure to iterating; notebook-centric flow is ideal for data-science teams (his preference); watch SDK ergonomics and integration.
2. **Human-in-the-loop support** — "error analysis is the highest ROI activity in AI engineering," so first-class manual annotation matters; many tools still lack **axial coding** support.
3. **Transparency vs "magic"** — be deeply skeptical of features that auto-create a rubric *and* immediately score with it ("stacking of abstractions" hides flaws behind a high score). Singles out Braintrust's "Loop" AI scorer as the cautionary example.
4. **Ecosystem integration vs walled gardens** — the tool should fit your stack; beware proprietary DSLs (e.g., Braintrust's BTQL); data export is a must-have.

Vendor snapshots (mid-2025): LangSmith — intuitive, smooth trace→playground, Annotation Queue, but cluttered UI and limited side-by-side comparison. Braintrust — clean UI, structured process, the "Money Table" of quantified failure modes, but the "Loop" auto-scorer and BTQL draw skepticism. Phoenix — notebook-centric, export to Pandas, open-source/local-first ("hackable"), a panelist's favorite OSS tool, but readability and aggregate-viz gaps. He personally uses these as a backend store plus Jupyter and custom annotation interfaces.

## Why it matters / where it cuts
The radar's most concrete **buyer's-guide** datapoint on the eval-tooling market, and a clean restatement of the human-in-the-loop principle: the most dangerous eval feature is an unvalidated AI scorer that manufactures false confidence — exactly the failure the arxiv layer documents ([[llm-as-judge]]: identical judge config flipping a guardrail's attack-success rate by 30×). Reinforces the evals-first position: tool choice is downstream of process. So what: if a team asks "which eval platform should we buy," these four criteria are the answer, and "none, until you've done error analysis" is the subtext.

## Graph
- **Author:** [[hamel-husain]]
- **Concepts:** [[agent-evaluation]] · [[llm-as-judge]]
- **Entities:** Braintrust · LangSmith · Arize Phoenix (eval-tool nodes — requested)
- **Debate:** [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2025-10-01-husain-eval-tools.md`
