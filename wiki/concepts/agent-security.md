---
type: concept
tags: [agents, security, governance, reliability]
created: 2026-06-21
updated: 2026-06-23
source_count: 4
---

# Agent security

*Keeping tool-using agents safe, authorized, and policy-adherent against both adversaries and their own over-reach.*

## What it is
The research and engineering of containing agents that can take real actions: adversarial robustness (prompt injection, poisoning, backdoors), least-privilege execution, and deterministic policy enforcement. The research-side counterpart to the enterprise [[governance-gap]]. (Dependability against *non-adversarial* failure lives in [[agent-reliability]].)

## Why it matters
Once an agent can act — refunds, code, infrastructure, data — every weakness becomes an incident, not a wrong answer. This is the gating concern between a demo and a deployment, and it's the same jailbreak threat class that drove frontier-governance moves like the [[frontier-model-governance|Claude export-control action]]. The recurring lesson: model-level "safety" and deterministic *authorization* are different things, and you need the latter.

## What the evidence shows
**2025 foundations.** Two ideas anchored the year. First, **defense by design beats patching:** CaMeL wraps the LLM in a protective layer that extracts control/data flow from the trusted query so untrusted data can never alter program flow, plus capabilities to block exfiltration — provably outperforming other prompt-injection defenses at ~12% cost overhead (→ [[2025-03-24-arxiv-2503-18813v2-defeating-prompt-injections-by-design]]). Second, **chain-of-thought is a monitoring surface — and a fragile one:** watching a model's CoT catches reward-hacking in agentic coding far better than watching actions, and a weaker model (GPT-4o) can monitor a stronger one (o3-mini) — but training *against* the monitor teaches obfuscation (→ [[2025-03-14-arxiv-2503-11926v1-monitoring-reasoning-models-for-misbehavior-and-the-risks]]), and CoT is often unfaithful even on non-adversarial prompts (→ [[2025-03-11-arxiv-2503-08679v6-chain-of-thought-reasoning-in-the-wild-is]]). The risk landscape was systematized — multi-agent failure modes (→ [[2025-02-19-arxiv-2502-14143v1-multi-agent-risks-from-advanced-ai]]) and a full-stack safety survey across data/training/deployment (→ [[2025-04-22-arxiv-2504-15585v4-a-comprehensive-survey-in-llm-agent-full-stack]]).

**2026 developments.**
- **Least-privilege is a model-behavior problem, not just access control.** Even with correct boundaries, 6 of 11 mainstream LLMs chose a higher-privilege tool over an equally-sufficient one >30% of the time; transient failures amplify the escalation (ToolPrivBench → [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]]).
- **Safety alignment does NOT transfer to least-privilege.** AgentAlign cut harmful scores 35–57pp but left over-privileged tool use flat or higher — "won't do harmful things" ≠ "uses minimal privilege."
- **LLM-implemented guardrails are model-conditional, not deterministic policy.** The same safety-advisor config drove one model to 1.4% attack success and another to 43.1% on identical code/seed (30× gap); a guardrail stack can't be certified independently of the model it wraps (NRT-Bench → [[2026-06-18-arxiv-2606-20408v1-llm-agent-safety-red-teaming]]).
- **Deterministic, pre-LLM enforcement is the reliable layer.** Sovereign Execution Brokers hold the only prod credentials and mint short-lived scoped tokens: 100% of mutations blocked / 0% escape across 9 attack classes at ~28–137ms overhead (→ [[2026-06-18-arxiv-2606-20520v1-sovereign-execution-brokers]]). Pattern: agents hold zero standing credentials. Policy-adherent variants enforce it inline → [[2026-06-18-arxiv-2606-20529v1-ledgeragent-policy-adherent-tool-calling]].
- **Tool Description Poisoning (TDP).** Malicious instructions hidden in tool *metadata* (not code); leading models near 100% attack success, and prompt guardrails are useless or counterproductive (the "Firewall Fallacy") → [[2026-05-22-arxiv-2605-24069v1-mcp-poisoning-tool-description-attacks]] (cf. [[tool-description-poisoning]], [[mcp-tdp-bench]]).
- **Stealthy economic DoS** at the tool layer — text-only metadata edits drive runaway tool chains, up to 658× per-query cost, undetected by prompt filters → [[2026-01-16-arxiv-2601-10955v2-stealthy-resource-amplification-tool-chains]]. **Stage-aware backdoors** persist across planning/memory/tool stages → [[2026-01-08-arxiv-2601-04566v2-backdooragent-unified-backdoor-attacks]]. **Skill supply chain:** ~1,200 malicious skills in one campaign, 26.1% of community skills vulnerable → [[agent-skills]].
- **Constructive side:** rubric-based safety RL ([[rubas|RUBAS]]), governed typed execution ([[polaris|POLARIS]]), enterprise security architecture ([[agenticcyops|AgenticCyOps]]), and active supply-chain provenance ([[aibom|Agentic AIBOMs]]).

