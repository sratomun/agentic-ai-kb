---
type: source
source_type: blog
title: "First impressions of Claude Cowork, Anthropic's general agent"
author: Simon Willison
outlet: simonwillison.net
url: https://simonwillison.net/2026/Jan/12/claude-cowork/
resource: https://simonwillison.net/2026/Jan/12/claude-cowork/
date: 2026-01-12
stake: Independent practitioner/educator — minimal commercial stake
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-security, coding-agents]
---

# First impressions of Claude Cowork, Anthropic's general agent

**Blog** · Simon Willison (simonwillison.net) · 2026-01-12 · [link](https://simonwillison.net/2026/Jan/12/claude-cowork/)

**The take (attributed):** Willison reads Claude Cowork as the move he'd predicted — "Claude Code is a general agent disguised as a developer tool" — repackaged with a non-scary UI and a default sandbox; smart product, but he flags that telling non-programmers to "watch out for prompt injection" is not a real defense.

**Stake:** Independent — hands-on day-of-release review; praises the product while pressing on its security posture.

## Argument
- The thesis he's repeated: "I've been saying for a while now that Claude Code is a 'general agent' disguised as a developer tool. It can help you with any computer task that can be achieved by executing code or running terminal commands… What it really needs is a UI that doesn't involve the terminal and a name that doesn't scare away non-developers." Cowork is exactly that: "regular Claude Code wrapped in a less intimidating default interface and with a filesystem sandbox configured for you without you needing to know what a 'filesystem sandbox' is."
- He reverse-engineered the app: "Claude uses VZVirtualMachine—the Apple Virtualization Framework—and downloads and boots a custom Linux root filesystem." Verdict: "a really smart product. Claude Code has an enormous amount of value that hasn't yet been unlocked for a general audience."
- **Security pushback.** Anthropic's help page advises users to "Monitor Claude for suspicious actions that may indicate prompt injection." Willison: "I do not think it is fair to tell regular non-programmer users to watch out for 'suspicious actions that may indicate prompt injection'!" He notes the WebFetch summarization layer is "partly intended as a prompt injection protection layer" (per Claude Code creator Boris Cherny), but: "they can attempt to filter out potential attacks all they like but the one thing they can't provide is guarantees that no future attack will be found that sneaks through their defenses and steals your data (see the lethal trifecta…)." Bigger structural point: "until there's a high profile incident it's really hard to get people to take it seriously." He concedes Cowork "does at least run in a filesystem sandbox by default, which is more than can be said for my `claude --dangerously-skip-permissions` habit!"
- Market call: "This is a general agent that looks well positioned to bring the wildly powerful capabilities of Claude Code to a wider audience. I would be very surprised if Gemini and OpenAI don't follow suit."

## Why it matters / where it cuts
The category-defining moment for "general agents for non-developers" — and the clearest articulation that the coding-agent runtime *is* the general-agent runtime, just rebranded. The security angle is the load-bearing radar signal: a default sandbox is progress, but the residual prompt-injection risk gets pushed onto users who can't evaluate it, restating his [[debate-prompt-injection-solvable|"unsolved for end users"]] position in a mass-market context. Ties [[coding-agents]] → general [[agentic-ai]].

## Graph
- **Author:** [[simon-willison]]
- **Concepts:** [[agentic-ai]] · [[coding-agents]] · [[agent-security]] · [[tool-use]]
- **Entities:** [[claude]] · [[anthropic]] · [[tool-description-poisoning]] · [[mcp]]
- **Debate:** [[debate-prompt-injection-solvable]]
- **Raw:** `raw/blogs/2026-01-12-simon-willison-claude-cowork.md`
