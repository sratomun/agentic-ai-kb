---
type: source
source_type: arxiv
title: "FORGE: Self-Evolving Agent Memory With No Weight Updates via Population Broadcast"
authors: Igor Bogdanov, Chung-Horng Lung, Thomas Kunz, Jie Gao et al.
url: https://arxiv.org/abs/2605.16233v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, self-evolving-agents, agentic-rl, agent-security, agent-protocols, arxiv, auto-ingested]
---

# FORGE: Self-Evolving Agent Memory With No Weight Updates via Population Broadcast

**arXiv:** [2605.16233v1](https://arxiv.org/abs/2605.16233v1) · 2026-05-15 · cs.AI
**Authors:** Igor Bogdanov, Chung-Horng Lung, Thomas Kunz, Jie Gao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Can LLM agents improve decision-making through self-generated memory without gradient updates? We propose FORGE (Failure-Optimized Reflective Graduation and Evolution), a staged, population-based protocol that evolves prompt-injected natural-language memory for hierarchical ReAct agents. FORGE wraps a Reflexion-style inner loop, where a dedicated reflection agent (using the same underlying LLM, no distillation from a stronger model) converts failed trajectories into reusable knowledge artifacts: textual heuristics (Rules), few-shot demonstrations (Examples), or both (Mixed), with an outer loop that propagates the best-performing instance's memory to the population between stages and freezes converged instances via a graduation criterion. We evaluate on CybORG CAGE-2, a stochastic network-defense POMDP at a 30-step horizon against the B-line attacker, where all four tested LLM families (Gemini-2.5-Flash-Lite, Grok-4-Fast, Llama-4-Maverick, Qwen3-235B) exhibit strongly negative, heavy-tailed zero-shot rewards. Compared against both a zero-shot baseline and a Reflexion baseline (isolated single-stream learning), FORGE improves average evaluation return by 1.7-7.7$\times$ over zero-shot and by 29-72% over Reflexion in all 12 model-representation conditions, reducing major-failure rates (below $-100$) to as low as $\sim$1%. We find that (1) population broadcast is critical mechanism, with a no-graduation ablation confirming that broadcast carries the performance gains while graduation primarily saves compute; (2) Examples achieves the strongest returns for three of four models, Rules offers the best cost-reliability profile with $\sim$40% fewer tokens; and (3) weaker baseline models benefit disproportionately, suggesting FORGE may mitigate capability gaps rather than amplify strong models. All evidence is confined to CAGE-2 B-line; cross-family findings are directional evidence.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[qwen]] · [[gemini]] · [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16233v1)
