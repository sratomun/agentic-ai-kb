# Template Bank: Entity Structure by Category

Use these three templates as reference patterns when normalizing wiki entities. Each shows the full frontmatter, title, one-liner, complete "What it is" and "Why it matters" sections, relationships structure, and canonical references where applicable.

---

## BENCHMARK TEMPLATE

Use this pattern for benchmarks, evaluation frameworks, and test suites.

### Frontmatter & Title

```
---
type: entity
entity_type: benchmark
tags: [agents, benchmark, <domain-tag>, <focus-tag>]
created: YYYY-MM-DD
updated: YYYY-MM-DD
census_count: N  # if mentioned in census
---

# <Benchmark Name>

<ONE-LINER: Phrase as "A/An ... for/that [verb] ...">
```

### What it is (2–3 paragraphs: mechanism, scope, variants, context)

**Pattern:** Start with the concrete measurement task, then expand to scope and positioning.

```
## What it is

<Paragraph 1: The core mechanism>
- What gets measured? (e.g., "function/tool-calling accuracy across N domains")
- How does it measure? (e.g., "provides pairs of sufficient lower- and higher-privilege tools; tests whether the agent picks the right one")
- Scale/coverage? (e.g., "X scenarios across Y domains")

<Paragraph 2 (if multi-faceted): Variants, dimensions, or categories>
- What are the recurring dimensions? (e.g., "5 risk types: Authority Escalation, Scope Expansion, Temporal Persistence, Safety Bypass, Data Over-Exposure")
- Key metrics reported? (e.g., "OPUR@k and PED")
- How does failure injection work? (e.g., "transient failures test premature escalation")

<Paragraph 3 (optional): Historical context or adoption>
- Where is it used? (e.g., "standard yardstick for tool-calling work in 2026")
- Evolution? (e.g., "versions through v3")
```

**Real example (ToolPrivBench):**
```
A benchmark for over-privileged tool selection — whether an agent picks or escalates to a higher-privilege tool despite an equally sufficient lower-privilege alternative. It comprises 544 scenarios across 8 application domains (Database and Business are largest) and 5 recurring risk types (Authority Escalation, Scope Expansion, Temporal Persistence, Safety Bypass, Data Over-Exposure). Each scenario provides both lower- and higher-privilege tools that are all independently sufficient, and injects transient failures to test premature escalation; it reports Over-Privileged Tool Use Rate (OPUR@k) and Pre-Escalation Exploration Depth (PED).
```

### Why it matters (1–2 paragraphs: significance + practical use case)

**Pattern:** Start with what gets unlocked, then address production constraints or gaps.

```
## Why it matters

<Paragraph 1: The research or production gap it fills>
- What's broken without it? (e.g., "agents don't generalize to new APIs")
- Why measure this specifically? (e.g., "tool selection directly maps to overprivilege risk in production")
- Who cares? (e.g., "enterprises need least-privilege guarantees")

<Paragraph 2 (optional): Scaling implication or decision point>
- What does this benchmark tell you about your model/agent?
- What's the hard choice you have to make now?
```

**Real example (BFCL):**
```
A widely-used function/tool-calling benchmark (versions through v3 in 2026) for measuring how reliably models select and invoke tools. Recurs across 2026 tool-use and agentic-RL work as the standard yardstick for tool-calling accuracy.
```

### Relationships

```
## Relationships
- evaluates [[concept-name]] (what this benchmark measures)
- relates to [[related-benchmark-or-concept]] (peer benchmarks or use cases)
- [optional] introduced by [[2026-XX-XX-arxiv-...-paper-title]] (if from a specific paper)

## Cited by
- [[paper-link-title]]
- [[paper-link-title]]

## Cited by (2025 deep notes)
- **count** · [[link-title]]
```

---

## FRAMEWORK TEMPLATE

Use this pattern for orchestration systems, platforms, and infrastructure libraries.

### Frontmatter & Title

```
---
type: entity
entity_type: framework
tags: [agents, framework, <domain>, <feature-tag>]
created: YYYY-MM-DD
updated: YYYY-MM-DD
census_count: N  # if mentioned in census
---

# <Framework Name>

<ONE-LINER: Phrase as "A/An ... for/that [verb] ...">
```

### What it is (2–4 paragraphs: design pattern, architecture, scope, positioning)

**Pattern:** Start with the abstraction offered, expand to scope and architectural choices.

