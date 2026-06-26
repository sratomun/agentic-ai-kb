---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "RECAP: REwriting Conversations for Intent Understanding in Agentic Planning"
authors: Kushan Mitra, Dan Zhang, Hannah Kim, Estevam Hruschka (Megagon Labs)
url: https://arxiv.org/abs/2509.04472
date: 2025-08-29
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-understanding, human-agent-interaction, agent-evaluation]
---

# RECAP: REwriting Conversations for Intent Understanding in Agentic Planning

**arXiv [2509.04472](https://arxiv.org/abs/2509.04472)** · 2025-08-29 · Megagon Labs

**Significance.** The cleanest statement of the shift *away* from fixed-taxonomy intent classification: don't classify the dialogue, **rewrite** it into an explicit goal. A planner-agnostic module + benchmark. Anchors the rewriting thread in [[intent-understanding]].

## Abstract
Traditional intent classification (predefined schemas/slots) is brittle in open-ended dialogue with ambiguity, underspecification, intent drift, and multi-intent. RECAP proposes **intent rewriting** as a planner-agnostic module that turns raw USER-AGENT dialogue into a concise explicit-intent representation, plus an 810-instance benchmark and an LLM-as-judge evaluator.

## From the paper (full-text)
**Contribution / method.** A Rewriter sits before the Planner: it distills accumulated dialogue into one explicit-intent string; the (static, temperature-0 GPT-4o) Planner turns that into a task-plan DAG. The 810-conversation benchmark is synthetically generated (GPT-4o + LLaMA-3.3-70B) and human-vetted, spanning five challenges — **shifted intent, noisy input, underspecified intent, multi-intent, perfect intent**. Rewriters compared: Dummy (verbatim), Basic (generic summary), **Advanced** (intent-aware prompt), **DPO:human** and **DPO:LLM** (fine-tuned on preferences over the *plans* each rewrite produced).
**Results.** Plan quality is highly sensitive to intent representation, and divergence grows with conversation length (GED up to 6.44 between Basic vs Advanced plans). The Advanced rewriter won most categories, biggest margins on **shifted-intent (50.0%)** and **multi-intent (40.48%)** win rates; it slipped on underspecified intent (misreading refinements as "fake intent shifts"). **DPO:human** was best overall (48.88% win vs Advanced; shifted-intent 55.56%); DPO:LLM trailed (LLM pseudo-labels < human signal). Fine-tuned GPT-4.1 judge hit 65% preference accuracy.
**Takeaway.** Rewrite-then-plan beats classify-then-plan when intent is moving. The hard cases are exactly the realistic ones: drift and multi-intent.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[human-agent-interaction]] · [[agent-evaluation]]
- **Entities:** [[megagon-labs]] · [[dpo]]
- **Raw:** abstract + full-text report (alphaXiv) read 2026-06-23
