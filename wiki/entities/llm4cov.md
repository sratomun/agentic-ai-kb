---
type: entity
entity_type: method
tags: [agents, method, code-generation, evaluation, coverage]
created: 2026-06-22
updated: 2026-06-22
---

# LLM4Cov

*An execution-aware agentic learning framework for high-coverage hardware testbench generation — a 4B model beating its 30B teacher.*

## What it is
LLM4Cov is an offline, execution-aware agentic framework (Zhang et al., ICML 2026) for automated testbench generation in hardware verification. It uses deterministic simulator feedback and worst-state-prioritized SFT, achieving 69.2% pass rate / 90.4% coverage with a 4B model.

## Why it matters
LLM4Cov demonstrates that execution-grounded RL/SFT — training on verified outcomes rather than human labels — can produce small models that outperform much larger ones. The pattern transfers directly to any domain with deterministic correctness signals (testing, formal verification, code execution).

## Relationships
- evaluates [[coding-agents]]
- part of [[agent-evaluation]]

## Cited by
- [[2026-02-18-arxiv-2602-16953v3-llm4cov-execution-aware-testbench]]
