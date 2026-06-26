---
type: source
source_type: blog
title: "The Revenge of the Data Scientist"
author: Hamel Husain
outlet: hamel.dev
url: https://hamel.dev/blog/posts/revenge/
resource: https://hamel.dev/blog/posts/revenge/
date: 2026-03-26
stake: Independent ML consultant (Parlance Labs); co-runs a paid evals course. The "evals = data science" framing elevates the discipline he teaches; the post also markets his evals-skills plugin.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, coding-agents, harness-engineering]
---

# The Revenge of the Data Scientist

**Blog / talk (PyAI Conf)** · Hamel Husain (hamel.dev) · 2026-03-26 · [link](https://hamel.dev/blog/posts/revenge/)

**The take (attributed):** Husain argues that the agent/harness era doesn't make data scientists obsolete — it makes them essential. The "harness" that bounds autonomous coding agents (tests, specs, AND **metrics/observability**) is, in large part, data-science work: experimental design, model evaluation, EDA, data collection, production ML. The names changed; the work didn't.

**Stake:** A morale-and-relevance argument for the audience he serves (data scientists/MLEs) and a re-framing that positions evals (his product) as the durable, defensible skill in an agent-built-software world.

## Argument
Provoked by the "is data science dead?" anxiety after foundation-model APIs let any team ship AI without an MLE on the critical path. Husain's counter: training models was never most of the job — the job is testing generalization, debugging stochastic systems, and designing metrics, none of which the API removed.

He anchors on **OpenAI's "[[harness-engineering|harness engineering]]"** post (Codex agents building a product over months, autonomously) and notes the easily-missed detail: the harness includes an **observability stack — logs, metrics, traces exposed to the agent so it can tell when it's going off track.** Karpathy's auto-research project shows the same pattern (models optimizing against a validation-loss metric). His claim: *a large portion of the harness is data science.* Today teams build on "vibes," ask the model if it did a good job, and grab off-the-shelf metric libraries without looking at data.

He then walks five eval pitfalls, each mapped to a data-science fundamental:
1. **Generic metrics** (helpfulness/coherence/hallucination dashboards are useless for diagnosis) → do EDA; read traces; drive toward application-specific failure modes ("Calendar Scheduling Failure," "Failure to Escalate to Human"). *"If there is one thing to take away: look at the data."*
2. **Unverified judges** → treat the judge as a classifier; human labels, train/dev/test, hill-climb the prompt; report **precision/recall, not accuracy** ("if a failure mode occurs 5% of the time, accuracy hides the system's true performance"). "Verifying classifiers has become a lost art."
3. **Bad experimental design** → ground synthetic test sets in real production data along the dimensions that matter; replace 1-5 Likert rubrics-in-one-call with binary pass/fail on scoped criteria.
4. **Bad data and labels** → domain experts label, stay skeptical; invokes **criteria drift** (Shankar et al., arXiv:2404.12272) — you don't know what you want until you see outputs.
5. **Automating too much** → LLMs write the plumbing but can't look at the data for you.

The mapping: EDA / Model Evaluation / Experimental Design / Data Collection / Production ML. Companion: his open-source evals-skills (his OSS eval toolkit) plugin.

## Why it matters / where it cuts
This is Husain's sharpest **agent-era** framing: it directly connects the radar's harness engineering / [[coding-agents]] thread to [[agent-evaluation]] — the harness's metric layer is the eval problem, so the field's eval debt becomes the bottleneck on autonomous-agent reliability. It also restates the evals-first thesis with the strongest one-liner for an exec ("look at the data; the highest-ROI activity is the one everyone skips"). Feeds [[debate-evals-vs-frameworks]]. So what: useful counter-narrative to "agents make MLEs redundant" — the opposite is closer to true, and the leverage moves to whoever can measure.

## Graph
- **Author:** [[hamel-husain]]
- **Concepts:** [[agent-evaluation]] · [[llm-as-judge]] · [[coding-agents]]
- **Entities:** [[openai]] (harness-engineering source); evals-skills (his OSS eval toolkit) (his plugin — node requested)
- **Debate:** [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2026-03-26-husain-revenge-data-scientist.md`
