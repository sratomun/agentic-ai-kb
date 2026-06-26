---
type: source
source_type: talk
title: "Living dangerously with Claude"
author: Simon Willison
outlet: simonwillison.net (annotated talk, Claude Code Anonymous SF)
url: https://simonwillison.net/2025/Oct/22/living-dangerously-with-claude/
resource: https://simonwillison.net/2025/Oct/22/living-dangerously-with-claude/
date: 2025-10-22
stake: Independent practitioner/educator — minimal commercial stake
ingested: 2026-06-22
tags: [perspective, agent-security, coding-agents]
---

# Living dangerously with Claude

**Talk (annotated)** · Simon Willison (simonwillison.net) · 2025-10-22 · [link](https://simonwillison.net/2025/Oct/22/living-dangerously-with-claude/)

**The take (attributed):** Willison argues the only *credible* defense for an unrestricted coding agent isn't smarter filtering — it's a **sandbox**, and specifically one that cuts off network access to kill the exfiltration leg of the [[tool-description-poisoning|lethal trifecta]].

**Stake:** Independent — coined "prompt injection" (2022); no vendor to sell. He's openly conflicted here: enormous personal value from running agents wide-open, paired with genuine alarm at the risk.

## Argument
- The dichotomy: he gets *enormous* value running coding agents "with as few restrictions as possible" — what he calls **"YOLO mode"** (`--dangerously-skip-permissions`) — while being "deeply concerned by the risks that accompany that freedom." YOLO mode "genuinely feels like a completely different product" — you can leave the agent to grind on hairy problems unattended. He suspects skeptics of coding-agent value "have never experienced YOLO mode in all of its glory" (three throwaway side-quest projects in 48h as proof).
- The risk is **prompt injection** — "a term I coined three years ago… This remains an incredibly common vulnerability." His fundamental rule: "*anyone* who can get their tokens into your context should be considered to have full control over what your agent does next, including the tools that it calls."
- **AI-detects-the-attack doesn't work:** "Some people will try to convince you that prompt injection attacks can be solved using more AI to detect the attacks. This does not work 100% reliably, which means it's not a useful security defense at all." (His recurring "95% is a failing grade" stance, restated.)
- **The only credible solution is a sandbox** — "The best sandboxes are the ones that run on someone else's computer!" (Codex Cloud, Claude Code for web, Gemini Jules). Two sub-problems: filesystem isolation (easy) vs network access (hard) — and "controlling network access cuts off the data exfiltration leg of the lethal trifecta." Notes Anthropic's new open-source sandbox-runtime library and that macOS `sandbox-exec` has been deprecated in Apple's docs since ~2017.
- Verdict: "So go forth and live dangerously! (But do it in a sandbox.)"

## Why it matters / where it cuts
This is the constructive sequel to the lethal-trifecta framing: having named the problem, he names the one mitigation he'll endorse for end users running agents — sandboxing, with network egress as the load-bearing control. It feeds [[debate-prompt-injection-solvable]] (the "manage, don't solve" side) and connects the security thesis to the [[coding-agents]] vertical where he actually lives.

## Graph
- **Author:** [[simon-willison]]
- **Concepts:** [[agent-security]] · [[coding-agents]] · [[tool-use]]
- **Entities:** [[tool-description-poisoning]] · [[mcp]] · [[anthropic]] · [[claude]]
- **Debate:** [[debate-prompt-injection-solvable]]
- **Raw:** `raw/blogs/2025-10-22-simon-willison-living-dangerously-with-claude.md`
