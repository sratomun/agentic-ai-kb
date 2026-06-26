---
type: comparison
kind: debate
tags: [debate, perspective, agent-security]
created: 2026-06-22
updated: 2026-06-22
status: converging
---

# Debate: Is prompt injection solvable?

*Can agent systems be made safe against prompt injection — or is it a permanent structural risk you can only avoid?*

## The question
Is prompt injection a problem you can *solve* (architecturally make injection harmless), or only *manage* (reduce likelihood, avoid the dangerous combinations)? And solvable for whom — app developers, or end users mixing their own tools?

## Positions

### "Structurally unsolved — avoid the trifecta"
- **Who:** [[simon-willison]] — *stake: independent; coined the term.*
- **Argument:** LLMs "follow instructions in content" and can't reliably tell whose instructions to trust; the **lethal trifecta** (private data + untrusted content + external comms) makes exfiltration near-certain. **Guardrails fail** ("95% is a failing grade"), and **vendors can't protect end users** who mix tools — the only safe move is to avoid the combination. → [[2025-06-16-blog-willison-lethal-trifecta]]

### "Solvable by design — constrain the system"
- **Who:** the security-research camp.
- **Argument:** you can't make the *model* immune, but you can make the *system* safe by construction. **CaMeL** separates control/data flow so untrusted input can never trigger consequential actions, provably outperforming other defenses (→ [[2025-03-24-arxiv-2503-18813v2-defeating-prompt-injections-by-design]]). **Deterministic, pre-LLM enforcement** (Sovereign Execution Brokers) blocks 100% of mutations regardless of model behavior (→ [[2026-06-18-arxiv-2606-20520v1-sovereign-execution-brokers]]). The six design patterns formalize the rule.

## Where it stands
*Less a contradiction than a scope dispute — and they mostly agree:*
- **Both accept the model can't be trusted** to resist injection. Willison even cites CaMeL and the design patterns approvingly.
- The split is **model vs system** and **developer vs end-user**: the research "solves" it *at the system level for app developers* (constrain what untrusted input can do); Willison's "unsolved" is *for end users* freely composing [[mcp|MCP]] tools, where no one has applied those constraints.
- The radar's [[agent-security]] research backs "constrain the system" (deterministic enforcement works); the open problem is that the **easy, popular path (mix-and-match tools) bypasses all of it**. So: solvable in principle, unsolved in the default UX.

## Relationships
- concerns [[agent-security]], [[agent-protocols]], [[tool-use]]
- entities: [[mcp]] · [[tool-description-poisoning]] · [[polaris]]
- participants: [[simon-willison]] (+ the CaMeL / deterministic-enforcement research)
