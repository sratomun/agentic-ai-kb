---
type: source
source_type: arxiv
title: "SDOF: Taming the Alignment Tax in Multi-Agent Orchestration with State-Constrained Dispatch"
authors: Zhantao Wang
url: https://arxiv.org/abs/2605.15204v1
date: 2026-04-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agent-security, agent-skills, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SDOF: Taming the Alignment Tax in Multi-Agent Orchestration with State-Constrained Dispatch

**arXiv:** [2605.15204v1](https://arxiv.org/abs/2605.15204v1) · 2026-04-20 · cs.AI
**Authors:** Zhantao Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent orchestration frameworks such as LangChain, LangGraph, and CrewAI route tasks through graph-based pipelines but do not enforce the stage constraints that govern real business processes. We present SDOF, a framework that treats multi-agent execution as a constrained state machine. SDOF operates through two primary defensive layers, implemented by three components: (1) an Online-RLHF Specialized Intent Router trained via Generative Reward Modeling (GRPO) and (2) a StateAwareDispatcher with GoalStage finite-automaton checks and precondition/postcondition SkillRegistry validation for auditable execution control. On a recruitment system backed by the Beisen iTalent platform (6000+ enterprises), 185 expert-curated scenarios trigger 1671 live API calls. Our GSPO-aligned 7B Intent Router achieves higher joint accuracy than zero-shot GPT-4o on this FSM-constrained adversarial routing benchmark (80.9% versus 48.9%). In end-to-end execution, SDOF reaches 86.5% task completion (95% confidence interval 80.8 to 90.7) and blocks all 22 operations in the injection, illegal HR subset. Under a broader message-level blocking audit, SDOF attains precision 100% and recall 88%, expert agreement kappa=0.94. A separate evaluation on 960 SGD-derived dialogues spanning 8 service domains surfaces 201 stage-order conflicts under our FSM mapping, 41 of which arise in the normal split. This arXiv version reports the current validated scope; extended multi-seed training comparisons and deeper workflow evaluations will be released in a subsequent update.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[grpo]] · [[langgraph]] · [[crewai]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15204v1)
