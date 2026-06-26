# A practical guide to building agents

Source: https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf
Author: OpenAI
Date: undated (no publication date in the PDF body; filed under 2025-01-01 as a placeholder — the guide accompanies the March 2025 Agents SDK / Responses API launch and is oriented around the Agents SDK; treat the year as 2025)
Category: OpenAI business guide / resource (33 pages)
Captured: 2026-06-22
Vendor stake: OpenAI's own guidance, distilled from its customer deployments and oriented around its Agents SDK; pattern recommendations favor OpenAI's code-first SDK over declarative graph frameworks.

---

The guide targets product/engineering teams building their first agents. Four sections: What is an agent? (p4); When should you build an agent? (p5); Agent design foundations (p7); Guardrails (p24); plus a conclusion.

## What is an agent?
"Agents are systems that independently accomplish tasks on your behalf." Distinguished from LLM-integrated apps that don't control workflow execution: "Applications that integrate LLMs but don't use them to control workflow execution—think simple chatbots, single-turn LLMs, or sentiment classifiers—are not agents." Two core characteristics: (1) it leverages an LLM to manage workflow execution and make decisions, recognizing completion and self-correcting; (2) it has access to tools to interact with external systems and "dynamically selects the appropriate tools depending on the workflow's current state, always operating within clearly defined guardrails."

## When should you build an agent?
Prioritize workflows that resist traditional automation:
- Complex decision-making (nuanced judgment/exceptions, e.g. refund approval)
- Difficult-to-maintain rules (unwieldy rulesets, e.g. vendor security reviews)
- Heavy reliance on unstructured data (natural-language interpretation, e.g. insurance claims)
Uses the payment-fraud "seasoned investigator vs. checklist" analogy.

## Agent design foundations — three components
- **01 Model** — the LLM powering reasoning/decisions.
- **02 Tools** — external functions/APIs. Three types: Data, Action, and Orchestration (agents-as-tools).
- **03 Instructions** — explicit guidelines and guardrails.
Model selection: set up evals for a baseline, prototype with the most capable model, then swap in smaller models for cost/latency. Instructions best practices: use existing documents, prompt agents to break down tasks, define clear actions, capture edge cases.

## Orchestration
- **Single-agent systems:** one model in a loop (via `Runner.run()` exit conditions); manage complexity with prompt templates. "Our general recommendation is to maximize a single agent's capabilities first."
- Split into multiple agents on complex logic (many if-then-else branches) or tool overload (similarity/overlap, not raw count): "Some implementations successfully manage more than 15 well-defined, distinct tools while others struggle with fewer than 10 overlapping tools."
- **Multi-agent patterns:**
  - **Manager (agents as tools):** "A central 'manager' agent coordinates multiple specialized agents via tool calls, each handling a specific task or domain." Edges are tool calls; ideal when one agent controls execution and user access.
  - **Decentralized (agents handing off to agents):** "Multiple agents operate as peers, handing off tasks to one another based on their specializations." Edges are handoffs; ideal for triage.
- Contrasts declarative graph frameworks vs. the Agents SDK's code-first approach.

## Guardrails
"Think of guardrails as a layered defense mechanism. While a single one is unlikely to provide sufficient protection, using multiple, specialized guardrails together creates more resilient agents." Types: Relevance classifier; Safety classifier (jailbreak/prompt-injection detection); PII filter; Moderation; Tool safeguards (low/medium/high risk ratings); Rules-based protections (blocklists, length limits, regex); Output validation. Build heuristic: focus on data privacy/content safety first; add guardrails from real-world failures; optimize for security + UX. Plan for human intervention triggered by exceeding failure thresholds and high-risk actions: "High-risk actions... should trigger human oversight... Examples include canceling user orders, authorizing large refunds, or making payments."

## Conclusion
"Start with strong foundations: pair capable models with well-defined tools and clear, structured instructions."

Tags: guide · agents · 2025
