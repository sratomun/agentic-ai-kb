---
type: concept
tags: [agents, small-language-models, on-device, edge, efficiency]
created: 2026-06-23
updated: 2026-06-23
kind: domain
census_count: 30
---

# On-Device Agents

*Running agents locally — on phones, laptops, consumer GPUs, and edge hardware — instead of round-tripping every call to a cloud LLM API. The deployment surface where [[small-language-models]] actually earn their keep.*

## What it is
The slice of the agent stack that executes inference (and increasingly fine-tuning) on the user's own device or at the network edge, rather than on centralized cloud infrastructure. It spans on-device GUI/mobile agents, edge inference systems, in-flash and memory-efficient serving, quantized KV-cache handoff, and on-device fine-tuning. It's the practical consequence of [[small-language-models]] — a model only matters on-device if it's small enough to fit — and it borders [[computer-use-agents]] (the GUI/mobile agents that increasingly run locally) and [[post-training]] (on-device fine-tuning).

## Why it matters
On-device is where the SLM economics turn into product properties the exec cares about: **lower latency, offline operation, and data never leaving the device** — the privacy and compliance story that cloud LLMs structurally can't offer. The same 10–30× inference saving that makes small models cheap also makes them deployable on hardware people already own, which collapses both per-call cost and the data-governance surface. The strategic read: for any agent that touches sensitive data or needs to work without a network, on-device isn't a downgrade — it's the differentiator, and it's a place incumbents with cloud-revenue commitments are slow to move.

## What the evidence shows
**Foundations.** The anchor case is made in Belcak et al. (→ [[2025-06-02-arxiv-2506-02153v2-small-language-models-are-the-future-of-agentic|SLMs are the Future of Agentic AI]]): on-device inference systems like ChatRTX already run SLMs locally on consumer-grade GPUs for real-time, offline agentic inference with stronger data control; serving systems (PowerInfer on a consumer GPU, PowerInfer-2 on a smartphone) and edge-oriented inference schedulers (NVIDIA Dynamo) make low-latency local serving practical. The paper frames edge deployment as a core *flexibility* advantage of small models, not a compromise — the 10–30× cost gap holds in latency, energy, and FLOPs.

**Recent developments.** The 2026 corpus turns this into engineering across four fronts. On-device **GUI/mobile agents** matured — building small on-device GUI agents (→ [[2025-09-30-arxiv-2509-26539v1-ferret-ui-lite-lessons-from-building-small-on-device-gui-agents|Ferret-UI Lite]]), accelerating mobile GUI inference via online exploration (→ [[2025-11-27-arxiv-2511-22138v1-tinyllm-evaluation-and-optimization-of-small-language-models-for-agent|TinyLLM on edge]], → [[2026-05-26-arxiv-2605-26546v1-mobileexplorer-accelerating-on-device-inference-for-mobile-gui-agents|MobileExplorer]]). **Serving / systems** pushed the hardware envelope — DRAM-free in-flash inference (→ [[2025-12-03-arxiv-2512-03608v1-kvnand-efficient-on-device-large-language-model-inference-using-dram-f|KVNAND]]), quantized KV-cache handoff across on-device agents (→ [[2026-05-05-arxiv-2605-03884v1-qkvshare-quantized-kv-cache-handoff-for-multi-agent-on-device-llms|QKVShare]]), and full-pipeline acceleration (→ [[2026-05-11-arxiv-2605-10380v1-agent-x-full-pipeline-acceleration-of-on-device-ai-agents|Agent-X]]). **On-device fine-tuning / adaptation** became feasible — mobile-native fine-tuning (→ [[2025-12-09-arxiv-2512-08211v2-mobilefinetuner-a-mobile-native-framework-for-on-device-llm-fine-tunin|MobileFineTuner]]), backprop-free zeroth-order optimization (→ [[2025-11-14-arxiv-2511-11362v2-on-device-fine-tuning-via-backprop-free-zeroth-order-optimization|on-device ZO fine-tuning]]), and 1-bit quantized edge RL (→ [[2026-04-27-arxiv-2604-24273v1-bitrl-reinforcement-learning-with-1-bit-quantized-language-models-for|BitRL]]). And a **hybrid local↔cloud** pattern recurs — splitting work between on-device small models and cloud LLMs (→ [[2025-02-06-arxiv-2502-04392v1-division-of-thoughts-harnessing-hybrid-language-model-synergy-for-effi|Division-of-Thoughts]]), with adaptive on-device context management (→ [[2025-09-24-arxiv-2511-03728v1-efficient-on-device-agents-via-adaptive-context-management|adaptive context management]]).

**Caveat.** Local execution moves the attack surface onto the device: on-device mobile agents are vulnerable to environmental injection (→ [[2025-10-23-arxiv-2510-20333v3-ghostei-bench-do-mobile-agents-resilience-to-environmental-injection-i|GhostEI-Bench]]), so the privacy win comes with a new [[agent-security]] surface, not fewer risks overall.

## Relationships
- deployment surface for [[small-language-models]] (the parent economics) and [[mixture-of-experts]] (sparse models also target edge serving)
- overlaps [[computer-use-agents]] (GUI/mobile agents, increasingly local) and [[recommendation-agents]] (on-device personalization)
- on-device fine-tuning is a branch of [[post-training]]; quantization folded in here as an edge-serving concern
- introduces a device-side [[agent-security]] surface (environmental injection)
- exemplar hardware/vendors: [[nvidia]] (ChatRTX, Dynamo), small models [[phi]], [[smollm]], [[nemotron]]

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. -->
- **35** · 2.1/mo · [[2025-02-06-arxiv-2502-04392v1-division-of-thoughts-harnessing-hybrid-language-model-synergy-for-effi|Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for…]]
- **8** · 1.0/mo · [[2025-10-23-arxiv-2510-20333v3-ghostei-bench-do-mobile-agents-resilience-to-environmental-injection-i|GhostEI-Bench: Do Mobile Agents Resilience to Environmental Inject…]]
- **8** · 0.9/mo · [[2025-09-30-arxiv-2509-26539v1-ferret-ui-lite-lessons-from-building-small-on-device-gui-agents|Ferret-UI Lite: Lessons from Building Small On-Device GUI Agents]]
- **5** · 0.6/mo · [[2025-10-21-arxiv-2510-18546v3-efficientnav-towards-on-device-object-goal-navigation-with-navigation|EfficientNav: Towards On-Device Object-Goal Navigation with Naviga…]]
- **3** · 0.4/mo · [[2025-11-27-arxiv-2511-22138v1-tinyllm-evaluation-and-optimization-of-small-language-models-for-agent|TinyLLM: Evaluation and Optimization of Small Language Models for …]]
- **3** · 0.4/mo · [[2025-11-05-arxiv-2511-03370v3-eq-negotiator-dynamic-emotional-personas-empower-small-language-models|EQ-Negotiator: Dynamic Emotional Personas Empower Small Language M…]]
- **2** · 0.2/mo · [[2025-10-01-arxiv-2510-01427v3-small-language-model-agents-enable-efficient-and-high-quality-knowledg|Small Language Model Agents Enable Efficient and High-Quality Know…]]
- **2** · 0.2/mo · [[2025-09-12-arxiv-2509-10436v2-refactorcoderqa-benchmarking-llms-for-multi-domain-coding-question-sol|RefactorCoderQA: Benchmarking LLMs for Multi-Domain Coding Questio…]]
