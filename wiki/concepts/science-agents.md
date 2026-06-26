---
type: concept
tags: [agents, science, discovery, research]
created: 2026-06-21
updated: 2026-06-22
census_count: 297
kind: domain
---

# Scientific-discovery agents

*Agents that automate research — hypothesis generation, experiment design, literature synthesis, and discovery, in closed "AI scientist" loops.*

## What it is
Agents that run parts (or all) of the research workflow: propose hypotheses, design and execute experiments, analyze results, and write them up — increasingly multi-agent, with tournament-style hypothesis evolution and, in the strongest cases, real wet-lab validation.

## Why it matters
The highest-upside frontier — agents that compound *knowledge generation* rather than just doing tasks. It's also the sharpest stress test for [[agent-reliability]] and verification: a wrong scientific claim is far costlier than a wrong summary, so this is where "show your work" and reproducibility get pushed hardest.

## What the evidence shows
**2025 foundations.** The year went from "research assistant" to "autonomous scientist with lab results." **Agent Laboratory** ran the literature→experiments→writing loop as a cheap autonomous assistant (~$2/run) with iterative self-correction (→ [[2025-01-08-arxiv-2501-04227v2-agent-laboratory-using-llm-agents-as-research-assistants]]). **AI co-scientist** added a tournament-evolution process for self-improving hypotheses that benefits from test-time compute — and, crucially, produced *validated* biology (epigenetic targets that reduced fibrogenesis in human hepatic organoids) (→ [[2025-02-26-arxiv-2502-18864v1-towards-an-ai-co-scientist]]). **AI Scientist-v2** reached workshop-level automated discovery via agentic tree search (→ [[2025-04-10-arxiv-2504-08066v1-the-ai-scientist-v2-workshop-level-automated-scientific]]), and [[coding-agents|AlphaEvolve]] proved the algorithmic-discovery case (Strassen beaten). The essential reality check: **PaperBench** — agents replicating ICML papers — where the best model scored **21% vs a 41.6% human-PhD baseline** (→ [[2025-04-02-arxiv-2504-01848v3-paperbench-evaluating-ai-s-ability-to-replicate-ai]]).
- Reads as: real generative capability, still far short of autonomous science.

## Includes (sub-themes folded here)
Folds in: **AI-scientist / autonomous-research systems** (AI Scientist, AI co-scientist, automated discovery labs — ~62 papers), hypothesis generation, and experiment automation.

## Relationships
- commentary: [[demis-hassabis]] ("root-node problems"; AlphaFold template; Co-Scientist), [[jeff-dean]]
- uses [[multi-agent-systems]], [[self-evolving-agents]], [[agentic-rag]]
- evaluated by [[mle-bench]]; reality-checked by PaperBench (see [[agent-evaluation]])
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **559** · [[2025-06-16-arxiv-2506-13131v1-alphaevolve-a-coding-agent-for-scientific-and-algorithmic|AlphaEvolve: A coding agent for scientific and algorithmic discovery]]
- **370** · [[2025-01-08-arxiv-2501-04227v2-agent-laboratory-using-llm-agents-as-research-assistants|Agent Laboratory: Using LLM Agents as Research Assistants]]
- **311** · [[2025-02-26-arxiv-2502-18864v1-towards-an-ai-co-scientist|Towards an AI co-scientist]]
- **269** · [[2025-04-10-arxiv-2504-08066v1-the-ai-scientist-v2-workshop-level-automated-scientific|The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic ...]]
- **191** · [[2025-04-02-arxiv-2504-01848v3-paperbench-evaluating-ai-s-ability-to-replicate-ai|PaperBench: Evaluating AI's Ability to Replicate AI Research]]
- **130** · [[2025-02-18-arxiv-2502-13138v1-aide-ai-driven-exploration-in-the-space-of|AIDE: AI-Driven Exploration in the Space of Code]]
