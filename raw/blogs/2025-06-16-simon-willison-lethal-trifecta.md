# RAW — The lethal trifecta for AI agents (Simon Willison)
Source: https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/ · 2025-06-16 · captured 2026-06-22 · channel: blog
- Willison (coined "prompt injection", 2022). The "lethal trifecta" = (1) access to private data + (2) exposure to untrusted content + (3) ability to externally communicate. Combine all three and an attacker can exfiltrate your data.
- Root cause: "LLMs follow instructions in content" and "cannot reliably distinguish the importance of instructions based on where they came from."
- Guardrails don't work: vendors claiming "95% of attacks" caught — "95% is very much a failing grade" in security. MCP makes it easy to mix tools that hit all three.
- Mitigations exist for app developers (CaMeL, the six design patterns: "once an agent has ingested untrusted input, it must be constrained so it can't trigger consequential actions") but NOT for end users mixing tools. Only safe path for users: avoid the trifecta combination.
- "The LLM vendors are not going to save us." Distinguishes prompt injection (mixing trusted/untrusted content) from jailbreaking.
Stake: independent practitioner/educator (Datasette/Django co-creator); minimal commercial stake — part of why the warnings carry weight.
