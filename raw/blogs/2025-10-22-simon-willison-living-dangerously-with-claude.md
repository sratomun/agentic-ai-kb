# RAW CAPTURE — Living dangerously with Claude

- **Author:** Simon Willison
- **Outlet:** simonwillison.net
- **URL:** https://simonwillison.net/2025/Oct/22/living-dangerously-with-claude/
- **Date:** 2025-10-22
- **Fetched:** 2026-06-22 (via web_fetch)
- **Format:** annotated talk (given at Claude Code Anonymous, San Francisco)

## Provenance / framing
Annotated slides from a talk at the unofficial Claude Code enthusiasts' meetup. Core dichotomy: he gets *enormous* value running coding agents "with as few restrictions as possible" while being "deeply concerned by the risks that accompany that freedom."

## Key quotes (verbatim)
- "Why you should *always* use `--dangerously-skip-permissions`." … "And why you should *never* use `--dangerously-skip-permissions`."
- "`--dangerously-skip-permissions` is a bit of a mouthful, so I'm going to use its better name, 'YOLO mode'."
- "Claude Code running in this mode genuinely feels like a *completely different product* from regular, default Claude Code." In YOLO mode "you can leave Claude alone to solve all manner of hairy problems while you go and do something else entirely."
- "I have a suspicion that many people who don't appreciate the value of coding agents have never experienced YOLO mode in all of its glory."
- Three projects in 48h were "side quests… pure curiosity that I could outsource to Claude Code and solve in the background." (DeepSeek-OCR on NVIDIA Spark; Pyodide in Node; running 2001-era Perl SLOCCount in WebAssembly.)
- "The reason for this is **prompt injection**, a term I coined three years ago… This remains an incredibly common vulnerability."
- The fundamental rule: "*anyone* who can get their tokens into your context should be considered to have full control over what your agent does next, including the tools that it calls."
- "Some people will try to convince you that prompt injection attacks can be solved using more AI to detect the attacks. This does not work 100% reliably, which means it's not a useful security defense at all."
- "The only solution that's credible is to **run coding agents in a sandbox**." … "The best sandboxes are the ones that run on someone else's computer!" (Codex Cloud, Claude Code for web, Gemini Jules.)
- Two sandboxing problems: filesystem (easy) vs network access (really hard). "Controlling network access cuts off the data exfiltration leg of the lethal trifecta."
- Notes Anthropic's new open-source sandbox-runtime library and macOS `sandbox-exec` (which "has been marked as deprecated in Apple's documentation since at least 2017").
- "So go forth and live dangerously! (But do it in a sandbox.)"

## Tags on the post
sandboxing, security, ai, webassembly, prompt-injection, generative-ai, llms, anthropic, claude, annotated-talks, ai-agents, coding-agents, claude-code, lethal-trifecta, async-coding-agents
