# Effective harnesses for long-running agents

- **Source:** Anthropic Engineering
- **URL:** https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents
- **Published:** 2025-11-26
- **Author:** Justin Young (+ code RL & Claude Code teams)
- **Captured:** 2026-06-22 (web_fetch, full text)

---

Agents still face challenges working across many context windows. We looked to human engineers for inspiration in creating a more effective harness for long-running agents.

As AI agents become more capable, developers increasingly ask them to take on complex tasks spanning hours or even days. Getting agents to make consistent progress across multiple context windows remains an open problem.

The core challenge: long-running agents must work in discrete sessions, and each new session begins with no memory of what came before. Imagine a software project staffed by engineers working in shifts, where each new engineer arrives with no memory of the previous shift. Because context windows are limited, agents need a way to bridge the gap between coding sessions.

A two-fold solution to enable the **Claude Agent SDK** to work effectively across many context windows: an **initializer agent** that sets up the environment on the first run, and a **coding agent** that makes incremental progress in every session while leaving clear artifacts for the next session. (Code examples in the autonomous-coding quickstart.)

## The long-running agent problem
The Claude Agent SDK is a general-purpose agent harness with context management capabilities such as compaction. However, compaction isn't sufficient. Out of the box, even a frontier coding model like Opus 4.5 running on the Claude Agent SDK in a loop across multiple context windows will fall short of building a production-quality web app from a high-level prompt like "build a clone of claude.ai."

Two failure patterns:
1. The agent tries to do too much at once (one-shot the app), often running out of context mid-implementation, leaving the next session with a feature half-implemented and undocumented.
2. Later in a project, a later agent instance looks around, sees progress was made, and declares the job done.

Solution decomposes into: (1) set up an initial environment laying the foundation for all required features, setting the agent up to work step-by-step; (2) prompt each agent to make incremental progress while leaving the environment in a clean state (mergeable to main: no major bugs, orderly, well-documented).

Two-part solution:
1. **Initializer agent:** the first session uses a specialized prompt to set up the environment — an `init.sh` script, a `claude-progress.txt` log of what agents have done, and an initial git commit.
2. **Coding agent:** every subsequent session makes incremental progress, then leaves structured updates. (These are the same agent — same system prompt, tools, harness — differing only in initial user prompt.)

Key insight: a way for agents to quickly understand the state of work when starting fresh, accomplished via `claude-progress.txt` plus git history. Inspiration came from what effective software engineers do every day.

## Environment management
(Builds on the updated Claude 4 prompting guide's multi-context-window workflows, which use "a different prompt for the very first context window.")

**Feature list** — prompt the initializer agent to write a comprehensive file of feature requirements expanding on the user's prompt. In the claude.ai clone, over 200 features (e.g., "a user can open a new chat, type in a query, press enter, and see an AI response"), all initially marked "failing." Coding agents may edit this file ONLY by changing the `passes` field; strongly-worded instructions: "It is unacceptable to remove or edit tests because this could lead to missing or buggy functionality." Used JSON (the model is less likely to inappropriately overwrite JSON than Markdown).

**Incremental progress** — the coding agent works on only ONE feature at a time; critical to addressing the do-too-much tendency. Leave the environment clean: commit progress to git with descriptive messages, write summaries to a progress file. Git lets the model revert bad changes and recover working states.

**Testing** — Claude tended to mark features complete without proper end-to-end testing (did unit tests / curl against a dev server but failed to verify end-to-end). Explicitly prompting Claude to use browser automation tools and test as a human user would dramatically improved performance (used the Puppeteer MCP server to test the claude.ai clone). Some issues remain: Claude can't see browser-native alert modals through Puppeteer, so features relying on these tended to be buggier.

## Getting up to speed
Every coding agent runs steps to orient: (1) `pwd` to see the working directory; (2) read git logs and progress files; (3) read the feature list and choose the highest-priority not-done feature. The initializer writes an `init.sh` script to run the dev server. In the claude.ai clone, the agent always started the dev server and used Puppeteer to start a new chat, send a message, and receive a response — ensuring it could quickly identify a broken state and fix existing bugs before implementing anything new.

## Failure modes and solutions (summary table)
| Problem | Initializer behavior | Coding-agent behavior |
| --- | --- | --- |
| Declares victory too early | Set up a structured JSON feature list of end-to-end descriptions | Read feature list at session start; choose a single feature |
| Leaves environment buggy/undocumented | Write initial git repo + progress notes | Start by reading progress notes + git logs, run basic test; end by committing + progress update |
| Marks features done prematurely | Set up a feature list file | Self-verify all features; only mark "passing" after careful testing |
| Spends time figuring out how to run the app | Write `init.sh` | Start by reading `init.sh` |

## Future work
Open questions: whether a single general-purpose coding agent performs best, or whether a multi-agent architecture (specialized testing / QA / code-cleanup agents) does better. The demo is optimized for full-stack web app development; future direction is generalizing to other fields (scientific research, financial modeling).
