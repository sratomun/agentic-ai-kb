---
type: source
source_type: arxiv
title: "AgentTrust: Runtime Safety Evaluation and Interception for AI Agent Tool Use"
authors: Chenglin Yang
url: https://arxiv.org/abs/2605.04785v1
date: 2026-05-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [data-query-agents, agent-security, agent-protocols, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# AgentTrust: Runtime Safety Evaluation and Interception for AI Agent Tool Use

**arXiv:** [2605.04785v1](https://arxiv.org/abs/2605.04785v1) · 2026-05-06 · cs.AI
**Authors:** Chenglin Yang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern AI agents execute real-world side effects through tool calls such as file operations, shell commands, HTTP requests, and database queries. A single unsafe action, including accidental deletion, credential exposure, or data exfiltration, can cause irreversible harm. Existing defenses are incomplete: post-hoc benchmarks measure behavior after execution, static guardrails miss obfuscation and multi-step context, and infrastructure sandboxes constrain where code runs without understanding what an action means. We present AgentTrust, a runtime safety layer that intercepts agent tool calls before execution and returns a structured verdict: allow, warn, block, or review. AgentTrust combines a shell deobfuscation normalizer, SafeFix suggestions for safer alternatives, RiskChain detection for multi-step attack chains, and a cache-aware LLM-as-Judge for ambiguous inputs. We release a 300-scenario benchmark across six risk categories and an additional 630 independently constructed real-world adversarial scenarios. On the internal benchmark, the production-only ruleset achieves 95.0% verdict accuracy and 73.7% risk-level accuracy at low-millisecond end-to-end latency. On the 630-scenario benchmark, evaluated under a patched ruleset and not claimed as zero-shot, AgentTrust achieves 96.7% verdict accuracy, including about 93% on shell-obfuscated payloads. AgentTrust is released under the AGPL-3.0 license and provides a Model Context Protocol server for MCP-compatible agents.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.04785v1)
