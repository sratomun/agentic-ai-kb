# Components of A Coding Agent
## How coding agents use tools, memory, and repo context to make LLMs work better in practice

**Sebastian Raschka, PhD — Apr 04, 2026 — Ahead of AI**
Source: https://magazine.sebastianraschka.com/p/components-of-a-coding-agent

---

In this article, I want to cover the overall design of coding agents and agent harnesses: what they are, how they work, and how the different pieces fit together in practice.

Agents have become an important topic because much of the recent progress in practical LLM systems is not just about better models, but about how we use them. In many real-world applications, the surrounding system, such as tool use, context management, and memory, plays as much of a role as the model itself. This also helps explain why systems like Claude Code or Codex can feel significantly more capable than the same models used in a plain chat interface.

## Claude Code, Codex CLI, and Other Coding Agents

Claude Code and the Codex CLI are essentially agentic coding tools that wrap an LLM in an application layer, a so-called agentic harness, to be more convenient and better-performing for coding tasks. Coding agents are engineered for software work where the notable parts are not only the model choice but the surrounding system, including repo context, tool design, prompt-cache stability, memory, and long-session continuity.

## On The Relationship Between LLMs, Reasoning Models, and Agents

An LLM is the core next-token model. A reasoning model is still an LLM, but usually one that was trained and/or prompted to spend more inference-time compute on intermediate reasoning, verification, or search over candidate answers. An agent is a layer on top — a control loop around the model. Given a goal, the agent layer (or harness) decides what to inspect next, which tools to call, how to update its state, and when to stop.

Roughly: the LLM is the engine, a reasoning model is a beefed-up engine (more powerful, but more expensive to use), and an agent harness helps us [use] the model.

Summary:
- *LLM:* the raw model
- *Reasoning model:* an LLM optimized to output intermediate reasoning traces and to verify itself more
- *Agent:* a loop that uses a model plus tools, memory, and environment feedback
- *Agent harness:* the software scaffold around an agent that manages context, tool use, prompts, state, and control flow
- *Coding harness:* a special case of an agent harness; a task-specific harness for software engineering that manages code context, tools, execution, and iterative feedback

Coding work is only partly about next-token generation. A lot of it is about repo navigation, search, function lookup, diff application, test execution, error inspection, and keeping all the relevant information in context.

## The Coding Harness

When we say harness, we typically mean the software layer around the model that assembles prompts, exposes tools, tracks file state, applies edits, runs commands, manages permissions, caches stable prefixes, stores memory, and more.

Since the vanilla versions of LLMs nowadays have very similar capabilities (e.g., GPT-5.4, Opus 4.6, GLM-5), the harness can often be the distinguishing factor that makes one LLM work better than another. This is speculative, but I suspect that if we dropped one of the latest, most capable open-weight LLMs, such as GLM-5, into a similar harness, it could likely perform on par with GPT-5.4 in Codex or Claude Opus 4.6 in Claude Code. That said, some harness-specific post-training is usually beneficial (e.g., OpenAI historically maintained separate GPT-5.3 and GPT-5.3-Codex variants).

Six main components (annotated in the from-scratch Mini Coding Agent, https://github.com/rasbt/mini-coding-agent):
1. Live Repo Context → WorkspaceContext
2. Prompt Shape And Cache Reuse → build_prefix, memory_text, prompt
3. Structured Tools, Validation, And Permissions → build_tools, run_tool, validate_tool, approve, parse, path, tool_*
4. Context Reduction And Output Management → clip, history_text
5. Transcripts, Memory, And Resumption → SessionStore, record, note_tool, ask, reset
6. Delegation And Bounded Subagents → tool_delegate

## 1. Live Repo Context

When a user says "fix the tests" or "implement xyz," the model should know whether it is inside a Git repo, what branch it is on, which project documents might contain instructions. "Fix the tests" is not a self-contained instruction. If the agent sees AGENTS.md or a project README, it may learn which test command to run. The coding agent collects info ("stable facts" as a workspace summary) upfront before doing any work, so it's not starting from zero on every prompt.

## 2. Prompt Shape And Cache Reuse

It would be relatively wasteful to combine and re-process the workspace summary on every user query. Coding sessions are repetitive, and the agent rules, tool descriptions, and workspace summary usually stay the same. "Smart" runtimes don't rebuild everything as one giant undifferentiated prompt on every turn. The "Stable prompt prefix" (general instructions, tool descriptions, workspace summary) is reused/cached; the changing parts (short-term memory, recent transcript, newest user request) update each turn.

## 3. Tool Access and Use

A plain model can suggest commands in prose, but an LLM in a coding harness should actually execute the command and retrieve the results. Instead of letting the model improvise arbitrary syntax, the harness usually provides a pre-defined list of allowed and named tools with clear inputs and boundaries (though something like Python `subprocess.call` can be part of this). The runtime can stop and run programmatic checks: "Is this a known tool?", "Are the arguments valid?", "Does this need user approval?", "Is the requested path even inside the workspace?" Only after those checks pass does anything run. In a sense, the harness is giving the model less freedom, but it also improves usability and reliability at the same time.

## 4. Minimizing Context Bloat

Context bloat is an issue for LLMs in general, but coding agents are even more susceptible because of repeated file reads, lengthy tool outputs, logs. A minimal harness uses at least two compaction strategies: (1) clipping — shortens long document snippets, tool outputs, memory notes, transcript entries; (2) transcript reduction/summarization — keep recent events richer (more likely to matter) and compress older events more aggressively; also deduplicate older file reads. "A lot of apparent 'model quality' is really context quality."

## 5. Structured Session Memory

A coding agent separates state into (at least) two layers: working memory (the small, distilled state the agent keeps explicitly) and a full transcript (all user requests, tool outputs, LLM responses; resumable). The compact transcript is for prompt reconstruction; the working memory is for task continuity (current task, important files, recent notes). Session files are usually stored as JSON on disk.

## 6. Delegation With (Bounded) Subagents

Delegation lets us parallelize work into subtasks via subagents. A subagent is only useful if it inherits enough context to do real work, but if we don't restrict it, we get multiple agents duplicating work or touching the same files. The trick is the subagent inherits enough context to be useful but is constrained (e.g., read-only, restricted recursion depth). Claude Code has supported subagents for a long time; Codex added them more recently (Codex does not generally force subagents into read-only mode — boundary is more about task scoping, context, and depth).

## How Does This Compare To OpenClaw?

OpenClaw is more like a local, general agent platform that can also code, rather than a specialized terminal coding assistant. Overlaps: prompt/instruction files (AGENTS.md, SOUL.md, TOOLS.md), JSONL session files with transcript compaction, helper sessions/subagents. But the emphasis differs: coding agents are optimized for a person working in a repository; OpenClaw is optimized for running many long-lived local agents across chats, channels, and workspaces.

---
*Note: He also announces Build A Reasoning Model (From Scratch) is finished (early access). Main topics: evaluating reasoning models, inference-time scaling, self-refinement, reinforcement learning, distillation.*

*Raw capture — immutable. Stripped of Substack nav/footer/comments/figure-URLs. Author: Sebastian Raschka (Raschka AI Research / RAIR Lab LLC), independent.*
