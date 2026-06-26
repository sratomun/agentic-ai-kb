---
type: source
source_type: arxiv
title: "From Risk Classification to Action Plan Remediation: A Guardrail Feedback Driven Framework for LLM Agents"
authors: Yuhao Sun, Jiacheng Zhang, Shaanan Cohney, Zhexin Zhang et al.
url: https://arxiv.org/abs/2606.05805v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-security, tool-use, arxiv, auto-ingested]
---

# From Risk Classification to Action Plan Remediation: A Guardrail Feedback Driven Framework for LLM Agents

**arXiv:** [2606.05805v1](https://arxiv.org/abs/2606.05805v1) · 2026-06-04 · cs.AI
**Authors:** Yuhao Sun, Jiacheng Zhang, Shaanan Cohney, Zhexin Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based guardrails typically safeguard agents by evaluating proposed actions or inputs before execution, producing safety signals such as binary allow/deny decisions, risk categories, and/or explanatory rationales about potential policy violations. However, agent risks often arise when otherwise benign tasks are contaminated by untrusted external content, unsafe instructions, or risky tool use. Existing guardrails often flag the entire task uniformly as unsafe, thereby blocking the threat but sacrificing the benign part. Moreover, existing work largely evaluates guardrails in isolation, leaving unclear whether their interventions lead to safer downstream agent behavior. To address this, we introduce TRIAD (Tripartite Response for Iterative Agent Guardrailing), a guardrail-integrated agent framework that leverages guardrail-generated verbal feedback as a guiding signal to keep the agent aligned with benign objectives at each planning step. We finetune a language model on a self-curated training dataset to output one of three decisions: proceed, refuse, or update, together with structured natural-language feedback. Rather than merely allowing or blocking execution, update guides the agent to revise its plan, avoid harmful components, and preserve the benign task where possible. TRIAD injects this feedback into the agent's context, enabling subsequent plan revision and forming a closed loop between guardrail feedback and agent planning. Extensive experiments on ASB and AgentHarm show that TRIAD reduces the average attack success rate to 10.42%, while achieving the best safety-utility trade-off among guardrail-integrated baselines. Our code is available at: https://github.com/YUHAOSUNABC/TRIAD.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.05805v1)
