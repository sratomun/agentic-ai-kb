# Introducing deep research

Source: https://openai.com/index/introducing-deep-research/
Author: OpenAI
Date: February 2, 2025
Category: Release
Captured: 2026-06-22
Vendor stake: OpenAI launching/marketing its own agentic product (deep research in ChatGPT). Benchmark figures (HLE, GAIA) and "research-analyst level" framing are self-reported.

---

Today we're launching deep research in ChatGPT, a new agentic capability that conducts multi-step research on the internet for complex tasks. It accomplishes in tens of minutes what would take a human many hours.

Deep research is OpenAI's next agent that can do work for you independently—you give it a prompt, and ChatGPT will find, analyze, and synthesize hundreds of online sources to create a comprehensive report at the level of a research analyst. Powered by a version of the upcoming OpenAI o3 model optimized for web browsing and data analysis, it leverages reasoning to search, interpret, and analyze massive amounts of text, images, and PDFs on the internet, pivoting as needed in reaction to information it encounters.

"The ability to synthesize knowledge is a prerequisite for creating new knowledge. For this reason, deep research marks a significant step toward our broader goal of developing AGI, which we have long envisioned as capable of producing novel scientific research."

## Why we built deep research
Built for people who do intensive knowledge work in finance, science, policy, and engineering and need thorough, precise, and reliable research; also useful for discerning shoppers. Every output is fully documented, with clear citations and a summary of its thinking. It is particularly effective at finding niche, non-intuitive information that would require browsing numerous websites.

It was trained on real-world tasks requiring browser and Python tool use, using the same reinforcement learning methods behind OpenAI o1. While o1 demonstrates impressive capabilities in coding, math, and other technical domains, many real-world challenges demand extensive context and information gathering; deep research builds on these reasoning capabilities to bridge that gap.

## How it works
Deep research was trained using end-to-end reinforcement learning on hard browsing and reasoning tasks across a range of domains. It learned to plan and execute a multi-step trajectory to find the data it needs, backtracking and reacting to real-time information. It can browse user-uploaded files, plot and iterate on graphs using the Python tool, embed generated graphs and images from websites, and cite specific sentences or passages from its sources.

### Humanity's Last Exam
The model powering deep research scores a new high at 26.6% accuracy. (Comparison table: GPT-4o 3.3; Grok-2 3.8; Claude 3.5 Sonnet 4.3; Gemini Thinking 6.2; OpenAI o1 9.1; DeepSeek-R1 9.4; o3-mini medium 10.5; o3-mini high 13.0; OpenAI deep research 26.6 — deep research figure with browsing + python tools.)

### GAIA (public benchmark, real-world questions)
The model reaches a new state of the art, topping the external leaderboard.
- Previous SOTA: L1 67.92, L2 67.44, L3 42.31, Avg 63.64
- Deep Research (pass@1): L1 74.29, L2 69.06, L3 47.6, Avg 67.36
- Deep Research (cons@64): L1 78.66, L2 73.21, L3 58.03, Avg 72.57

### Expert-level tasks
In an internal evaluation, deep research was rated by domain experts to have automated multiple hours of difficult manual investigation. "The more the model browses and thinks about what it's browsing, the better it does." Estimated economic value of a task is more correlated with pass rate than the number of hours it would take a human.

## Limitations
Can sometimes hallucinate facts or make incorrect inferences (at a notably lower rate than existing ChatGPT models, per internal evaluations). May struggle to distinguish authoritative information from rumors; shows weakness in confidence calibration. Minor formatting/citation errors at launch.

## Access
Compute intensive; started with a Pro-optimized version (up to 100 queries/month), with Plus and Team next, then Enterprise.
- Later updates noted in post: Feb 25, 2025 all Plus users; Apr 24, 2025 rate-limit increases via a lightweight version powered by a version of o4-mini (Plus/Team/Enterprise/Edu 25/month, Pro 250, Free 5); Jul 17, 2025 deep research can use a visual browser as part of ChatGPT agent; Feb 10, 2026 deep research can connect to any MCP or app and restrict web searches to trusted sites, with real-time progress tracking and interrupt-to-refine.

## What's next
Future: connect to more specialized data sources (subscription-based or internal). "We envision agentic experiences coming together in ChatGPT for asynchronous, real-world research and execution. The combination of deep research... and Operator, which can take real-world action, will enable ChatGPT to carry out increasingly sophisticated tasks."

Feb 3, 2025 addendum: rigorous safety testing on the early version of o3 that powers deep research identified it as Medium risk under the Preparedness Framework; additional safety testing and mitigations added for web browsing.

Tags: Release · 2025
