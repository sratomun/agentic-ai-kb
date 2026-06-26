---
type: entity
entity_type: framework
aliases: [OWASP Top 10 for Agentic Applications, Agentic Top 10, ASI Top 10, Agentic AI Threats and Mitigations]
tags: [security, framework, standards, agents]
created: 2026-06-23
updated: 2026-06-23
url: https://genai.owasp.org/
---

# OWASP Top 10 for Agentic Applications

*The agent-native risk checklist — goal hijack, tool misuse, memory poisoning, rogue agents — for systems that act, use tools, and talk to each other.*

## What it is
OWASP's agentic security work has two layers. The **Agentic AI – Threats and Mitigations** taxonomy (Feb 2025) enumerates 15 threats (**T1 Memory Poisoning, T2 Tool Misuse, T3 Privilege Compromise, T4 Resource Overload, T5 Cascading Hallucination, T6 Intent Breaking & Goal Manipulation, T7 Misaligned & Deceptive Behaviors, … T10 Overwhelming Human-in-the-Loop, T11 Unexpected RCE, T12 Agent Communication Poisoning, T13 Rogue Agents**, and more). The ranked **Top 10 for Agentic Applications** (ASI01–ASI10, Dec 2025) distills it: **ASI01 Agent Goal Hijack, ASI02 Tool Misuse & Exploitation, ASI03 Identity & Privilege Abuse, ASI04 Agentic Supply Chain, ASI05 Unexpected Code Execution (RCE), ASI06 Memory & Context Poisoning, ASI07 Insecure Inter-Agent Communication, ASI08 Cascading Failures, ASI09 Human-Agent Trust Exploitation, ASI10 Rogue Agents**.

## Why it matters
This is the checklist for the *high-autonomy* end of the spectrum — risks that only exist once an agent has tools, memory, loops, and peers. It's the connective tissue across the radar's security corpus: [[2026-01-08-arxiv-2601-04566v2-backdooragent-unified-backdoor-attacks|stage-aware backdoors]] and [[2025-12-18-arxiv-2512-16962v1-memorygraft-persistent-compromise-of-llm-agents-via-poisoned|MemoryGraft]] → ASI06/T1; [[tool-description-poisoning|TDP]] → ASI02/ASI04; [[2026-01-16-arxiv-2601-10955v2-stealthy-resource-amplification-tool-chains|economic DoS]] → T4; [[2025-10-05-arxiv-2510-05179v2-agentic-misalignment-how-llms-could-be-insider-threats|agentic misalignment]] → ASI10/T7. AWS and Microsoft now embed the taxonomy in their own guidance.

## Relationships
- authored by [[owasp]]
- extends [[owasp-llm-top-10]] (LLM06 Excessive Agency → the agentic list)
- complements [[nist-ai-rmf]], [[mitre-atlas]], [[maestro]]
- part of the [[security-standards]] layer for [[agent-security]], [[multi-agent-systems]]
- maps to radar attack classes: [[tool-description-poisoning]], memory poisoning, rogue agents, economic DoS

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
