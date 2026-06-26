---
type: entity
entity_type: org
aliases: [Hugging Face, HF, 🤗]
tags: [agents, org, open-models]
created: 2026-06-22
updated: 2026-06-22
url: https://huggingface.co/
---

# Hugging Face

*The hub and tooling layer of the open-model ecosystem — models, datasets, Spaces, and increasingly the open infrastructure for *training* and *running* agents.*

## What it is
The de-facto commons for open ML: model/dataset/Spaces hosting plus the libraries (`transformers`, `huggingface_hub`/`hf` CLI, TRL, smolagents) developers build on. In 2025–26 HF has leaned hard into agents specifically — stewarding **OpenEnv** (an open interoperability layer for agentic-RL environments), shipping computer-use and robotics agent work, and re-tooling its own developer surfaces (the `hf` CLI) for coding agents as first-class users.

## Why it matters
HF is the open-source counterweight to the closed labs' agent moat. Its [[2026-06-08-blog-hugging-face-openenv-agentic-rl|OpenEnv]] play targets exactly the bottleneck that keeps open models behind — the *environments* agents train in — and makes [[mcp|MCP]] a first-class citizen in the training loop, not just inference. Its [[2026-06-04-blog-hugging-face-hf-cli-for-agents|hf-CLI benchmark]] is a rare *measured* look at how agents consume tools (and quietly confirms Claude Code and Codex as the dominant [[coding-agents]] by Hub traffic). So what: HF is the place to watch whether the open stack can keep pace on agents, and a source of transferable patterns (agent-aware tooling, open RL environments).

## Relationships
- stewards OpenEnv (open [[agentic-rl]] environment standard) → [[2026-06-08-blog-hugging-face-openenv-agentic-rl]]
- builds the `hf` CLI for [[coding-agents]] → [[2026-06-04-blog-hugging-face-hf-cli-for-agents]]
- central to [[open-models]]
- uses [[mcp]] (first-class in OpenEnv)
- collaborates with [[meta-ai]] (Meta-PyTorch), [[nvidia]] on OpenEnv
- competes-with-and-hosts a wide range of model makers

## Perspective (blog-scanner)
- **"The Open Source Community is backing OpenEnv for Agentic RL"** (Jun 2026): OpenEnv recast as a vendor-neutral protocol layer ("common socket") for RL environments, governed by a multi-org committee; MCP first-class → [[2026-06-08-blog-hugging-face-openenv-agentic-rl]].
- **"Designing the hf CLI as an agent-optimized way to work with the Hub"** (Jun 2026): agent-aware CLI output, next-command rails; benchmark shows curl/SDK burn up to 6x the tokens on multi-step tasks → [[2026-06-04-blog-hugging-face-hf-cli-for-agents]].

### Other agent-relevant 2025–26 posts (enumerated, not deep-captured)
- **Holo3.1: Fast & Local Computer Use Agents** (Hcompany, Jun 2026) — [[computer-use-agents]].
- **Adding MCP Tools to Reachy Mini** (Jun 2026) — [[mcp]], [[embodied-agents]] (LeRobot/Reachy).
- **How an Agent Built a 3D Paris Gallery by Chaining Two HF Spaces** (Jun 2026) — agent tool/Spaces chaining.
- **OpenEnv in Practice: Evaluating Tool-Using Agents in Real-World Environments** (Feb 2026) — [[agent-evaluation]], [[tool-use]].
- **Building the Open Agent Ecosystem Together: Introducing OpenEnv** (Oct 2025) — origin post for OpenEnv.
- **Say hello to `hf`: a faster, friendlier Hugging Face CLI** (Jul 2025) — predecessor to the agent-CLI work.
- (smolagents — HF's lightweight code-first agent library — is the recurring framework underneath much of this; promote to its own node if it recurs.)