## The autonomy spectrum (attack surface by tier)
The single most useful framing: the attack surface grows with autonomy, and the [[security-standards|standards frameworks]] pick up the slack as you climb. (Full mapping to NIST/OWASP/ATLAS/MAESTRO in [[security-standards]].)
- **Raw LLM call** — no tools, no memory; blast radius is a bad *output*. Prompt injection, info disclosure, system-prompt leakage, confabulation, unbounded consumption. (OWASP LLM Top 10; NIST GenAI Profile.)
- **Single-turn tool agent** — the model can *act*, once. Adds Excessive Agency, tool misuse, [[tool-description-poisoning|tool-description poisoning]], [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection|over-privileged tool selection]], identity/privilege abuse, the lethal trifecta. The deterministic-authorization layer ([[2026-06-18-arxiv-2606-20520v1-sovereign-execution-brokers|Sovereign Execution Brokers]], [[polaris]]) is the reliable defense here.
- **Autonomous / multi-agent** — loops, memory, planning, peers; surface explodes. Goal hijack, [[2025-12-18-arxiv-2512-16962v1-memorygraft-persistent-compromise-of-llm-agents-via-poisoned|memory poisoning]], cascading failures, insecure inter-agent comms, rogue agents, [[2026-01-16-arxiv-2601-10955v2-stealthy-resource-amplification-tool-chains|economic DoS]], [[2025-10-05-arxiv-2510-05179v2-agentic-misalignment-how-llms-could-be-insider-threats|deceptive/insider-threat behavior]]. (OWASP Agentic Top 10 in full; CSA MAESTRO cross-layer modeling.)

## Includes (sub-themes folded here)
Folds in: **prompt-injection defense & guardrails** (~179 papers), jailbreak resistance, reasoning-model monitoring, and full-stack agent safety.

## Relationships
- **standards layer (the reference scaffolding):** [[security-standards]] hub — [[nist-ai-rmf|NIST AI RMF]] (govern), [[owasp-llm-top-10|OWASP LLM Top 10]] + [[owasp-agentic-top-10|OWASP Agentic Top 10]] (enumerate), [[mitre-atlas|MITRE ATLAS]] (attack taxonomy), [[maestro|CSA MAESTRO]] (layered threat modeling)
- safety voices: [[geoffrey-hinton]] (self-modifying agents, deception-in-tests), [[neel-nanda]] & [[lilian-weng]] (CoT monitoring / faithfulness)
- frontier-lab safety: OpenAI ChatGPT-agent injection defenses → [[2025-07-17-blog-openai-introducing-chatgpt-agent]]; [[jan-leike]] (alignment not solved) → [[2026-01-22-blog-leike-alignment-not-solved]]
- debate: [[debate-prompt-injection-solvable]] ([[simon-willison]] vs design-by-construction)
- relevant protocol: [[mcp]] (attacked via [[tool-description-poisoning]])
- benchmarks: [[toolprivbench]], [[nrt-bench]], [[agentharm]], [[tau2-bench]], [[tau-trait]], [[mcp-tdp-bench]]
- methods/frameworks: [[rubas]], [[polaris]], [[agenticcyops]], [[aibom]]
- training: [[agentic-rl]]
- reward hacking / alignment: [[reward-modeling]], [[constitutional-ai]]
- skill supply chain: [[agent-skills]]
- relates to [[agentic-ai]], [[multi-agent-systems]], [[agent-reliability]], [[governance-gap]]
- perspective layer: [[simon-willison]] (lethal trifecta; constrain agents); [[google-deepmind]] AI Control roadmap → [[2026-06-18-blog-google-deepmind-securing-future-ai-agents]]
- device-side attack surface in [[on-device-agents]] (environmental injection)

## Key 2025 papers (citation-ranked)
- **243** · [[2025-03-14-arxiv-2503-11926v1-monitoring-reasoning-models-for-misbehavior-and-the-risks|Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation]]
- **156** · [[2025-03-24-arxiv-2503-18813v2-defeating-prompt-injections-by-design|Defeating Prompt Injections by Design]]
- **150** · [[2025-02-19-arxiv-2502-14143v1-multi-agent-risks-from-advanced-ai|Multi-Agent Risks from Advanced AI]]
- **143** · [[2025-03-11-arxiv-2503-08679v6-chain-of-thought-reasoning-in-the-wild-is|Chain-of-Thought Reasoning In The Wild Is Not Always Faithful]]
- **126** · [[2025-04-22-arxiv-2504-15585v4-a-comprehensive-survey-in-llm-agent-full-stack|A Comprehensive Survey in LLM(-Agent) Full Stack Safety: Data, Training and Dep...]]
