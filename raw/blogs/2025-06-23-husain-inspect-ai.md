---
source: hamel.dev
url: https://hamel.dev/notes/llm/evals/inspect.html
title: "Inspect AI, An OSS Python Library For LLM Evals"
author: Hamel Husain
date: 2025-06-23
captured: 2026-06-22
note: Immutable raw capture. Verbatim full text from web_fetch (nav/boilerplate and per-slide image refs stripped; timestamps dropped). Annotated guest-lecture presentation by JJ Allaire (creator of Inspect AI; founder of RStudio/Posit).
---

# Inspect AI, An OSS Python Library For LLM Evals

A look at Inspect AI with its creator, JJ Allaire.

A few weeks ago, I hosted JJ Allaire for a guest lecture in our LLM Evals course. JJ is a legend in developer tools — founder of RStudio (now Posit). His latest endeavor is **Inspect AI**, an open-source framework for building and running LLM evaluations, developed during a sabbatical with the UK's AI Safety Institute (AISI), which runs thousands of evaluations on frontier models. It has been adopted by many of the largest AI labs including **Anthropic, DeepMind, and Grok**.

## Core concepts: Dataset, Solver, Scorer
- **Dataset**: test cases, each with an `input` (prompt) and `target` (correct answer / grading guidance).
- **Solver**: a Python function defining how the model generates its output — from a simple model call to complex chains (prompt engineering, self-critique, agent scaffold with tool use). Solvers transform a `TaskState`.
- **Scorer**: evaluates output vs target — text comparison, model-graded (LLM-as-judge), or custom validation.

A `@task` returns a `Task` with a `dataset`, a `plan` (list of solvers like `chain_of_thought`, `self_critique`), and a `scorer`. `eval()` runs it against a model.

## Two views
- **High level**: pre-built building blocks (solvers, scorers) to compose evals quickly. Example tasks: `gpqa_diamond` (multiple choice); `intercode_ctf` (agentic eval — model gets bash/python in a docker container).
- **Low level**: a deep universal LLM interface (caching, logging, metrics, tools, parallel execution); write an async `solve` function for full control over the generation/tool-calling loop — used to build advanced agents.

## Solvers
Baseline solvers: `prompt_template()`, `generate()` (handles the model call and auto-resolves tool calls, repeating the generation→tool loop). `multiple_choice` (rewrites prompt with choices, shuffles to avoid positional bias, maps single-token output back to choice). `self_critique` (generate → critique with a template, optionally a stronger model → regenerate). Composition: custom solvers/scorers packaged as Python packages and shared (e.g., AISI's internal `sheppard` package of jailbreak techniques).

## Agents and tools
First-class tool use via `use_tools()`. Agents: simple ReAct-style "autopilot" agents, or bespoke logic in a custom solver. **Agent Bridges** integrate external libraries (LangChain, Autogen) by monkey-patching the OpenAI API client and proxying calls — lets you evaluate an existing agent (incl. Claude Code planned) without rewriting it. Agent API: tools for Linux/web tasks, state sharing, forking `TaskState` to sub-agents, observability, sandboxing, configurable approval. Pre-built agent tools: Web Search, Bash/Python, Text Editor, Web Browser (headless Chromium), Computer (desktop via screenshots), Think. JJ insisted these tools are **for evals only** — you should run the same pipeline for evals and production, not separate tools. Interactive **agent approval** lets a human approve/reject/terminate sensitive tool calls (safety layer). Built-in agent benchmarks: **GAIA**, **GDM Dangerous Capabilities** (CTF cybersecurity), **SWE-Bench**.

## Scoring & production
Built-in pattern-matching and model-graded scorers, pluggable and customizable; full support for offline/human scoring. Custom scorer example: `expression_equivalence` (regex-extract, then LLM judges mathematical equivalence). Production features: parallelism (`max_connections`, `max_subprocesses`); **Eval Sets** (auto-retry, reuse samples from failed tasks, resume where it left off); comprehensive logging — every run produces a structured `EvalLog` (status, task/model, solver plan, per-sample input/output/score, aggregated results, token usage, errors). Log viewer (`inspect-view`) with bootstrap standard deviation, sample drill-down, message history, assistant-thinking view; VS Code plugin; `inspect view bundle` produces a standalone static report site. Sandbox environments isolate LLM-generated code; `local` sandbox should only be used inside an outer sandbox.

## Q&A highlights
- You can evaluate existing LangChain/Claude Code agents via the Agent Bridge (message-in/message-out wrapping).
- Jailbreaks bypass refusals; they don't generally improve capability benchmarks like SWE-Bench.
- Annotation tooling for dataset creation / judge evaluation is on the roadmap.
- Latency tracked (accounting for retries); token usage tracked as a cost proxy; exact dollar cost via pricing is in a PR.
- Inspect is an open project with 100+ external contributors.
