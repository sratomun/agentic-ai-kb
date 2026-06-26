---
type: concept
tags: [agents, intent-understanding, nlu, clarification, human-agent-interaction]
created: 2026-06-23
updated: 2026-06-23
kind: hub
---

# Intent understanding

*Turning what a user said into what they want — detection, clarification, disambiguation, and rewriting — before an agent acts on it.*

## What it is
The layer that resolves a user utterance into an actionable goal. It spans the classic NLU task (map an utterance to an intent label, fill slots, flag out-of-scope) and its agentic successors: **clarifying** underspecified requests, **disambiguating** queries with multiple valid readings, and **rewriting** messy multi-turn dialogue into one explicit goal. It borders [[intent-routing]] (what you do once intent is known), [[tool-use]] (intent → structured call), and [[human-agent-interaction]] (when to ask the human).

## Why it matters
This is where most agent failures are actually born — a wrong tool call usually traces back to a misread intent, not a bad executor. The decision that matters isn't "which classifier" but **where intent lives**: a cheap fixed-label component, a flexible-but-slow agent capability, or a routing signal. The pragmatic 2026 default braids all three — **a small embedding/sentence-transformer classifier for the common case, an LLM only for the uncertain tail.** [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms|Intent Detection in the Age of LLMs]] is the load-bearing number: that hybrid **closes the accuracy gap to ~2% while cutting latency ~50%** vs. an LLM-everywhere setup.

## What the evidence shows
**Foundations — the component view, and its limits.** Classic intent detection maps utterances to a fixed taxonomy (benchmarks [[clinc150]], [[banking77]], [[multiwoz]]) and remains the cheap, controllable default — but it is brittle on new intents and open-ended dialogue. The hybrid escape hatch is the anchor result: SetFit handles the bulk, Monte-Carlo-Dropout **uncertainty routes** the hard tail to an LLM, **~2% gap for ~50% latency**, plus a two-step out-of-scope method (+>5%) ([[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms|Intent Detection in the Age of LLMs]]). At scale the classifier survives by becoming **retrieval-grounded** — REIC retrieves candidate (query,intent) pairs and lets a fine-tuned Mistral-7B score only those via constrained decoding, so new intents are an index update not a retrain (**F1 0.572 > RoBERTa 0.516**; **+3.38pp** in production) ([[2025-05-30-arxiv-2506-00210-reic-rag-enhanced-intent-classification-at-scale|REIC]]). On-device neuro-symbolic variants push the same trade: a 3B Llama + intent ontology reaches **85% vs GPT-4's 90%** at a fraction of the footprint ([[2025-11-24-arxiv-2511-19780v1-noem3a-neuro-symbolic-multi-intent-understanding|NOEM³A]]).

**Recent developments — intent becomes a behavior, not a label.** Three threads pull intent out of the classifier:
- **Clarification (knowing *when* to ask).** Assistants barge ahead because single-turn RLHF undervalues clarifying questions; rewarding the *future* turn fixes it (**+4-5% F1**, [[2024-10-17-arxiv-2410-13788-modeling-future-conversation-turns-clarifying-questions|Modeling Future Conversation Turns]]). The newer work makes "when to ask" principled: EVPI over tool parameters ([[2025-11-11-arxiv-2511-08798v2-structured-uncertainty-guided-clarification|Structured Uncertainty]], When2Call 36.5%→65.2%), Bayesian information-gain rewards ([[2026-06-02-arxiv-2606-03135v1-uncertainty-aware-clarification-information-gain|Information Gain]]), and uncertainty-aware scaffolds for coding agents (**69.4%** on underspecified SWE-bench, [[2026-03-27-arxiv-2603-26233v2-ask-or-assume-clarification-coding-agents|Ask or Assume?]]). Benchmarks confirm a systematic **under-clarification bias** that worsens with dialogue depth ([[2025-12-24-arxiv-2512-21120v1-clarifymt-bench-multi-turn-clarification|ClarifyMT-Bench]]).
- **Disambiguation (multiple valid readings).** Rather than winner-takes-all, emit an ordered multi-intent set and resolve with policy — DoorDash grounds an LLM in catalog retrieval + live web search to hit **90.7% (+13pp)** on context-sparse queries, in production over 95% of impressions ([[2026-03-02-arxiv-2603-01486v2-agentic-multi-source-grounding-doordash|DoorDash]]).
- **Rewriting (moving intent).** Don't classify the dialogue — rewrite it into an explicit goal, biggest wins exactly on **shifted-intent and multi-intent** ([[2025-08-29-arxiv-2509-04472-recap-rewriting-conversations-intent-understanding|RECAP]]). Proactive variants clarify latent intent *before* expensive long-horizon work ([[2026-02-03-arxiv-2602-03468v1-intentrl-proactive-user-intent-agents|IntentRL]]), and 14M+ real search logs show intent is recoverable from trajectory dynamics ([[2026-01-24-arxiv-2601-17617v3-agentic-search-in-the-wild-intents|Agentic Search in the Wild]]).

