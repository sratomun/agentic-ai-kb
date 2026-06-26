---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-22
updated: 2026-06-22
---

# MCTS (Monte Carlo Tree Search)

*Monte Carlo Tree Search — search over reasoning/action trees for agent planning and test-time deliberation scaling.*

## What it is
MCTS (Monte Carlo Tree Search) is a search algorithm that builds a tree of possible actions or reasoning steps by sampling and evaluating paths, used in agent planning and test-time compute scaling to improve decision quality beyond a single forward pass.

## Why it matters
MCTS is the bridge between training-time capability and test-time performance: it lets agents spend more compute at inference to get better answers without retraining. It's a key technique for high-stakes agentic decisions where quality matters more than speed.

## Relationships
- used in [[agentic-rl]], [[multi-agent-systems]]
- relates to [[self-evolving-agents]]
