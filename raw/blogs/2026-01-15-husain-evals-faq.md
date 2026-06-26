---
source: hamel.dev
url: https://hamel.dev/blog/posts/evals-faq/
title: "LLM Evals: Everything You Need to Know (AI Evals FAQ)"
authors: [Hamel Husain, Shreya Shankar]
date: 2026-01-15
captured: 2026-06-22
note: Immutable raw capture. Cleaned full-text rendering from web_fetch (nav/boilerplate stripped). Q&A-format FAQ distilled from the authors' Maven "AI Evals for Engineers & PMs" course (4,500+ students). Co-authored with Shreya Shankar.
---

# LLM Evals: Everything You Need to Know (The AI Evals FAQ)

A long-form FAQ compiling the most common questions Hamel Husain and Shreya Shankar get from the 4,500+ students of their AI Evals course. It is the canonical reference for their evals methodology. Key questions and their answers, as the authors frame them:

## What are evals, and why do I need them?
"Evals" here means **product/application evals** — measuring whether *your* AI pipeline works on *your* task with *your* data — NOT foundation-model benchmarks (MMLU, HELM, etc.). Generic benchmarks tell you nothing about whether your specific application is failing. You need evals because LLM systems are stochastic and fail in long-tail, domain-specific ways you cannot anticipate without looking at your own data.

## Why is error analysis so important, and how is it performed?
Error analysis is the foundation. Process: (1) sample real traces; (2) write open-ended notes describing what went wrong (open coding); (3) cluster the notes into a taxonomy of failure modes (axial coding); (4) count how often each failure mode occurs. The counts tell you where to invest. The authors stress this is iterative and that the dominant failure mode is usually a surprise. Error analysis precedes writing any automated eval — you measure what's actually broken, not what you imagine is broken. "Axial coding" is the step most eval tools don't support well.

## How many traces should I look at / what's the sample size?
Look at enough traces to reach theoretical saturation (you stop discovering new failure modes). In practice this is often dozens to ~100 to start. Use the binomial/Wilson interval reasoning when you need a confidence interval on a failure rate — small samples have wide intervals, so don't over-trust a delta from a handful of examples.

## Should I build a custom annotation tool or use something off the shelf?
The authors lean toward **building a custom, minimal annotation/trace-review interface** tailored to your domain, because friction in reviewing data is the main thing that kills error analysis. Off-the-shelf tools are fine as a backend data store, but the review UX usually needs domain customization. (Husain typically uses vendor tools as a backend and Jupyter + custom interfaces for the human-review layer.)

## How do I build and trust an LLM-as-judge?
Treat the judge as a **classifier you must validate**: (1) get human gold labels; (2) split into train/dev/test; (3) iterate ("hill-climb") the judge prompt on the dev set, sourcing few-shot examples from the train set; (4) hold out a test set to confirm you didn't overfit; (5) report **TPR/TNR (or precision/recall)**, not raw accuracy — accuracy hides performance when a failure is rare; (6) correct for the judge's measured bias when estimating the true failure rate; (7) re-validate periodically (judges drift). Prefer **binary pass/fail** on a single, well-scoped criterion per judge over multi-criterion Likert scales — Likert hides ambiguity and is hard to validate.

## What about generic / off-the-shelf metrics (helpfulness, coherence, hallucination scores)?
Avoid them as primary signals. They're generic enough to be useless for diagnosing your application. Drive toward **application-specific, actionable** failure modes ("Calendar Scheduling Failure," "Failure to Escalate to Human"). Similarity metrics (ROUGE/BLEU/embedding cosine) rarely fit LLM outputs.

## How do I generate good synthetic / test data?
Ground synthetic data in real production logs. Identify the **dimensions** that matter (feature × scenario/persona), then systematically generate examples across that grid, injecting edge cases. Don't naively prompt "give me 50 queries" — you get unrepresentative data.

## RAG, fine-tuning, and other recurring questions
The FAQ addresses adjacent questions (when RAG still matters, retrieval evaluation, scoping multi-turn evals, observability) consistent with Husain's other writing: retrieval is more important than ever; evaluate retrieval and generation separately; scope evals tightly before automating.

## The "criteria drift" point
Drawing on Shankar et al.'s research, the authors emphasize **criteria drift**: people don't know their grading criteria until they look at outputs, and the act of labeling outputs is what defines the criteria. This is why you can't skip human review by asking an LLM to invent and apply a rubric in one shot.

---

(Cleaned rendering; Q&A structure and the authors' canonical terminology — error analysis, open/axial coding, TPR/TNR judge validation, criteria drift, binary pass/fail — preserved verbatim where load-bearing.)
