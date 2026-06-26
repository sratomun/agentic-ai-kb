# RAW — Agents (Chip Huyen, huyenchip.com)
Source: https://huyenchip.com/2025/01/07/agents.html · 2025-01-07 · captured 2026-06-22 · channel: blog
Note: Adapted from the **Agents** chapter (Ch. 6) of *AI Engineering* (O'Reilly, 2025) "with minor edits to make it a standalone post." So this is the canonical, public version of the book's agent material.

## Core definitions
- An **agent** = "anything that can perceive its environment and act upon that environment" (Russell & Norvig framing). Characterized by (1) its **environment** and (2) the **set of actions** it can perform. The action set is augmented by the **tools** it has access to.
- Strong dependency between environment and tools: the environment determines which tools are usable; the tool inventory restricts which environment the agent can operate in.
- "ChatGPT is an agent. … RAG systems are agents — text retrievers, image retrievers, and SQL executors are their tools." (Agents framed broadly, not as a special new artifact.)
- The AI model is "the brain that processes the task, plans a sequence of actions … and determines whether the task has been accomplished."

## Why agents need stronger models (two reasons)
- **Compound mistakes**: multi-step → accuracy compounds down. "If the model's accuracy is 95% per step, over 10 steps … 60%, and over 100 steps … only 0.6%." (Key quantitative claim.)
- **Higher stakes**: tool access → more impactful actions → any failure has more severe consequences.
- Cost critique acknowledged: "agents are only good for burning through your API credits" — but if autonomous, they save human time, making cost worthwhile.

## Tools — three categories
1. **Knowledge augmentation** (context construction): text/image retrievers, SQL executor, internal people search, inventory API, Slack/email readers, **web browsing** (umbrella term for all internet-access tools; prevents the model going "stale"). Caveat: internet tools "open up your agent to the cesspools of the internet."
2. **Capability extension**: fix inherent model weaknesses — calculator (models bad at math; "199,999 / 292" fails), calendar, timezone/unit converters, translators, **code interpreters** (powerful but code-injection risk → defensive prompt engineering). Tools can turn a text-only model multimodal (text→image model, image captioner, OCR, transcription). Cites **Chameleon** (Lu et al. 2023): GPT-4 + 13 tools beats GPT-4 alone — +11.37% on ScienceQA, +17% on TabMWP.
3. **Write actions**: change data sources (SQL write/delete, send email, initiate bank transfer). Enables end-to-end automation (customer outreach: research → contact → draft → send → follow-up → update DB). BUT: "you shouldn't allow an unreliable AI to initiate bank transfers." Trust + security crucial.
- Sidebar (Agents & security): self-driving-car-hijack fear is visceral but AI can harm without physical presence (market manipulation, copyright theft, privacy, bias, misinfo). Doesn't mean never give AI real-world action — "I would trust a self-driving car more than the average stranger to give me a lift."
- Tool use ≈ function calling; expects function calling with wide tool sets to become common across most models.

## Planning
- Task = goal + constraints (e.g., 2-week SF→India trip, budget $5,000).
- **Decouple planning from execution**: generate plan → **validate** → only then execute. Avoids agent running a bad 1,000-step plan "for hours, wasting time and money." Validate via heuristics (drop invalid-action plans; drop >X-step plans) or **AI judges** (ask a model if the plan is reasonable).
- System ⇒ 3 components: plan generator, plan validator, plan executor. "If you consider each component an agent, this can be considered a **multi-agent system**. Because most agentic workflows are sufficiently complex … **most agents are multi-agent**." (Notable framing claim.)
- **Intent classification** helps planning + tool selection; should be able to classify requests as `IRRELEVANT` so the agent politely rejects instead of "wasting FLOPs."
- **Humans-in-the-loop** at any stage (provide/validate/execute plan; explicit approval before risky ops). Need to define the level of automation per action.
- Solving a task = plan generation (task decomposition) → reflection/error-correction → execution → reflection/error-correction. Reflection isn't mandatory but "will significantly boost the agent's performance."

### Foundation models as planners (the LeCun debate)
- Open question whether FMs can plan. Yann LeCun (Meta Chief AI Scientist): "Auto-Regressive LLMs can't plan (and can't really reason)."
- Huyen's counter: planning is a **search problem** (search paths, predict reward, pick best; backtracking). Autoregressive ≠ can't backtrack — model can revise/restart a path. LLMs may be poor planners because they aren't given the **tooling** (action outcomes / world model). Cites Hao et al. 2023 "Reasoning with Language Model is Planning with World Model" — LLM contains enough world info to predict action outcomes. "Even if AI can't plan, it can still be a part of a planner" (augment with search tool + state tracking).
- Sidebar FM vs RL planners: RL planner trained by RL algo (costly); FM planner = the model itself (prompt/finetune, cheaper). "I suspect that in the long run, FM agents and RL agents will merge."

### Plan generation
- Simplest = prompt engineering (system prompt listing valid actions + few-shot examples → outputs a plan = sequence of functions).
- **Function calling**: declare tool inventory (name, params, docs); specify per-query allowed tools; controls `required` / `none` / `auto`. APIs can guarantee valid function names but NOT correct parameter values. Hallucination can produce invalid function or wrong params. Tips to improve planning: better system prompt + examples; better tool/param descriptions; simpler functions; stronger model; finetune for plan generation.
- **Planning granularity**: planning/execution tradeoff (detailed plan = harder to generate, easier to execute; high-level = reverse). Solve via **hierarchical planning**. Using exact function names is brittle (rename breaks prompt + finetuning); prefer **natural-language plans** + a translator ("program generator" in Chameleon) — robust to tool-API change; translation is easier than planning, so a weaker model can do it.
- **Complex plans / control flow**: sequential, parallel, if-statement (Anthropic calls this "routing"), for-loop. AI determines control flow (vs exact conditions in traditional SWE). Tip: check what control flows a framework supports (e.g., can it browse 10 sites in parallel?).

### Reflection & error correction
- Useful after: query received (feasible?), plan generated (sensible?), each execution step (on track?), whole plan executed (goal met?).
- **ReAct** (Yao et al. 2022): interleave reasoning + action (Thought/Act/Observation loop) — now a common pattern. **Reflexion** (Shinn et al. 2023): split into evaluator + self-reflection module; agent proposes new "trajectory" each step (e.g., code fails 1/3 tests → reflect → regenerate). Cheap to implement, big gains; downside = latency + token cost (thoughts/observations are token-heavy; many few-shot examples needed).

### Tool selection
- No foolproof guide. Literature ranges: **Toolformer** (5 tools, finetuned GPT-J), **Chameleon** (13 tools), **Gorilla** (1,645 APIs).
- More tools = more capability but harder to use + bloats context with descriptions. Use experimentation: compare tool sets; **ablation study** (drop a tool, measure perf drop — if none, remove it); spot tools the agent errs on; plot tool-call distribution. Chameleon: different tasks need different tools; different models have different tool preferences (GPT-4 wider set vs ChatGPT favoring image captioning).
- Tool creation: **Chameleon** tool-transition study (after tool X, how likely tool Y?) → combine frequently-paired tools. **Voyager** (Wang et al. 2023) skill manager → adds useful skills (coding programs) to a skill library for reuse.

## Agent failure modes & evaluation
- "Evaluation is about detecting failures." More complex task → more failure points.
- **Planning failures**: tool-use failures (invalid tool; valid tool/invalid params; valid tool/incorrect param values); goal failure (wrong outcome or ignores constraints — e.g., SF→Vietnam instead of India, or over budget); **time** as an overlooked constraint (late grant proposal = useless); reflection errors (agent insists task done when it isn't — assigns 40/50 people and claims success).
  - Eval method: planning dataset of (task, tool inventory); generate K plans/task; metrics: % valid plans; #plans to get a valid one; % valid tool calls; rates of invalid-tool / invalid-param / wrong-param-value calls.
- **Tool failures**: correct tool, wrong output (bad caption, bad SQL); translation errors (NL→command). Test each tool independently; print every tool call + output; benchmark the translator; detect missing-tool failures via domain experts.
- **Efficiency**: avg steps/task; avg cost/task; time per action. Compare to baseline (another agent or human) — but human vs AI efficiency differ (visiting 100 pages: slow for human, trivial for AI).

## Conclusion / forward pointers
- "Access to tools makes a model vastly more capable, so **the agentic pattern is inevitable.**"
- Agents build on long-standing LLM concepts: self-critique, chain-of-thought, structured outputs.
- Promises future posts on **evaluating agent frameworks** and on **memory systems** (agentic patterns deal with info exceeding context limits; a memory system enhances capability).
- Notes alignment with Anthropic's "Building Effective Agents" (Dec 2024) — "conceptually aligned, though with slightly different terminologies. However, Anthropic's post focuses on isolated patterns, whereas my post covers why and how things work. I also focus more on planning, tool selection, and failure modes."

Stake: Author of *AI Engineering* (O'Reilly, 2025) — this post markets/excerpts the book; practitioner-educator lens, no specific model/framework to sell (vendor-neutral). Now building in robotics.