**Caveat.** Our local arXiv census is agents-centric, so the classic NLU line ([[clinc150]]/[[banking77]] detection, slot filling) is under-sampled there and was recovered via extended search — treat the component-view coverage as curated, not exhaustive.

## Includes (sub-themes folded here)
Folds in: **clarification / when-to-ask** (~6 papers), **disambiguation of ambiguous queries** (DoorDash, multi-intent), **intent rewriting / query reformulation** (RECAP, conversational query rewriting), and **out-of-scope / open-intent detection**. The systems side — routing on intent — lives in its own hub, [[intent-routing]].

## Relationships
- precedes / feeds [[intent-routing]] (resolve intent → route on it)
- resolved against structure by [[intent-grounding]] (knowledge graph / semantic layer)
- capability of [[agentic-ai]]
- borders [[tool-use]] (intent → structured tool call) and [[human-agent-interaction]] (when to ask the human)
- efficiency lever shared with [[distillation]] (small classifier, LLM fallback)
- evaluated under [[agent-evaluation]]; clarification benchmarks ClarifyBench / ClarifyMT-Bench / When2Call
- benchmarks: [[clinc150]] · [[banking77]] · [[multiwoz]]
- methods/systems: [[setfit]] · [[arch-router]]
- the cheap classifier tier is typically [[small-language-models]]

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. Citations from census/source-note frontmatter. -->
- **17** · 2.3/mo · [[2025-11-11-arxiv-2511-08798v2-structured-uncertainty-guided-clarification|Structured Uncertainty guided Clarification for LLM Agents]]
- **5** · 0.8/mo · [[2025-12-24-arxiv-2512-21120v1-clarifymt-bench-multi-turn-clarification|ClarifyMT-Bench: Benchmarking and Improving Multi-Turn Clarificati…]]
- **2** · 0.2/mo · [[2025-05-29-arxiv-2505-23006v1-production-conversational-agents-workflow-graphs|A Practical Approach for Building Production-Grade Conversational …]]
- **0** · [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL: An Agentic LLM System for Governed Enterprise …]]
- **0** · [[2024-10-02-arxiv-2410-01627-intent-detection-in-the-age-of-llms|Intent Detection in the Age of LLMs]]
- **0** · [[2025-06-19-arxiv-2506-16655-arch-router-aligning-llm-routing-with-human-preferences|Arch-Router: Aligning LLM Routing with Human Preferences]]
- **0** · [[2024-10-17-arxiv-2410-13788-modeling-future-conversation-turns-clarifying-questions|Modeling Future Conversation Turns to Teach LLMs to Ask Clarifying…]]
- **0** · [[2025-05-30-arxiv-2506-00210-reic-rag-enhanced-intent-classification-at-scale|REIC: RAG-Enhanced Intent Classification at Scale]]
- **0** · [[2025-08-29-arxiv-2509-04472-recap-rewriting-conversations-intent-understanding|RECAP: REwriting Conversations for Intent Understanding in Agentic…]]