```
## What it is

<Paragraph 1: The core abstraction and design decision>
- What does it model? (e.g., "multi-agent workflows as directed acyclic graphs")
- What primitives does it provide? (e.g., "nodes for agent decision-points, edges for message routing")
- Problem it solves? (e.g., "stateful orchestration of sequential and conditional agent steps")

<Paragraph 2: Scope and supported patterns>
- What patterns does it enable? (e.g., "sequential, branching, feedback-loop orchestration")
- How do agents interact? (e.g., "via a centralized message bus" vs. "peer-to-peer conversation loops")
- Deployment footprint? (e.g., "runs on serverless, single-machine, or distributed")

<Paragraph 3 (if production-grade): Architecture details and guarantees>
- Statefulness? (e.g., "preserves full execution trace for reproducibility")
- Observability? (e.g., "logs all messages and role transitions")
- Guardrails? (e.g., "optional policy enforcement at node boundaries")

<Paragraph 4 (optional): Positioning and adoption>
- Where does it fit in the ecosystem? (e.g., "one of the most-cited MAS frameworks in 2026")
- What populations use it? (e.g., "from research teams to enterprise back-office automation")
```

**Real example (POLARIS):**
```
A governed orchestration framework for enterprise back-office automation: typed plan synthesis (type-checked DAGs), rubric-guided plan selection, and compiled policy guardrails that block side effects before they occur — producing audit-grade artifacts and execution traces.
```

### Why it matters (1–2 paragraphs: unlock + production constraint)

**Pattern:** Start with what becomes possible, then highlight the specific advantage over alternatives.

```
## Why it matters

<Paragraph 1: What you can now build that was hard/impossible before>
- Research unlock? (e.g., "isolates orchestration logic from agent logic, speeding iteration")
- Production win? (e.g., "enterprises can deploy agents with policy compliance baked in")
- Adoption barrier lowered? (e.g., "developers no longer need to hand-code complex state machines")

<Paragraph 2 (optional): Tradeoff or positioning claim>
- When do you pick this vs. alternatives? (e.g., "if you need stateful loops, use LangGraph; if you need governance, use POLARIS")
- What's the tax? (e.g., "added latency from policy evaluation")
```

### Relationships

```
## Relationships
- framework for [[concept-name]] (e.g., multi-agent-systems, agentic-ai)
- relates to [[complementary-framework-or-protocol]] (peer abstractions)
- addresses [[problem-or-requirement]] (e.g., governance-gap)
- advances [[capability]] (e.g., agent-security)
- [optional] maker [[organization]] (if made by a known org)

## Cited by
- [[paper-link-title]]
```

---

## METHOD TEMPLATE

Use this pattern for algorithms, training recipes, evaluation techniques, and learned mechanisms.

### Frontmatter & Title

```
---
type: entity
entity_type: method
aliases: [<short-form-name>]  # optional
tags: [agents, method, <domain>, <capability>, <stage>]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# <Method Name>

*<ONE-LINER: Phrase as "[Verb phrase] — [short problem description]." (descriptive, not marketing)>*
```

### What it is (2–3 paragraphs: mechanism, scope, failure modes, variants)

**Pattern:** Start with the core algorithmic idea, then explain scope and failure modes. Use bulleted sub-clauses.

```
## What it is

<Paragraph 1: Core mechanism and intuition>
- Mechanism: [How does it work? e.g., "learns a scalar reward score from preference data (A > B)"]
- Where it fits: [Stage of pipeline, or type of problem e.g., "the engine inside [[rlhf]]"]
- Key insight: [One-sentence intuition, e.g., "decouples reasoning and tool-use into separate low-rank modules to avoid misaligned gradients"]

<Paragraph 2: Scope, variants, and failure modes>
- Scope: [What does it cover? e.g., "agentic-RL: teaches agents *when not to act*"]
- Variants or related work: [[alternate-method]], [[baseline]]
- Known failure modes: [e.g., "reward hacking" / "over-optimization"]
- How it avoids or addresses them: [e.g., "[[dpo]] sidesteps the explicit reward model"]

<Paragraph 3 (if empirical): Results and benchmarking>
- Benchmarks: [e.g., "restores Phi-4 14B from 0%→84.4% accuracy at 20 tools"]
- Metrics: [e.g., "52–57% token savings; 18–25% reduction in tool calls vs [[grpo]]"]
- Deployment: [e.g., "ships as zero-dependency TypeScript package"]
```

**Real example (SFT):**
```
Fine-tuning a pre-trained model on high-quality demonstration pairs (instructions and ideal responses, or distilled reasoning traces) so it follows instructions and adopts a format. It's stage one of the [[post-training]] recipe, before preference optimization and RL. Data quality dominates quantity — LIMA showed strong alignment from ~1,000 well-chosen examples.
```

