# RAW CAPTURE — First impressions of Claude Cowork, Anthropic's general agent

- **Author:** Simon Willison
- **Outlet:** simonwillison.net
- **URL:** https://simonwillison.net/2026/Jan/12/claude-cowork/
- **Date:** 2026-01-12
- **Fetched:** 2026-06-22 (via web_fetch)
- **Format:** product first-impressions

## Provenance / framing
Hands-on review of Claude Cowork ("Claude Code for the rest of your work"), Anthropic's general-purpose agent, on day of release.

## Key quotes (verbatim)
- "I've been saying for a while now that Claude Code is a 'general agent' disguised as a developer tool. It can help you with any computer task that can be achieved by executing code or running terminal commands… What it really needs is a UI that doesn't involve the terminal and a name that doesn't scare away non-developers."
- "As far as I can tell Claude Cowork is regular Claude Code wrapped in a less intimidating default interface and with a filesystem sandbox configured for you without you needing to know what a 'filesystem sandbox' is."
- Update — reverse-engineered the app: "Claude uses VZVirtualMachine—the Apple Virtualization Framework—and downloads and boots a custom Linux root filesystem."
- "I think that's a really smart product. Claude Code has an enormous amount of value that hasn't yet been unlocked for a general audience."
- On security: Anthropic's help page advises users to "Monitor Claude for suspicious actions that may indicate prompt injection." Willison: "I do not think it is fair to tell regular non-programmer users to watch out for 'suspicious actions that may indicate prompt injection'!"
- Notes the WebFetch summarization layer is "partly intended as a prompt injection protection layer" (per Claude Code creator Boris Cherny).
- "they can attempt to filter out potential attacks all they like but the one thing they can't provide is guarantees that no future attack will be found that sneaks through their defenses and steals your data (see the lethal trifecta…)."
- "The problem with prompt injection remains that until there's a high profile incident it's really hard to get people to take it seriously."
- "Cowork does at least run in a filesystem sandbox by default, which is more than can be said for my `claude --dangerously-skip-permissions` habit!"
- "This is a general agent that looks well positioned to bring the wildly powerful capabilities of Claude Code to a wider audience. I would be very surprised if Gemini and OpenAI don't follow suit with their own offerings in this category."

## Tags on the post
sandboxing, ai, prompt-injection, generative-ai, llms, anthropic, claude, ai-agents, claude-code, lethal-trifecta, claude-cowork
