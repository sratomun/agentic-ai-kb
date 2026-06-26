---
type: concept
tags: [agents, open-models, foundation-models]
created: 2026-06-22
updated: 2026-06-22
kind: crosscutting
---

# Open Models

*Models whose weights (and often training tooling) are released openly, so anyone can run, fine-tune, and build agents on them without a closed API.*

## What it is
The open-weight side of the frontier-model split: families like Llama, Gemma, Mistral's open releases, Qwen, DeepSeek, and the tooling ecosystem around them. It borders [[agentic-rl]] (open RL environments to train open agents), [[coding-agents]] and [[tool-use]] (open models as the substrate harnesses run on), and the [[frontier-model-governance]] debate over whether open or closed wins. The contrast class is closed, API-only frontier models.

## Why it matters
For agents specifically, the open-vs-closed gap is now less about raw model quality and more about *infrastructure*: closed labs train models and harnesses "hand in glove," and the open ecosystem is racing to replicate that with shared training environments and agent-aware tooling. Whoever owns the open agent substrate (environments, hubs, CLIs) shapes where open agents can compete. So what: open models are the hedge against the access-fragmentation risk that closed, export-controlled frontier models create — worth tracking as a strategic option, not just a cost play.

## What the evidence shows
**Recent developments.** [[hugging-face|Hugging Face]]'s OpenEnv recasts open agentic-RL environments as a vendor-neutral standard so open models can be trained to use harnesses the way frontier models are → [[2026-06-08-blog-hugging-face-openenv-agentic-rl]]. [[mistral|Mistral]] and [[google|Google's]] Gemma sit on the open side while also building agent platforms on top. [[meta-ai|Meta AI]] is the Western standard-bearer for open-weight frontier models (Llama), though 2025–26 reporting describes traction struggles.

## Relationships
- substrate for [[agentic-rl]], [[coding-agents]], [[tool-use]]
- contested in [[frontier-model-governance]], [[debate-llms-path-to-agi]]
- championed by [[meta-ai]], [[hugging-face]], [[mistral]], [[google]]
- built via [[frontier-model-training]]; cheap to serve via [[mixture-of-experts]]; seeded by [[distillation]]
- heavy overlap with [[small-language-models]] (most SLMs ship open-weight)
- efficiency note: quantization (QLoRA/GPTQ — arXiv:2305.14314, arXiv:2210.17323) folded here as an open-weight inference concern, not a standalone node
