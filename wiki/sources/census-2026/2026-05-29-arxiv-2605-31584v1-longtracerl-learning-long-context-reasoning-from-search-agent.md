---
type: source
source_type: arxiv
title: "LongTraceRL: Learning Long-Context Reasoning from Search Agent Trajectories with Rubric Rewards"
authors: Nianyi Lin, Jiajie Zhang, Lei Hou, Juanzi Li
url: https://arxiv.org/abs/2605.31584v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# LongTraceRL: Learning Long-Context Reasoning from Search Agent Trajectories with Rubric Rewards

**arXiv:** [2605.31584v1](https://arxiv.org/abs/2605.31584v1) · 2026-05-29 · cs.CL
**Authors:** Nianyi Lin, Jiajie Zhang, Lei Hou, Juanzi Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-context reasoning remains a central challenge for large language models, which often fail to locate and integrate key information in extensive distracting content. Reinforcement learning with verifiable rewards (RLVR) has shown promise for this task, yet existing methods are limited by low-confusability distractors and sparse, outcome-only reward signals that cannot supervise intermediate reasoning steps. To address these issues, we introduce \textsc{LongTraceRL}. For data construction, we generate multi-hop questions via knowledge graph random walks and leverage search agent trajectories to build \emph{tiered distractors}: documents the agent read but did not cite (high confusability) and documents that appeared in search results but were never opened (low confusability), producing training contexts that are far more challenging than those built by random sampling or one-shot search. For reward design, we propose a \emph{rubric reward} that uses the gold entities along each reasoning chain as fine-grained, entity-level process supervision. This rubric reward is applied only to responses with correct final answers (positive-only strategy), distinguishing the reasoning quality among correct responses and preventing reward hacking. Experiments on three reasoning LLMs (4B--30B) across five long-context benchmarks demonstrate that \textsc{LongTraceRL} consistently outperforms strong baselines and encourages comprehensive, evidence-grounded reasoning. Codes, datasets and models are available at \href{https://github.com/THU-KEG/LongTraceRL}{https://github.com/THU-KEG/LongTraceRL}.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.31584v1)
