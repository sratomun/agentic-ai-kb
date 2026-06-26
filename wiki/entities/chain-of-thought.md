---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-22
updated: 2026-06-22
---

# Chain-of-Thought (CoT)

*Eliciting intermediate reasoning steps before an answer — the foundational technique beneath agentic planning and reasoning models.*

## What it is
Chain-of-Thought (CoT) prompting elicits step-by-step reasoning from LLMs before producing a final answer. It substantially improves performance on multi-step tasks and is the substrate for long-reasoning, agentic planning, and tool-use orchestration.

## Why it matters
CoT is the mechanism behind most reasoning-model gains and the observable 'thinking' in agent traces. Understanding its limits — faithfulness, reward hacking, over-thinking — is essential for building reliable agent evaluation pipelines.

## Relationships
- faithfulness/monitoring discussed by [[lilian-weng]], [[neel-nanda]]
- coined/discussed by [[jason-wei]]
- substrate for [[agentic-ai]], [[agentic-rl]]
- precursor to [[tool-use]] reasoning
