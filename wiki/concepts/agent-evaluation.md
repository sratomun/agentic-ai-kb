---
type: concept
tags: [agents, evaluation, benchmarks, reliability]
created: 2026-06-21
updated: 2026-06-22
source_count: 9
---

# Agent evaluation

*How we measure agents — and the growing evidence that the usual measurements mislead.*

## What it is
The methods, benchmarks, and metrics used to judge whether an agent actually works: behavior benchmarks (browsing, tool use, enterprise tasks), task-level functional metrics (text-to-query accuracy, RCA precision, code pass rates), and the [[llm-as-judge]] machinery underneath the soft scores. Closely tied to [[agent-reliability]] (does it work the same way twice) and [[governance-gap]] (can you trust the number).

## Why it matters
Read every agent benchmark skeptically — the headline number is usually the least trustworthy part. Two findings to keep in your pocket: leaderboard rankings **don't transfer out-of-distribution** (so rank by predictive validity, not aggregate score), and the best of 14 frontier models scores only **37.4%** on realistic enterprise tasks. That second number is the cleanest one-line rebuttal to "agents are ready for autonomous deployment."

## What the evidence shows
**2025 foundations.** The year built the benchmarks that exposed how far agents have to go. **BrowseComp** (1,266 hard multi-hop browsing questions) showed frontier models score near-zero without strong tool use (→ [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing]]); **PaperBench** asked agents to replicate 20 ICML papers and the best (Claude 3.5 Sonnet) hit only **21% vs a 41.6% human-PhD baseline** (→ [[2025-04-02-arxiv-2504-01848v3-paperbench-evaluating-ai-s-ability-to-replicate-ai]]); and the first **evaluation survey** organized the field into five perspectives (core capabilities, app-specific, generalist, benchmark dimensions, tooling → [[2025-03-20-arxiv-2503-16416v2-survey-on-evaluation-of-llm-based-agents]]). τ²-Bench added dual-control (the user acts too → [[tau2-bench]]); EmbodiedBench and WebWalker extended rigor to embodied and web traversal.

**2026 developments.** The frame turned skeptical and deployment-focused:
- Aggregate-score rankings systematically fail to transfer OOD; rank by in-sample↔out-of-sample correlation (predictive validity) instead (→ [[2026-06-18-arxiv-2606-19704v1-predictive-validity-agent-evaluation]]).
- On a realistic enterprise benchmark, the best of 14 frontier models (Claude Opus 4.5) hits only **37.4%**; strategic reasoning is the bottleneck and agents rarely refuse infeasible tasks (EnterpriseOps-Gym → [[2026-03-13-arxiv-2603-13594v1-enterpriseops-gym-stateful-agentic-planning]]).
- More orchestration is not free: a negative ablation shows expanded orchestration failed to improve GAIA L1 accuracy while increasing failures and cost (ChromaFlow → [[2026-05-13-arxiv-2605-14102v2-chromaflow-negative-ablation-orchestration]]).
- No agent paradigm dominates; a reasoning harness multiplies LLM performance 3–10× (Agentick → [[2026-05-07-arxiv-2605-06869v2-agentick-unified-sequential-decision-benchmark]]).

## Task-level evaluation (functional outputs)
Beyond agent-behavior benchmarks, recent work pins down metrics per functional task:
- **Text2query** — execution accuracy gated on intent-grounding ([[2026-01-22-arxiv-2601-15728v2-bird-python-text-to-python-vs-sql]]); cost/efficiency at scale ([[2026-02-25-arxiv-2602-21480v4-text-to-big-sql-cost-metrics]]).
- **Data analysis / RCA** — active diagnostic reasoning, root-cause precision/recall ([[2026-02-28-arxiv-2603-00468v1-cloud-opsbench-agentic-rca]]); insight accuracy + tail latency ([[2026-01-27-arxiv-2601-20048v2-insight-agents-data-insights]]).
- **Code / tool generation** — execution-grounded pass rate + coverage, deterministic evaluators ([[2026-02-18-arxiv-2602-16953v3-llm4cov-execution-aware-testbench]]).
- **Content / summarization** — faithfulness, coherence, layout, multi-turn instruction following ([[2026-02-10-arxiv-2602-13318v1-deckbench-slide-generation]]).
- **LLM-as-judge** — the substrate for all the soft metrics above; treat as a validated component → [[llm-as-judge]].

## Relationships
- verifier's rule (what's measurable gets solved): [[jason-wei]] → [[2025-07-15-blog-wei-asymmetry-of-verification]]
- cross-refs (methods/benchmarks/models): [[aime]] · [[gpqa]] · [[swe-bench]] · [[gaia-benchmark]]
- benchmarks: [[enterpriseops-gym]], [[agentick]], [[gaia-benchmark]], [[bfcl]]
- evaluates: [[multi-agent-systems]], [[tool-use]], [[agentic-ai]]
- relates to [[governance-gap]]
- cost/latency as eval axes: [[agent-finops]]
- sub-areas: [[llm-as-judge]], [[data-analysis-agents]]
- functional benchmarks: [[cloud-opsbench]], [[deckbench]], [[bird-python]], [[llm4cov]], [[tau2-bench]], [[swe-bench]]
- state-of-field synthesis: [[agent-evals-state-2026]]
- perspective voices: [[hamel-husain]] (evals-first; error analysis + validated judges → [[debate-evals-vs-frameworks]]), [[chip-huyen]] (agent failure-mode taxonomy), [[ethan-mollick]] (work-benchmarks from the user's seat)
- tooling: [[inspect-ai]]
- evaluates: [[harness-engineering]] (the "beyond final task success" problem)

## Key 2025 papers (citation-ranked)
- **441** · [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing|BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents]]
- **275** · [[2025-06-09-arxiv-2506-07982v1-2-bench-evaluating-conversational-agents-in-a-dual|$τ^2$-Bench: Evaluating Conversational Agents in a Dual-Control Environment]]
- **222** · [[2025-04-04-arxiv-2504-07981v1-screenspot-pro-gui-grounding-for-professional-high-resolution|ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use]]
- **191** · [[2025-04-02-arxiv-2504-01848v3-paperbench-evaluating-ai-s-ability-to-replicate-ai|PaperBench: Evaluating AI's Ability to Replicate AI Research]]
- **179** · [[2025-03-20-arxiv-2503-16416v2-survey-on-evaluation-of-llm-based-agents|Survey on Evaluation of LLM-based Agents]]
- **172** · [[2025-02-13-arxiv-2502-09560v3-embodiedbench-comprehensive-benchmarking-multi-modal-large-language-models|EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for...]]
- **168** · [[2025-06-13-arxiv-2506-11763v1-deepresearch-bench-a-comprehensive-benchmark-for-deep-research|DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents]]
- **146** · [[2025-01-13-arxiv-2501-07572v3-webwalker-benchmarking-llms-in-web-traversal|WebWalker: Benchmarking LLMs in Web Traversal]]
