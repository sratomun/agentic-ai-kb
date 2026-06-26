---
type: source
source_type: arxiv
title: "LLM4Cov: Execution-Aware Agentic Learning for High-coverage Testbench Generation"
authors: Hejia Zhang, Zhongming Yu, Chia-Tung Ho, Haoxing Ren, Brucek Khailany, Jishen Zhao (UCSD / NVIDIA)
url: https://arxiv.org/abs/2602.16953v3
date: 2026-02-18
ingested: 2026-06-22
depth: full-text
venue: ICML 2026
tags: [agent-evaluation, coding-agents, arxiv]
---

# LLM4Cov: Execution-Aware Agentic Learning for High-coverage Testbench Generation

**Why it matters:** A clean exemplar of **execution-grounded** eval for code/test generation — judge generated code by deterministic execution signals (does it compile, does it run, what coverage does it hit), not by reference similarity. The pattern that should govern any code-gen or tool-gen agent eval.

## What it is
An offline agent-learning framework that models hardware verification as **single-step state transitions** evaluated by a deterministic simulator (the evaluator). Techniques: execution-validated data curation, worst-state-prioritized sampling, and staged (verification-conditioned) progressive SFT. Final model is a 4B (Qwen3-4B) fine-tuned from a Qwen3-Coder-30B teacher.

## Metrics (execution-grounded)
- **Pass Rate** — % of repositories where achieved coverage exceeds a human-expert threshold (primary metric).
- **Avg Coverage** — mean coverage across repos (0% when simulation fails).
- **Syn Pass** — % repos where the testbench has correct syntax, compiles, and completes simulation.
- Agentic eval = up to N=3 refine rounds with simulator feedback; Direct Inference = single pass; reported Pass@1 (n=5).

## Findings (verified)
- 4B LLM4Cov (Stage 2): **CVDP-ECov 69.2% pass / 90.4% avg coverage**; **AutoEval-ECov 85.0% pass / 96.3% avg coverage** — beating its 30B teacher by 5.3 / 10.5 pts and matching 50–100× larger models.
- Memoryless single-step state ≥ full-history "vanilla" agent (e.g. 63.9% vs 59.5% Pass@1 on a 30B coder).
- **Most baseline LLMs fail to even compile** (Syn Pass <70%); execution-validated curation lifts Syn Pass past 85% across model families — execution filtering is the dominant lever.
- Coverage gains saturate after 2–3 agentic rounds.

## So what
For code generation and tool generation, the metric that matters is functional correctness under execution (compiles, runs, coverage/tests pass) via deterministic evaluators — not LLM judges or text-match. Reinforces the report's "deterministic checks before the LLM."

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[coding-agents|Coding agents]]
- **Entities:** [[llm4cov]]
- **Raw:** alphaXiv full-text (id 2602.16953v3)

## Relationships
- introduced by [[llm4cov]]
- evaluates [[coding-agents]]
- part of [[agent-evaluation]]
