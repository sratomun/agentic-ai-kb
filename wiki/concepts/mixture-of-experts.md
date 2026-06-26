---
type: concept
tags: [agents, frontier-models, architecture, moe]
created: 2026-06-22
updated: 2026-06-22
kind: domain
---

# Mixture-of-Experts

*A sparse architecture where each token is routed to a few specialized expert sub-networks instead of the whole model — the design that lets labs scale total parameters without scaling per-token compute.*

## What it is
A model architecture that replaces dense feed-forward layers with many "expert" sub-networks plus a router that activates only a small subset per token. Total parameter count can be huge while *active* parameters per token stay small — e.g. DeepSeek-V3's 671B total / 37B active. The recurring engineering problem is load balancing (keeping experts evenly used without a separate loss that hurts quality). MoE is now the default for frontier open-weight models and a key reason they stay cheap to serve.

## Why it matters
MoE is how the open ecosystem reached frontier scale on a budget: you get the capability of a very large model at the inference cost of a much smaller one. For the exec that's the cost-curve story behind the open-vs-closed convergence — MoE is why GLM-4.5, Kimi K2, and DeepSeek can be both frontier-class and economically serveable, which directly shapes [[open-models]] competitiveness and agent unit economics.

## What the evidence shows
**Foundations.** The sparse-MoE layer was introduced by Shazeer et al. (arXiv:1701.06538), scaled via GShard (arXiv:2006.16668) and Switch Transformer to trillion-parameter sparsity (arXiv:2101.03961). The modern LLM lineage runs through Mixtral (arXiv:2401.04088), DeepSeekMoE's fine-grained expert specialization (arXiv:2401.06066), and DeepSeek-V3's auxiliary-loss-free load balancing (arXiv:2412.19437).

**Recent developments.** 2025 open-weight models converged on MoE as the default backbone → [[2025-12-30-blog-raschka-state-of-llms-2025]]; census model reports (GLM-4.5 at 355B/32B-active, Kimi K2 at ~1T/32B-active) show the pattern in production. These exemplars already have entity nodes: [[glm-45]], [[kimi-k2]], [[deepseek]].

## Relationships
- architecture for [[pretraining]]; cross-cuts [[frontier-model-training]]
- governed by [[scaling-laws]]; lowers serving cost for [[open-models]]
- exemplified by [[deepseek]], [[glm-45]], [[kimi-k2]]
- alternative efficiency route to [[small-language-models]] (sparse activation vs. smallness)
- explained by [[sebastian-raschka]]
- lowers cost-per-token feeding [[agent-finops]]

## Key papers (full-text ingested)
- [[2026-06-22-arxiv-1701-06538-sparsely-gated-moe|Sparsely-Gated MoE Layer]] — up to 137B params at ~6% of the compute; the origin point
- [[2026-06-22-arxiv-2006-16668-gshard|GShard]] — 600B MoE trained ~10x cheaper than the dense baseline
- [[2026-06-22-arxiv-2101-03961-switch-transformers|Switch Transformers]] — top-1 routing, 7x+ pretrain speedup; 1.57T-param Switch-C
- [[2026-06-22-arxiv-2401-04088-mixtral-of-experts|Mixtral of Experts]] — 47B total / 13B active (top-2 of 8), beats Llama-2-70B
- [[2026-06-22-arxiv-2401-06066-deepseekmoe|DeepSeekMoE]] — fine-grained + shared experts; matches dense quality at ~40% of compute
- [[2026-06-22-arxiv-2412-19437-deepseek-v3-technical-report|DeepSeek-V3]] — 671B/37B-active, auxiliary-loss-free load balancing
