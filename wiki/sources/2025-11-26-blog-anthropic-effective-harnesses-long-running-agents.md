---
type: source
source_type: blog
title: "Effective harnesses for long-running agents"
author: Justin Young (Anthropic)
outlet: Anthropic Engineering
url: https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents
resource: https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents
date: 2025-11-26
stake: Anthropic (sells Claude + the Agent SDK) — demonstrates the Agent SDK on a long-horizon coding task
ingested: 2026-06-22
tags: [perspective, harness-engineering, coding-agents, agentic-ai]
---

# Effective harnesses for long-running agents

**Blog** · Justin Young ([[anthropic|Anthropic]] Engineering) · 2025-11-26 · [link](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)

**The take (attributed):** Anthropic argues that **compaction alone isn't enough** for agents that must work across many context windows — even Opus 4.5 on the Agent SDK fails to one-shot a production web app. Their fix borrows from how human engineers work in shifts: an **initializer agent** that scaffolds the environment, plus a **coding agent** that does *one feature at a time* and leaves clean, documented artifacts (git history + a progress file) for the next session.

**Stake:** Anthropic sells Claude and the Agent SDK; this is a demo of *its* harness (with an autonomous-coding quickstart) doing long-horizon software engineering on its own frontier model.

## Argument
- **The core problem:** agents work in discrete sessions with no memory of the prior one — "engineers working in shifts." Out of the box, even Opus 4.5 on the Agent SDK falls short of "build a clone of claude.ai."
- **Two failure modes:** (1) trying to one-shot the app → runs out of context mid-feature, leaving undocumented half-work; (2) a later instance sees prior progress and *prematurely declares done*.
- **Two-part harness:** an **initializer agent** writes `init.sh`, a `claude-progress.txt` log, and an initial git commit; the **coding agent** makes incremental progress then leaves structured updates. (Same agent — only the first user prompt differs.)
- **Feature list:** the initializer writes a structured **JSON** file (>200 features for the claude.ai clone), all marked "failing"; coding agents may only flip the `passes` field — "It is unacceptable to remove or edit tests." JSON chosen because the model is less likely to overwrite it than Markdown.
- **Incremental + clean state:** one feature per session; commit to git with descriptive messages so the model can revert and recover working states.
- **Testing:** Claude marked features done without true end-to-end testing until *explicitly* prompted to use browser automation (Puppeteer MCP) and test as a human user — which dramatically improved results. Limits remain (can't see native alert modals through Puppeteer).
- **Orientation ritual each session:** `pwd` → read git log + progress file → pick highest-priority unfinished feature → run a basic dev-server test before building anything new.
- **Future work:** maybe specialized multi-agent roles (testing/QA/cleanup) beat one general agent; generalize beyond web apps to research and financial modeling.

## Why it matters / where it cuts
The most concrete recipe yet for **long-horizon autonomous coding** — and an honest admission that the hard part is *harness design*, not raw model capability. The git-history-plus-progress-file pattern is directly reusable. Extends [[2025-09-29-blog-anthropic-effective-context-engineering]] (compaction is necessary but insufficient) and anchors [[harness-engineering]]; relevant to [[coding-agents]] and the autonomy side of [[debate-agents-vs-workflows]].

## Graph
- **Author:** [[anthropic|Anthropic]] (code RL / Claude Code teams)
- **Entities:** [[anthropic]] · [[mcp]] · [[claude]]
- **Concepts:** [[harness-engineering]] · [[coding-agents]] · [[agentic-ai]] · [[agent-memory]] · [[multi-agent-systems]]
- **Debate:** [[debate-agents-vs-workflows]]
- **Raw:** `raw/blogs/2025-11-26-anthropic-effective-harnesses-long-running-agents.md`