**Real example (Reward Modeling):**
```
A reward model learns from preference data (A is better than B) to assign a scalar quality score, which an RL algorithm ([[ppo]], [[grpo]]) then maximizes. The recurring failure mode is *reward hacking* / over-optimization: the policy games the proxy reward instead of the true objective, a Goodhart's-law problem with its own scaling law. [[dpo]] sidesteps an explicit reward model ("your LM is secretly a reward model"); [[rlvr]] replaces it with verifiable rewards.
```

### Why it matters (1–2 paragraphs: unlock + alignment tradeoff)

**Pattern:** Start with what problem it solves, then state the production or research constraint.

```
## Why it matters

<Paragraph 1: What becomes possible or what gets unlocked>
- Research unlock: [e.g., "showed reasoning and tool-use induce misaligned gradients under joint optimization"]
- Practical win: [e.g., "highest-leverage, lowest-cost lever for teams that can't run full RL"]
- Adoption story: [e.g., "where most of the behavior you see in a chat model is installed"]

<Paragraph 2: The bottleneck or ceiling it exposes>
- What's now limiting? [e.g., "the quality and robustness of the reward signal is the real ceiling on alignment"]
- Scaling property: [e.g., "doesn't scale as cleanly as compute"]
- When do you care most? [e.g., "in production RL, reward hacking is now an observed phenomenon, not a theoretical worry"]
- Connection to security/safety: [ties to [[agent-security]] or [[alignment]]]
```

**Real example (SFT):**
```
SFT is where most of the *behavior* you see in a chat model is installed, and where distillation enters the pipeline (SFT a small model on a big model's outputs — see [[distillation]], [[synthetic-data]]). So what: it's the highest-leverage, lowest-cost lever for teams that can't run full RL — the 80/20 of post-training.
```

**Real example (Reward Modeling):**
```
The reward model is the alignment bottleneck: it's where human values enter the loop and where they get gamed. Reward hacking is now an observed production-RL phenomenon, not a theoretical worry, and it ties directly to [[agent-security]] (a model that games rewards games oversight). So what: the quality and robustness of the reward signal is the real ceiling on alignment, and it doesn't scale as cleanly as compute.
```

### Relationships

```
## Relationships
- method in [[capability-area]] (e.g., agentic-rl, post-training, llm-as-judge)
- stage of [[pipeline]] (e.g., post-training; precedes [[next-stage]])
- mechanism for [[application]] (e.g., distillation, synthetic-data)
- addresses [[problem]] (e.g., tool-use, agent-security)
- related to [[peer-method]], [[baseline-method]]
- [optional] studied by [[researcher-name]]

## Canonical references (queued for deep ingest)
- arXiv:XXXX.XXXXX · [Title] · YYYY
- arXiv:XXXX.XXXXX · [Title] · YYYY
- arXiv:XXXX.XXXXX · [Title] · YYYY

## Cited by
- [[paper-link-title]]
```

**Real example (SFT canonical references):**
```
## Canonical references (queued for deep ingest)
- arXiv:2203.02155 · InstructGPT (SFT is stage 1) · 2022
- arXiv:2305.11206 · LIMA: Less Is More for Alignment · 2023
- arXiv:2411.15124 · Tülu 3 · 2024
```

---

## Quick Checklist

When normalizing an entity against these templates:

### BENCHMARK
- [ ] One-liner describes what is measured (not why)
- [ ] "What it is" explains: mechanism → scope/variants → adoption context
- [ ] "Why it matters" explains: what gap it fills → practical constraint
- [ ] Relationships include what it measures (not just abstract concepts)
- [ ] Cited by section tracks papers that use this benchmark

### FRAMEWORK
- [ ] One-liner describes the abstraction it provides
- [ ] "What it is" explains: core abstraction → scope/patterns → architectural details
- [ ] "Why it matters" explains: what you can build → competitive positioning
- [ ] Relationships include the domain it supports (not just other frameworks)
- [ ] Census count populated if recurring in literature

### METHOD
- [ ] One-liner is in form "[Verb phrase] — [problem description]"
- [ ] "What it is" explains: mechanism → scope/variants → failure modes
- [ ] "Why it matters" explains: what unlock → what constraint or bottleneck
- [ ] "What it is" includes actual empirical results or metrics (not promises)
- [ ] Relationships show both what problem it solves and what it precedes
- [ ] Canonical references point to original/exemplar papers if known

