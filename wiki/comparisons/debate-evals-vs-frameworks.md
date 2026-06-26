---
type: comparison
kind: debate
tags: [debate, perspective, evaluation, agent-frameworks]
created: 2026-06-22
updated: 2026-06-22
status: open
---

# Debate: Is the binding constraint evals, or the framework?

*When an LLM/agent product doesn't work, where's the highest-ROI fix — better measurement, or better orchestration architecture? The answer decides where a team spends its scarce engineering time.*

## The question
What is the actual bottleneck on shipping a working agent product: **evaluation discipline** (error analysis + validated, domain-specific measurement) or the **agent framework / orchestration architecture** (the harness, the multi-agent topology, the tool-routing layer)? Stated so neither side is begged: given a team that's stuck, do you tell them to build evals or to rebuild their scaffold?

## Positions

### "Evals are the bottleneck"
- **Who:** [[hamel-husain]] (and Shreya Shankar) — *stake: sells the discipline — a paid evals course and an OSS evals toolkit; his thesis is also his business.*
- **Argument:** successful teams "barely talk about tools"; the highest-ROI activity is **error analysis** — reading traces, building a domain-specific failure taxonomy, then a *validated* LLM-judge (measured as a classifier with human labels, TPR/TNR, not vibes). Off-the-shelf metrics and unvalidated judges are the real failure mode, not the framework. → [[2025-03-24-blog-husain-field-guide]] · [[2026-01-15-blog-husain-evals-faq]] · [[2026-03-26-blog-husain-revenge-data-scientist]]
- **Evidence they cite:** dozens of consulting engagements where measurement, not architecture, was the unlock; the rise of agent-eval tooling like Inspect AI (→ [[2025-06-23-blog-husain-inspect-ai]]).

### "Frameworks / orchestration are load-bearing"
- **Who:** the framework ecosystems ([[langgraph]], [[autogen]], [[crewai]]) and the multi-agent/orchestration tradition; adjacent to the autonomy camp in [[debate-agents-vs-workflows]].
- **Argument:** the scaffold *is* the product — routing, memory, multi-agent decomposition and orchestration are where reliability and capability come from; pick the right architecture and the behavior follows.
- **Evidence they cite:** complex production agents built on orchestration frameworks; multi-agent decompositions of hard tasks.

## Where it stands
The radar's own **research layer leans toward the evals side.** On realistic enterprise tasks the best frontier model scores ~37%, and benchmark rankings don't transfer out-of-distribution (→ [[agent-evaluation]]) — i.e. *your own validated measurement*, not a leaderboard or a framework, predicts deployed behavior. An [[llm-as-judge]] flips guardrail results by up to 30× depending on configuration, which is exactly the "validate the judge" point. And a negative ablation (ChromaFlow) found that *more* orchestration failed to improve accuracy while raising cost and failures (→ [[agent-evaluation]]) — evidence that scaffold sophistication isn't the missing ingredient. The honest read: measurement quality is the more reliable lever today, but the two aren't mutually exclusive — you need a harness that's *instrumented* enough to evaluate.

## Relationships
- concerns [[agent-evaluation]], [[llm-as-judge]], [[agentic-ai]]
- adjacent to [[debate-agents-vs-workflows]]
- participants: [[hamel-husain]] · [[langgraph]] · [[autogen]] · [[crewai]]
