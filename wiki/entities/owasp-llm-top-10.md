---
type: entity
entity_type: framework
aliases: [OWASP Top 10 for LLM Applications, LLM Top 10, OWASP LLM Top 10]
tags: [security, framework, standards]
created: 2026-06-23
updated: 2026-06-23
url: https://genai.owasp.org/llm-top-10/
---

# OWASP Top 10 for LLM Applications

*The practitioner checklist for LLM-app risk — prompt injection at #1, Excessive Agency as the bridge to agents.*

## What it is
OWASP's ranked list of the ten most critical LLM-application risks (2025 edition): **LLM01 Prompt Injection**, **LLM02 Sensitive Information Disclosure**, **LLM03 Supply Chain**, **LLM04 Data & Model Poisoning**, **LLM05 Improper Output Handling**, **LLM06 Excessive Agency**, **LLM07 System Prompt Leakage**, **LLM08 Vector & Embedding Weaknesses**, **LLM09 Misinformation**, **LLM10 Unbounded Consumption**. Prompt injection has held #1 across editions; the root cause it names — instructions and data sharing one channel with no trust boundary — is the through-line of the whole field.

## Why it matters
This is the baseline checklist for the *low-autonomy* end of the spectrum (raw LLM calls and single-turn tool use). **LLM06 Excessive Agency** is the explicit pivot point to agents — too much functionality, permission, or autonomy — and is where the [[owasp-agentic-top-10|agentic Top 10]] takes over. The radar's own findings slot in directly: [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection|over-privileged tool selection]] under LLM06, [[tool-description-poisoning|TDP]] under LLM03/LLM01.

## Relationships
- authored by [[owasp]]
- extended for agents by [[owasp-agentic-top-10]]
- complements [[nist-ai-rmf]], [[mitre-atlas]], [[maestro]]
- part of the [[security-standards]] layer for [[agent-security]]
- LLM01 ↔ [[debate-prompt-injection-solvable]], [[simon-willison]] (lethal trifecta)

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
