---
type: concept
tags: [agents, frontier-models, training, supply-side]
created: 2026-06-22
updated: 2026-06-22
kind: hub
---

# Frontier Model Training

*The supply-side pipeline that produces a frontier model: data → pre-training → post-training → distillation, plus the compute and scaling that govern all of it. The thing agents run on top of.*

## What it is
The end-to-end recipe a frontier lab runs to turn raw data and compute into a deployable model. The spine has four stages — assemble and curate [[pretraining-data|data]] (and increasingly [[synthetic-data|synthesize]] it), run [[pretraining]] to get a base model, apply [[post-training]] (SFT → preference optimization → RL) to make it useful and aligned, and optionally [[distillation|distill]] the large model into smaller deployable ones. Two cross-cutting forces shape every stage: [[scaling-laws]] (how capability tracks compute/data/params) and architecture choices like [[mixture-of-experts]]. This hub is the **supply-side mirror of [[agentic-ai]]**: that hub covers what you build *with* a model; this one covers how the model is *made*.

## Why it matters
For the exec the load-bearing question is **where capability actually comes from** — base model vs. post-training vs. the agent scaffold — because it dictates where to invest. The 2025–26 shift is that the marginal gains moved downstream: pre-training scaling is hitting diminishing returns, and the action is in post-training (reasoning RL) and distillation. Knowing the pipeline is also how you read the strategic map: who controls data, compute, and the post-training recipe is who controls the frontier, and that's the layer export controls and the open-vs-closed split actually target.

## What the evidence shows
**Foundations.** The pipeline as a named, reproducible recipe crystallized around the DeepSeek-R1 release — a base model put through a multi-stage post-training process (cold-start SFT → RL → distillation to small models) that an outsider could follow → [[2025-01-21-blog-lambert-deepseek-r1-recipe]]. The four post-training routes (RL-only, SFT+RL, pure SFT/distill) are laid out in [[2025-02-05-blog-raschka-understanding-reasoning-llms]].

**Recent developments.** The 2025 retrospective view is that progress shifted from training-side scaling toward inference-time scaling and post-training, with open-weight models converging on [[mixture-of-experts]] architectures → [[2025-12-30-blog-raschka-state-of-llms-2025]]. The three-year arc from GPT-3 to frontier reasoners is traced in [[2025-11-18-blog-mollick-three-years-from-gpt-3-to-gemini]].

## Includes (sub-themes folded into stage nodes)
- **Data:** [[pretraining-data]] (absorbs data curation, dedup, mixtures), [[synthetic-data]], [[tokenization]]
- **Pre-training:** [[pretraining]], [[scaling-laws]], [[mixture-of-experts]]
- **Post-training:** [[post-training]] (hub over [[sft]], [[rlhf]], [[dpo]], [[ppo]], [[grpo]], [[rlvr]], [[reward-modeling]], [[constitutional-ai]])
- **Compression:** [[distillation]] (quantization folded into [[open-models]] efficiency; training-compute folded into [[nvidia]]/[[vera-rubin]])

## Relationships
- produces the base models behind [[reasoning-models]], [[agentic-ai]]
- parent hub of [[pretraining]], [[pretraining-data]], [[synthetic-data]], [[scaling-laws]], [[mixture-of-experts]], [[post-training]], [[distillation]]
- contested in [[open-models]], [[frontier-model-governance]]
- compute supplied by [[nvidia]], [[vera-rubin]]
- explained by [[sebastian-raschka]], [[nathan-lambert]]

## Key papers (full-text ingested)
- [[2020-05-28-arxiv-2005-14165-gpt3-few-shot-learners|GPT-3: Language Models are Few-Shot Learners]] — scale unlocks few-shot capability (175B params)
- [[2022-03-04-arxiv-2203-02155-instructgpt|InstructGPT]] — the SFT→RM→RL alignment recipe; 1.3B aligned beats 175B base
- [[2026-06-22-arxiv-2412-19437-deepseek-v3-technical-report|DeepSeek-V3 Technical Report]] — modern MoE pretraining (671B/37B-active, 14.8T tokens)
- [[2026-06-22-arxiv-2501-12948-deepseek-r1|DeepSeek-R1]] — open, legible multi-stage post-training recipe
- [[2024-11-22-arxiv-2411-15124-tulu-3|Tülu 3]] — open post-training blueprint (SFT+DPO+RLVR)
