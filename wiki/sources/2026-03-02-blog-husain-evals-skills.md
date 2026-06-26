---
type: source
source_type: blog
title: "Evals Skills for Coding Agents"
author: Hamel Husain
outlet: hamel.dev
url: https://hamel.dev/blog/posts/evals-skills/
resource: https://hamel.dev/blog/posts/evals-skills/
date: 2026-03-02
stake: Independent ML consultant (Parlance Labs); ships the evals-skills OSS plugin and co-runs a paid evals course (4,000+ students cited) — the post launches his own tool.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, coding-agents, skills]
---

# Evals Skills for Coding Agents

**Blog** · Hamel Husain (hamel.dev) · 2026-03-02 · [link](https://hamel.dev/blog/posts/evals-skills/)

**The take (attributed):** Coding agents can now do the *tedious* eval plumbing (instrument the app, orchestrate experiments, build annotation UIs) — but an agent with an eval platform "still needs to know what to do with it." Husain ships **evals-skills**, a plugin encoding the judgement (error analysis, judge validation, scoped failure modes) that vendor MCP servers don't provide.

**Stake:** This is a launch post for his own OSS plugin and a pointer to his course; the methodology and the product are the same thing.

## Argument
Husain frames coding agents as the new operators of the eval workflow. He cites **OpenAI's harness-engineering** result — a product built entirely with Codex agents (three engineers, five months, ~1M lines of code) where *improving the infrastructure around the agent mattered more than improving the model*; agents queried traces to verify their own work. All major eval vendors (Braintrust, LangSmith, Phoenix/Arize, Truesight) now ship MCP servers, so instrumentation/experiment-orchestration/annotation-tooling falls to agents.

But the agent still needs domain judgement. His example: a support bot saying "your plan includes free returns" (a wrong fact) vs "I've canceled your order" when nobody asked (a fabricated action) are *different* failure modes — lump them into a generic "hallucination score" and you miss errors. The skills encode this. He ships:
- **eval-audit** — diagnostic across six areas, prioritized problem list (recommended via parallel subagents).
- **error-analysis** — read traces, categorize failures, build a vocabulary of what's broken.
- **generate-synthetic-data** — diverse test inputs when real data is sparse.
- **write-judge-prompt** — design **binary Pass/Fail** LLM-as-judge evaluators.
- **validate-evaluator** — calibrate judges vs human labels using **TPR/TNR and bias correction**.
- **evaluate-rag** — evaluate retrieval and generation separately.
- **build-review-interface** — generate human trace-review annotation UIs.

He stresses they only encode mistakes that generalize; skills grounded in your own stack/domain/data will outperform them ("start here, then write your own"). Footnote distinguishes product evals from MMLU/HELM-style capability benchmarks.

## Why it matters / where it cuts
The clearest bridge between Husain's evals methodology and the **agent-builds-software** moment: he's packaging error-analysis/judge-validation as **skills coding agents run**, which is exactly the "infra around the agent > the model" lesson the radar's harness-engineering thread reports. Directly relevant to [[agent-evaluation]] and [[llm-as-judge]] (binary pass/fail, TPR/TNR validation, separate RAG retrieval/generation eval). Also a concrete data point that the eval-vendor ecosystem has standardized on MCP. So what: a buildable artifact — point a coding agent at this plugin to audit a team's eval pipeline.

## Graph
- **Author:** [[hamel-husain]]
- **Concepts:** [[agent-evaluation]] · [[llm-as-judge]] · [[coding-agents]] · [[agentic-rag]]
- **Entities:** [[openai]] (harness-engineering); [[mcp]] (vendor MCP servers); evals-skills (his OSS eval toolkit) (his plugin — node requested)
- **Debate:** [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2026-03-02-husain-evals-skills.md`
