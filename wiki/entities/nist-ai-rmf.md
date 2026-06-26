---
type: entity
entity_type: framework
aliases: [NIST AI RMF, AI RMF, NIST AI 100-1, NIST AI 600-1, Generative AI Profile]
tags: [security, governance, framework, standards]
created: 2026-06-23
updated: 2026-06-23
url: https://www.nist.gov/itl/ai-risk-management-framework
---

# NIST AI RMF

*The voluntary risk-management spine for AI — four functions (Govern, Map, Measure, Manage) plus a Generative AI Profile that names the risks to manage.*

## What it is
NIST's AI Risk Management Framework (**AI 100-1**) organizes AI risk into four continuous functions — **Govern** (accountability, ownership, risk appetite), **Map** (context: where AI is used, who's affected, what could go wrong), **Measure** (assess, test, monitor), and **Manage** (prioritize and apply safeguards). The **Generative AI Profile (AI 600-1**, Jul 2024) layers on twelve GenAI-specific risk categories — including Confabulation, Information Integrity, Information Security, Data Privacy, Human-AI Configuration, Value Chain & Component Integration, and CBRN information — and maps suggested actions to each function. A NIST AI RMF **Agentic Profile** is in development (CSA-led).

## Why it matters
It's the framework that makes an agent-security program *governable*: it answers "who owns this risk and how do we show we're managing it," which is what boards, auditors, and regulators want. It deliberately does NOT enumerate attacks — pair it with [[owasp-llm-top-10]]/[[owasp-agentic-top-10]] (what to look for), [[mitre-atlas]] (how attacks happen), and [[maestro]] (where in the system). The GenAI Profile's "Human-AI Configuration" and "Value Chain" categories are the hooks where autonomous-agent and supply-chain risk attach.

## Relationships
- authored by [[nist]]
- complements [[owasp-llm-top-10]], [[owasp-agentic-top-10]], [[mitre-atlas]], [[maestro]]
- part of the [[security-standards]] layer for [[agent-security]]
- governs risk behind the [[governance-gap]]; informs [[frontier-model-governance]]

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
