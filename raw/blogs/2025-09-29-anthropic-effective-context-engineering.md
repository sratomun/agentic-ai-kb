# Effective context engineering for AI agents

- **Source:** Anthropic Engineering
- **URL:** https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- **Published:** 2025-09-29
- **Authors:** Anthropic Applied AI team — Prithvi Rajasekaran, Ethan Dixon, Carly Ryan, Jeremy Hadfield (+ contributors)
- **Captured:** 2026-06-22 (web_fetch, full text)

---

Context is a critical but finite resource for AI agents. This post explores strategies for curating and managing the context that powers them.

A new term has come to prominence after years of prompt engineering: **context engineering**. Building with language models is becoming less about finding the right words for prompts and more about "what configuration of context is most likely to generate our model's desired behavior?"

**Context** = the set of tokens included when sampling from an LLM. The engineering problem is optimizing the utility of those tokens against the inherent constraints of LLMs.

## Context engineering vs. prompt engineering
Anthropic views context engineering as the natural progression of prompt engineering. Prompt engineering = methods for writing/organizing instructions (esp. system prompts). Context engineering = strategies for curating and maintaining the optimal set of tokens during inference, including all the information beyond the prompts (system instructions, tools, MCP, external data, message history, etc). As agents operate over multiple turns and longer time horizons, we need to manage the entire context state. Context engineering is iterative — curation happens each time we decide what to pass to the model.

## Why context engineering is important
LLMs, like humans, lose focus or experience confusion at a certain point. **Context rot:** as the number of tokens in the context window increases, the model's ability to accurately recall information decreases (needle-in-a-haystack benchmarking). Context must be treated as a finite resource with diminishing marginal returns. LLMs have an "attention budget" that depletes with every new token. This stems from architectural constraints: transformers enable every token to attend to every other token, producing n² pairwise relationships for n tokens. As context length grows, the ability to capture these relationships gets stretched thin. Models also develop attention patterns from training distributions where shorter sequences are more common. These create a performance gradient rather than a hard cliff.

## The anatomy of effective context
Good context engineering = finding the smallest possible set of high-signal tokens that maximize the likelihood of a desired outcome.

**System prompts** should be clear, simple, direct, at the *right altitude* — the Goldilocks zone between hardcoded brittle if-else logic and vague high-level guidance. Organize prompts into distinct sections (`<background_information>`, `<instructions>`, `## Tool guidance`, `## Output description`) using XML tags or Markdown headers. Strive for the minimal set of information that fully outlines expected behavior (minimal ≠ short). Start by testing a minimal prompt with the best model available, then add instructions/examples based on failure modes.

**Tools** define the contract between agents and their information/action space. Tools should return token-efficient information and encourage efficient agent behaviors; be self-contained, robust to error, clear about intended use. A common failure mode: bloated tool sets that cover too much functionality or create ambiguous decision points. If a human engineer can't say which tool to use, an AI agent can't either.

**Examples (few-shot prompting)** remain strongly advised — but don't stuff a laundry list of edge cases. Curate a set of diverse, canonical examples.

Overall guidance: keep context informative yet tight.

## Context retrieval and agentic search
Simple definition adopted (per Simon Willison): **agents = LLMs autonomously using tools in a loop**. As models become more capable, agent autonomy can scale.

A shift in designing context: from embedding-based pre-inference-time retrieval toward **"just in time" context strategies**. Rather than pre-processing all relevant data up front, agents maintain lightweight identifiers (file paths, stored queries, web links) and use these references to dynamically load data into context at runtime via tools. Claude Code uses this to perform complex data analysis over large databases — writing targeted queries, storing results, leveraging Bash commands like `head` and `tail` to analyze large volumes without loading full data objects into context. This mirrors human cognition (file systems, inboxes, bookmarks).

Metadata of references refines behavior: a file named `test_utils.py` in a `tests` folder implies a different purpose than the same name in `src/core_logic/`. Folder hierarchies, naming conventions, and timestamps all provide signals. Letting agents navigate/retrieve autonomously enables **progressive disclosure** — incrementally discovering relevant context through exploration.

Trade-off: runtime exploration is slower than retrieving pre-computed data; requires thoughtful engineering so the LLM has the right tools and heuristics. The most effective agents might employ a **hybrid strategy** (retrieve some data up front for speed; pursue further autonomous exploration). Claude Code is a hybrid: CLAUDE.md files dropped into context up front, while glob/grep navigate just-in-time. "Do the simplest thing that works" will likely remain the best advice.

## Context engineering for long-horizon tasks
For tasks spanning tens of minutes to multiple hours (large codebase migrations, comprehensive research), token count exceeds the context window. Three techniques address context pollution directly:

**Compaction** — take a conversation nearing the limit, summarize its contents, reinitiate a new context window with the summary. Typically the first lever. In Claude Code, the message history is passed to the model to summarize; it preserves architectural decisions, unresolved bugs, and implementation details while discarding redundant tool outputs. The agent continues with compressed context plus the five most recently accessed files. The art lies in selecting what to keep vs discard. Tune the prompt: maximize recall first, then improve precision. A safe lightest-touch form is **tool result clearing** (now a feature on the Claude Developer Platform).

**Structured note-taking (agentic memory)** — the agent regularly writes notes persisted to memory outside the context window (e.g., a NOTES.md file, a to-do list), pulled back in later. Claude playing Pokémon demonstrates this in a non-coding domain: maintaining tallies across thousands of game steps, developing maps, remembering achievements, after context resets reading its own notes to continue multi-hour sequences. As part of the Sonnet 4.5 launch, Anthropic released a **memory tool** (public beta) — file-based storage outside the context window so agents build knowledge bases over time and maintain project state across sessions.

**Sub-agent architectures** — specialized sub-agents handle focused tasks with clean context windows. The main agent coordinates with a high-level plan while subagents perform deep work, each potentially using tens of thousands of tokens but returning only a condensed 1,000-2,000-token summary. Clear separation of concerns. (Per "How we built our multi-agent research system" — substantial improvement over single-agent systems on complex research.)

Choosing between approaches:
- Compaction → tasks requiring extensive back-and-forth;
- Note-taking → iterative development with clear milestones;
- Multi-agent → complex research/analysis where parallel exploration pays dividends.

## Conclusion
Context engineering represents a fundamental shift. The challenge isn't crafting the perfect prompt — it's thoughtfully curating what information enters the model's limited attention budget at each step. Find the smallest set of high-signal tokens that maximize the likelihood of the desired outcome. Smarter models require less prescriptive engineering, allowing more autonomy — but treating context as a precious, finite resource will remain central.
