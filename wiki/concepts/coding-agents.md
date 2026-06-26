---
type: concept
tags: [agents, coding, software-engineering]
created: 2026-06-21
updated: 2026-06-22
census_count: 612
kind: domain
---

# Coding & software-engineering agents

*Agents that write, repair, and maintain software — resolving issues, editing repositories, running tests in a loop. The most commercially mature agent vertical.*

## What it is
Agents that operate over real codebases: localize bugs, generate patches, run tests, and iterate, with the model wrapped in a "scaffold" (control loop, tools, context strategy). Evaluated rigorously on real GitHub issues ([[swe-bench]]) and contamination-resistant coding benchmarks ([[livecodebench]]).

## Why it matters
This is where agents *already* create measurable value and where evaluation is most honest (resolve-or-not on real issues). It's both a proof-point — agentic value is real, not hypothetical — and a leading indicator: the scaffolding patterns and RL recipes proven here migrate to harder, less-verifiable verticals.

## What the evidence shows
**2025 foundations.** Three results define the year. **AlphaEvolve** (DeepMind) showed a coding agent can *discover*, not just apply — its LLM-driven evolutionary loop produced the **first improvement over Strassen's matrix-multiplication algorithm in 56 years** (→ [[2025-06-16-arxiv-2506-13131v1-alphaevolve-a-coding-agent-for-scientific-and-algorithmic]]). **SWE-smith** attacked the data bottleneck — scaling SE training data to train SWE-agent-LM-32B to **40.2% Pass@1 on SWE-bench Verified, SOTA among open models** (→ [[2025-04-30-arxiv-2504-21798v2-swe-smith-scaling-data-for-software-engineering-agents]]). **AIDE** reframed ML-engineering as tree search over code, trading compute for performance to hit SOTA on MLE-bench / RE-Bench / Kaggle (→ [[2025-02-18-arxiv-2502-13138v1-aide-ai-driven-exploration-in-the-space-of]]).
- The connective themes: coding agents are where [[agentic-rl]] reward design and [[self-evolving-agents]] loops get their cleanest verifiable signal. Their *architecture* (the scaffold) is mapped in the [[2026-04-03-arxiv-2604-03515v2-survey-coding-agent-architecture-taxonomy|coding-agent architecture survey]].

## Relationships
- frontier coding agents: OpenAI Codex → [[2025-05-16-blog-openai-introducing-codex]]; Anthropic long-running harness → [[2025-11-26-blog-anthropic-effective-harnesses-long-running-agents]]
- benchmarks: [[swe-bench]], [[livecodebench]], [[mle-bench]]
- exemplars: [[alphaevolve]], [[devin]]
- relates to [[tool-use]], [[agentic-rl]], [[self-evolving-agents]]
- a form of [[agentic-ai]]
- perspective voices: [[ethan-mollick]] (coding agents as general-purpose tools → [[agent-adoption]]), [[simon-willison]] (agentic coding loops, vibe engineering), [[sebastian-raschka]] (harness anatomy)
- the scaffold: [[harness-engineering]]; the un-reviewed end: [[vibe-coding]]

## Key 2025 papers (citation-ranked)
- **559** · [[2025-06-16-arxiv-2506-13131v1-alphaevolve-a-coding-agent-for-scientific-and-algorithmic|AlphaEvolve: A coding agent for scientific and algorithmic discovery]]
- **170** · [[2025-04-30-arxiv-2504-21798v2-swe-smith-scaling-data-for-software-engineering-agents|SWE-smith: Scaling Data for Software Engineering Agents]]
- **130** · [[2025-02-18-arxiv-2502-13138v1-aide-ai-driven-exploration-in-the-space-of|AIDE: AI-Driven Exploration in the Space of Code]]
