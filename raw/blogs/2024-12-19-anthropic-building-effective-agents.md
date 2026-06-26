# RAW — Building effective agents (Anthropic)
Source: https://www.anthropic.com/engineering/building-effective-agents · 2024-12-19 · Erik Schluntz & Barry Zhang · captured 2026-06-22 · channel: blog (lab eng)
- "The most successful implementations use simple, composable patterns rather than complex frameworks."
- Distinction: WORKFLOWS = LLMs/tools orchestrated through predefined code paths; AGENTS = LLMs dynamically direct their own process + tool use.
- "Find the simplest solution possible, and only increase complexity when needed. This might mean not building agentic systems at all." Often a single augmented LLM call suffices.
- Workflow patterns: prompt chaining, routing, parallelization (sectioning/voting), orchestrator-workers, evaluator-optimizer. Agents = LLM using tools in a loop on environmental feedback; higher cost + compounding-error risk; sandbox + guardrails.
- Three principles: simplicity, transparency (show planning), well-crafted agent-computer interface (ACI). Frameworks add abstraction that obscures prompts; start from raw APIs.
Stake: Anthropic (sells Claude + Agent SDK) — but the post argues AGAINST over-engineering/frameworks, a nuanced "against-interest" stance.
