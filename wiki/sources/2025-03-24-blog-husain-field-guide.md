---
type: source
source_type: blog
title: "A Field Guide to Rapidly Improving AI Products"
author: Hamel Husain
outlet: hamel.dev
url: https://hamel.dev/blog/posts/field-guide/
resource: https://hamel.dev/blog/posts/field-guide/
date: 2025-03-24
stake: Independent ML consultant (Parlance Labs); co-runs a paid Maven evals course — promotes evals/error-analysis as the discipline he teaches and sells.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, error-analysis]
---

# A Field Guide to Rapidly Improving AI Products

**Blog** · Hamel Husain (hamel.dev) · 2025-03-24 · [link](https://hamel.dev/blog/posts/field-guide/)

**The take (attributed):** Husain argues that the teams who actually improve AI products "barely talk about tools at all" — the bottleneck is **measurement and iteration**, and the single highest-ROI activity is **error analysis** (reading your own traces and categorizing failures), not picking the right framework, vector DB, or agent abstraction.

**Stake:** Drawn from his consulting with 30+ companies and the methodology he teaches in his paid evals course. Read his "tools don't matter, process does" framing knowing process-coaching is what he sells — but it's grounded in a large hands-on sample.

## Argument
Husain opens with a recurring scene from his consulting: a team proudly walks him through their RAG/router/framework architecture; he asks how they measure whether any of it works; the room goes quiet. After 30+ engagements, his thesis is that successful teams obsess over a tight measure→hypothesize→experiment loop rather than tooling. He lays out six moves:
1. **Error analysis is always the highest-ROI activity.** Sample real production traces, write open-ended notes on what went wrong, cluster into a failure-mode taxonomy, then *count* the modes. The counts tell you empirically where to invest — and the dominant failure is "almost never the one the team assumed." Error analysis precedes writing any eval: you can't test a failure you haven't discovered by looking at data.
2. **A simple data viewer is your most important investment.** A custom, low-friction trace-review interface (often a small notebook/FastHTML app tailored to the domain) beats generic vendor dashboards, because friction is what stops people from looking at data.
3. **Empower domain experts, not just engineers.** The subject-matter expert defines "good" and does the labeling; engineers build the tooling. Outsourcing labels or pushing them onto engineers produces bad data.
4. **Synthetic data is more effective than you think — if grounded.** Define the dimensions that matter (feature × scenario/persona) and generate systematically across that grid with edge cases, rather than naively asking an LLM for "50 queries."
5. **Maintain trust in your evals by validating LLM judges like classifiers** — human gold labels, train/dev/test, measure agreement, re-validate for drift; prefer binary pass/fail over Likert.
6. **Count experiments, not features.** A healthy AI roadmap is measured by experiment velocity against good measurement.

## Why it matters / where it cuts
This is the foundational statement of Husain's **evals-first** position and the radar's clearest articulation of the practitioner counter-thesis to framework-centric AI engineering: *the bottleneck is evals and error analysis, not orchestration frameworks.* It's the opinion-layer complement to the arxiv-grounded [[agent-evaluation]] concept — where the research layer shows aggregate benchmarks don't predict deployed behavior, Husain prescribes the workflow (read your own traces) that makes a team's measurement actually predictive. Feeds the [[debate-evals-vs-frameworks]] stance (evals, not frameworks, are the gating constraint on AI product quality). So what: this is the one-page operating manual to hand any team that's "building agents" but can't answer "how do you know it works."

## Graph
- **Author:** [[hamel-husain]]
- **Concepts:** [[agent-evaluation]] · [[llm-as-judge]]
- **Entities:** related to [[anthropic]] / [[openai]] (model-agnostic methodology)
- **Debate:** [[debate-evals-vs-frameworks]] (evals-over-frameworks stance)
- **Raw:** `raw/blogs/2025-03-24-husain-field-guide.md`
