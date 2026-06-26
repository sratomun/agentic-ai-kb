---
type: source
source_type: blog
title: "LLM Evals: Everything You Need to Know (AI Evals FAQ)"
author: Hamel Husain
co_authors: [Shreya Shankar]
outlet: hamel.dev
url: https://hamel.dev/blog/posts/evals-faq/
resource: https://hamel.dev/blog/posts/evals-faq/
date: 2026-01-15
stake: Independent ML consultant (Parlance Labs); the FAQ is distilled from the paid Maven evals course he co-teaches with Shreya Shankar (4,500+ students) — it doubles as marketing for that course.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, error-analysis]
---

# LLM Evals: Everything You Need to Know (The AI Evals FAQ)

**Blog** · Hamel Husain with Shreya Shankar (hamel.dev) · 2026-01-15 · [link](https://hamel.dev/blog/posts/evals-faq/)

**The take (attributed):** The authors argue there's a clean, teachable methodology for product evals that most teams skip — and that the canonical mistakes (generic metrics, unvalidated judges, Likert scales, outsourced labels, automating away human review) all stem from not doing **error analysis** and not treating the **LLM judge as a classifier you must validate**.

**Stake:** This is the reference companion to their 4,500-student paid course; it's both their most complete public methodology statement and a funnel for the course. Heavily co-authored with Shreya Shankar (academic eval researcher), which raises the rigor.

## Argument
A long Q&A compiling the questions they get most. The load-bearing answers:
- **"Evals" means product evals, not benchmarks.** Measuring whether *your* pipeline works on *your* task with *your* data — MMLU/HELM tell you nothing about your application.
- **Error analysis is the foundation.** Sample traces → open coding (notes on what went wrong) → axial coding (cluster into a failure taxonomy) → count. It's iterative, the dominant failure is usually a surprise, and it precedes any automated eval. Look at "enough traces to reach saturation" (often dozens to ~100 to start); use binomial/Wilson reasoning for confidence intervals on a failure rate.
- **Validate the LLM judge like a classifier.** Human gold labels, train/dev/test split, hill-climb the judge prompt on dev with few-shots from train, hold out test to avoid overfitting, report **TPR/TNR (or precision/recall) not accuracy** (accuracy hides rare failures), correct for the judge's measured bias, and re-validate (judges drift). Prefer **binary pass/fail on one scoped criterion** over multi-criterion Likert.
- **Avoid generic metrics** (helpfulness/coherence/hallucination scores, ROUGE/BLEU); drive toward application-specific, actionable failure modes.
- **Ground synthetic data** in real logs across the dimensions that matter; build a custom annotation interface (friction kills review).
- **Criteria drift** (per Shankar et al.): people don't know their grading criteria until they look at outputs, so you can't have an LLM invent-and-apply a rubric in one shot — the human labeling loop is what defines "good."

## Why it matters / where it cuts
This is the **canonical, citable statement** of the evals-first methodology — the perspective-layer anchor for [[llm-as-judge]] and [[agent-evaluation]]. It maps precisely onto the radar's arxiv findings: the research layer proves an LLM judge is "a stochastic, model-dependent component, not a measurement" (see [[llm-as-judge]]); Husain & Shankar give the validation protocol (TPR/TNR, bias correction, dev/test) that operationalizes that warning. So what: the single best link to send a team standing up evals, and the source that grounds the [[debate-evals-vs-frameworks]] position. Note Shankar's [criteria-drift / EvalGen] research is the academic backbone here.

## Graph
- **Author:** [[hamel-husain]] (with Shreya Shankar — node requested)
- **Concepts:** [[llm-as-judge]] · [[agent-evaluation]] · [[agentic-rag]] (RAG-eval sections)
- **Entities:** [[chip-huyen]] (adjacent practitioner voice on evals)
- **Debate:** [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2026-01-15-husain-evals-faq.md`
