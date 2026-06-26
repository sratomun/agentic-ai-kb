---
title: "Vibe engineering"
author: Simon Willison
outlet: Simon Willison's Weblog
url: https://simonwillison.net/2025/Oct/7/vibe-engineering/
date: 2025-10-07
captured: 2026-06-22
source_type: blog
---

# Vibe engineering

*Full text captured verbatim for the radar. Immutable.*

Vibe coding is pretty well established now as covering the fast, loose and irresponsible way of building software with AI — entirely prompt-driven, with no attention paid to how the code actually works. This leaves a terminology gap: what should we call the other end of the spectrum, where seasoned professionals accelerate their work with LLMs while staying proudly and confidently accountable for the software they produce?

I propose we call this **vibe engineering**, with my tongue only partially in my cheek.

*Update 23rd February 2026: It looks like the term "Agentic Engineering" is coming out on top for this now. I have a new tag for that and I'm working on a not-quite-a-book (Agentic Engineering Patterns).*

One of the lesser spoken truths of working productively with LLMs as a software engineer on non-toy-projects is that it's *difficult*. The pace at which they churn out working code raises the bar for what the human participant can and should be contributing.

The rise of **coding agents** — Claude Code (released February 2025), OpenAI's Codex CLI (April), Gemini CLI (June) that iterate on code, actively testing and modifying until it achieves a specified goal — has dramatically increased the usefulness of LLMs for real-world coding. Experienced engineers are now running multiple copies of agents at once, tackling several problems in parallel.

LLMs actively reward existing top-tier software engineering practices:
- **Automated testing** — a robust, stable test suite lets agentic tools *fly*; without tests an agent might claim something works without testing it. Test-first is particularly effective with agents that iterate in a loop.
- **Planning in advance** — iterate on a high-level plan first, then hand it off.
- **Comprehensive documentation** — feed in relevant docs so the model can use APIs without reading the code.
- **Good version control habits** — LLMs are fiercely competent at Git (git bisect to find bug origins).
- **Effective automation** — CI, formatting, linting, continuous deployment to preview environments.
- **A culture of code review** — if you're fast at code review you'll have a much better time.
- **A very weird form of management** — clear instructions, context, actionable feedback; management experience proves surprisingly useful.
- **Really good manual QA** — predicting and digging into edge-cases.
- **Strong research skills** — figuring out the best of dozens of approaches.
- **The ability to ship to a preview environment** — safely preview a feature before production.
- **An instinct for what can be outsourced** to AI vs handled manually (constantly evolving).
- **An updated sense of estimation** — AI-assisted coding makes estimation even harder.

"If you're going to really exploit the capabilities of these new tools, you need to be operating *at the top of your game*. You're not just responsible for writing the code—you're researching approaches, deciding on high-level architecture, writing specifications, defining success criteria, designing agentic loops, planning QA, managing a growing army of weird digital interns who will absolutely cheat if you give them a chance, and spending *so much time on code review*."

Almost all of these are characteristics of senior software engineers already. **AI tools amplify existing expertise** — the more skills and experience you have, the faster and better the results.

#### "Vibe engineering", really?
Probably a stupid name. "Vibe coding" is used dismissively by many developers. Vibe engineering establishes a clear distinction: a different, harder, more sophisticated way of working with AI tools to build production software. Simon likes the self-contradiction between "vibes" and "engineering."
