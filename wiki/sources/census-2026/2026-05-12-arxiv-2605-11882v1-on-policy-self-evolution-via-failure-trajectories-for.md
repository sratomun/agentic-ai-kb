---
type: source
source_type: arxiv
title: "On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment"
authors: Bo Yin, Qi Li, Xinchao Wang
url: https://arxiv.org/abs/2605.11882v1
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, self-evolving-agents, agentic-rl, agent-security, tool-use, arxiv, auto-ingested]
---

# On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment

**arXiv:** [2605.11882v1](https://arxiv.org/abs/2605.11882v1) · 2026-05-12 · cs.AI
**Authors:** Bo Yin, Qi Li, Xinchao Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-using LLM agents fail through trajectories rather than only final responses, as they may execute unsafe tool calls, follow injected instructions, comply with harmful requests, or over-refuse benign tasks despite producing a seemingly safe answer. Existing safety-alignment signals are largely response-level or off-policy, and often incur a safety-utility trade-off: improving agent safety comes at the cost of degraded task performance. Such sparse and single-objective rewards severely limit real-world usability. To bridge this gap, we propose FATE, an on-policy self-evolving framework that transforms verifier-scored failures into repair supervision without expert demonstrations. For each failure, the same policy proposes repair candidates, which are then re-scored by verifiers and filtered across security, utility, over-refusal control, and trajectory validity. This dense trajectory-level information is then used as a supervision signal for agent self-evolution. During this process, we further introduce Pareto-Front Policy Optimization (PFPO), combining supervised warmup with Pareto-aware policy optimization to preserve safety-utility trade-offs. Experiments on AgentDojo, AgentHarm, and ATBench show that FATE improves safety across different models and scales while preserving useful behavior. Compared with strong baselines, FATE reduces attack success rate by 33.5%, harmful compliance by 82.6%, and improves external trajectory-safety diagnosis by 6.5%. These results suggest that failed trajectories can provide structured repair supervision for safer self-evolving agents.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.11882v1)
