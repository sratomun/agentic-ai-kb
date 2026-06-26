---
type: concept
tags: [agents, embodied, robotics]
created: 2026-06-21
updated: 2026-06-22
census_count: 755
kind: domain
---

# Embodied & robotics agents

*Agents grounded in the physical world — robots and simulated embodiments that perceive, plan, and act, increasingly driven by LLM/VLM controllers.*

## What it is
Agents whose action space is physical: manipulation, navigation, and control in real or simulated environments, driven by multimodal models that map perception + language to actions. The dominant model class is now [[vla|Vision-Language-Action models]]; evaluation runs on embodied benchmarks like [[alfworld]] and [[scienceworld]].

## Why it matters
The bridge from digital agents to physical automation. Further from your enterprise knowledge-work focus, but it runs the *same* planning/tool/memory stack — so techniques cross-pollinate (RL-for-GUI and RL-for-robots are converging), and it's where "an agent that acts in the world" gets stress-tested under real physics.

## What the evidence shows
**2025 foundations.** The year built the evaluation and the model class. **EmbodiedBench** gave the field a vision-driven embodied benchmark (1,128 tasks from high-level household to low-level navigation/manipulation), exposing how far MLLM-based embodied agents lag (→ [[2025-02-13-arxiv-2502-09560v3-embodiedbench-comprehensive-benchmarking-multi-modal-large-language-models]]). **Magma** was the foundation-model bet — one model setting SOTA on *both* UI navigation and robotic manipulation via action-grounding + action-planning pretraining (→ [[2025-02-18-arxiv-2502-13130v1-magma-a-foundation-model-for-multimodal-ai-agents]]). By mid-year the frontier was **reason-then-act**: ThinkAct's dual-system design uses reinforced visual latent planning to let an MLLM reason before acting in physical environments (→ [[2025-07-22-arxiv-2507-16815v2-thinkact-vision-language-action-reasoning-via-reinforced-visual]]).
- Connective tissue with the rest of the radar: [[world-models]] (plan against a learned simulator) and [[vla]] (the model class) both feed embodied agents.

## Relationships
- model class: [[vla]]; planning via [[world-models]]
- benchmarks: [[alfworld]], [[scienceworld]]
- shares stack with [[multi-agent-systems]], [[agent-memory]]
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **172** · [[2025-02-13-arxiv-2502-09560v3-embodiedbench-comprehensive-benchmarking-multi-modal-large-language-models|EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for...]]
- **149** · [[2025-02-18-arxiv-2502-13130v1-magma-a-foundation-model-for-multimodal-ai-agents|Magma: A Foundation Model for Multimodal AI Agents]]
- **125** · [[2025-07-22-arxiv-2507-16815v2-thinkact-vision-language-action-reasoning-via-reinforced-visual|ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning]]
