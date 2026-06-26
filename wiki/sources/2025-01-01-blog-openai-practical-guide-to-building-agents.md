---
type: source
source_type: blog
title: "A practical guide to building agents"
author: OpenAI
outlet: OpenAI business guides & resources (PDF)
url: https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf
resource: https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf
date: 2025-01-01
stake: Vendor how-to guide — OpenAI's own playbook, oriented around its Agents SDK; pattern recommendations favor OpenAI's code-first SDK over declarative graph frameworks. (PDF is undated; year inferred as 2025 — it accompanies the March 2025 Agents SDK launch. Date treated as approximate.)
ingested: 2026-06-22
tags: [perspective, agentic-ai, multi-agent-systems, tool-use, agent-security, agent-reliability]
---

# A practical guide to building agents

**Guide (PDF)** · OpenAI · ~2025 (undated) · [link](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf)

**The take (attributed):** OpenAI's framework for when and how to build an agent: an agent is a system that *controls its own workflow execution* (not just an LLM bolted into an app), you should build one only for workflows that resist traditional automation, and you should max out a single agent before reaching for multi-agent — with layered guardrails and human-in-the-loop for high-risk actions.

**Stake:** Vendor how-to. Useful and largely vendor-neutral on principles, but the orchestration patterns and code samples are oriented around OpenAI's [[agentic-ai|Agents SDK]] (`Runner.run()`, manager/decentralized handoffs) and it argues for a code-first SDK over declarative graph frameworks — a position, not a neutral fact.

## Argument
- **What is an agent:** "Agents are systems that independently accomplish tasks on your behalf." The dividing line is *workflow control*: chatbots, single-turn LLMs, and sentiment classifiers "are not agents." Two characteristics — the LLM manages execution/decisions and self-corrects, and it has [[tool-use|tools]] it *dynamically selects* within guardrails.
- **When to build:** prioritize workflows that beat traditional automation — complex decision-making (judgment/exceptions), difficult-to-maintain rulesets, and heavy reliance on unstructured data. (Don't build an agent where a deterministic rule will do.)
- **Design foundations — three components:** Model, Tools (three kinds: Data, Action, Orchestration/agents-as-tools), Instructions. Practical tip: build evals for a baseline, prototype on the most capable model, then swap down for cost/latency.
- **Orchestration:** "maximize a single agent's capabilities first." Split only on branching complexity or *tool overlap* — and the threshold is overlap, not count: ">15 well-defined, distinct tools" can work while "<10 overlapping tools" can fail. Two [[multi-agent-systems|multi-agent]] patterns: **Manager** (central agent calls specialists as tools) and **Decentralized** (peers hand off — good for triage).
- **[[agent-security|Guardrails]]:** "a layered defense mechanism" — relevance/safety classifiers (jailbreak & prompt-injection), PII filter, moderation, tool risk ratings (low/med/high), rules-based blocklists/regex, output validation. Plan [[agent-reliability|human intervention]] on failure thresholds and high-risk actions ("canceling user orders, authorizing large refunds, or making payments").

## Why it matters / where it cuts
This is the most cited "should I build an agent, and how" reference OpenAI publishes, and its definition — *agent = the LLM controls workflow execution* — is a clean line the exec can use to cut through vendor "agent-washing." The decision criteria (build agents only where rules break down) and the **single-agent-first** default are a sober counterweight to multi-agent hype, feeding the [[debate-agents-vs-workflows|agents-vs-workflows]] question. The tool-overlap-not-tool-count heuristic and the layered-guardrails + human-on-high-risk-action model are directly actionable. Caveat: the orchestration guidance is shaped to OpenAI's SDK and its anti-graph-framework stance is a position in the [[debate-evals-vs-frameworks|frameworks debate]], not settled fact.

## Graph
- **Author:** [[openai]]
- **Concepts:** [[agentic-ai]] · [[multi-agent-systems]] · [[tool-use]] · [[agent-security]] · [[agent-reliability]]
- **Entities:** [[openai]]
- **Debate:** [[debate-agents-vs-workflows]] · [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2025-01-01-openai-practical-guide-to-building-agents.md`
