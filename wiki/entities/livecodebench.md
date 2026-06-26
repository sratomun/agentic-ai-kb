---
type: entity
entity_type: benchmark
tags: [agents, benchmark]
created: 2026-06-21
updated: 2026-06-22
census_count: 17
---

# LiveCodeBench

*A contamination-resistant, continuously-updated coding benchmark drawing from real competitive programming problems.*

## What it is
LiveCodeBench continuously sources new problems from competitive programming platforms (LeetCode, AtCoder, CodeForces), preventing training data contamination by keeping evaluation problems ahead of training cutoffs. Appears in ~17 of the 2026 H1 census papers for measuring code-agent reasoning quality.

## Why it matters
Contamination-free evaluation is rare and valuable — LiveCodeBench results are the most trustworthy signal of genuine code-reasoning ability available, not inflated by training data memorization. Relevant for selecting code-generation agents in production where reasoning under novel problems is required.

## Relationships
- evaluates [[coding-agents]]
