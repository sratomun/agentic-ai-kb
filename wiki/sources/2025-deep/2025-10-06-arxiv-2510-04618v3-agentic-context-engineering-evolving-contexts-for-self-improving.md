---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models"
authors: Qizheng Zhang, Changran Hu, Shubhangi Upasani, Boyuan Ma et al.
url: https://arxiv.org/abs/2510.04618v3
date: 2025-10-06
citationCount: 185
influentialCitationCount: 25
velocity: 21.74
ingested: 2026-06-22
tags: [finance-agents, self-evolving-agents, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models

**arXiv [2510.04618v3](https://arxiv.org/abs/2510.04618v3)** · 2025-10-06 · **185 citations** (25 influential · 21.74/mo) · Qizheng Zhang, Changran Hu, Shubhangi Upasani, Boyuan Ma et al.

## Abstract
Large language model (LLM) applications such as agents and domain-specific reasoning increasingly rely on context adaptation: modifying inputs with instructions, strategies, or evidence, rather than weight updates. Prior approaches improve usability but often suffer from brevity bias, which drops domain insights for concise summaries, and from context collapse, where iterative rewriting erodes details over time. We introduce ACE (Agentic Context Engineering), a framework that treats contexts as evolving playbooks that accumulate, refine, and organize strategies through a modular process of generation, reflection, and curation. ACE prevents collapse with structured, incremental updates that preserve detailed knowledge and scale with long-context models. Across agent and domain-specific benchmarks, ACE optimizes contexts both offline (e.g., system prompts) and online (e.g., agent memory), consistently outperforming strong baselines: +10.6% on agents and +8.6% on finance, while significantly reducing adaptation latency and rollout cost. Notably, ACE could adapt effectively without labeled supervision and instead by leveraging natural execution feedback. On the AppWorld leaderboard, ACE matches the top-ranked production-level agent on the overall average and surpasses it on the harder test-challenge split, despite using a smaller open-source model. These results show that comprehensive, evolving contexts enable scalable, efficient, and self-improving LLM systems with low overhead.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background and Motivation 2.1 Context Adaptation 2.2 Limitations of Existing Context Adaptation Methods Brevity Bias Context Collapse 3 Agentic Context Engineering (ACE) 3.1 Incremental Delta Updates 3.2 Grow-and-Refine 4 Results 4.1 Tasks and Datasets Evaluation Metrics 4.2 Baselines and Methods Base LLM In-Context Learning (ICL) ( agarwal2024many ) MIPROv2 ( opsahl2024optimizing ) GEPA ( agrawal2025gepa ) Dynamic Cheatsheet (DC) ( suzgun2025dynamic ) ACE (ours) 4.3 Results on Agent Benchmark Analysis: AppWorld 4.4 Results on Domain-Specific Benchmark Analysis: Finance Benchmark Analysis: Medical and Text-to-SQL Benchmark 4.5 Generalization across LLMs 4.6 Ablation Study and Sensitivity Analysis Ablation Study Robustness to Reflection Quality Sensitivity to Hyperparameter Choice 4.7 Cost and Speed Analysis Fine-Grained Cost Analysis KV Cache Reuse: Longer Context ≠ \neq Higher Serving Cost 5 Discussion Implications for Online and Continual Learning Limitations and Ch…

**Method / approach.** Methods Brevity Bias Context Collapse 3 Agentic Context Engineering (ACE) 3.1 Incremental Delta Updates 3.2 Grow-and-Refine 4 Results 4.1 Tasks and Datasets Evaluation Metrics 4.2 Baselines and Methods Base LLM In-Context Learning (ICL) ( agarwal2024many ) MIPROv2 ( opsahl2024optimizing ) GEPA ( agrawal2025gepa ) Dynamic Cheatsheet (DC) ( suzgun2025dynamic ) ACE (ours) 4.3 Results on Agent Benchmark Analysis: AppWorld 4.4 Results on Domain-Specific Benchmark Analysis: Finance Benchmark Analysis: Medical and Text-to-SQL Benchmark 4.5 Generalization across LLMs 4.6 Ablation Study and Sensitivity Analysis Ablation Study Robustness to Reflection Quality Sensitivity to Hyperparameter Choice 4.7 Cost and Speed Analysis Fine-Grained Cost Analysis KV Cache Reuse: Longer Context ≠ \neq Higher Serving Cost 5 Discussion Implications for Online and Continual Learning Limitations and Challenges References…

**Results.** experimenting, reflecting, and consolidating, while avoiding the bottleneck of overloading a single model with all responsibilities. Figure 4: The ACE Framework. Inspired by Dynamic Cheatsheet, ACE adopts an agentic architecture with three specialized components: a Generator, a Reflector, and a Curator. To address the limitations of prior methods discussed in § 2.2 (notably brevity bias and context collapse ) ACE introduces three key innovations: (1) a dedicated Reflector that separates evaluation and insight extraction from curation, improving context quality and downstream performance (§ 4.6 ); (2) incremental delta updates (§ 3.1 ) that replace costly monolithic rewrites with localized edits, reducing both latency and compute cost (§ 4.7 ); and (3) a grow-and-refine mechanism (§ 3.2 ) that balances steady context expansion with redundancy control. As shown in Figure 4 , the workflow begins with the Generator producing reason…

**Conclusion.** Discussion Implications for Online and Continual Learning Limitations and Challenges References A Extended Results A.1 Generalization across Different LLMs Analysis A.2 Beyond Finance: Additional Domain Tasks Analysis A.3 Fine-Grained Cost Analysis Adaptation Stage Evaluation Stage A.4 Robustness to Reflection Quality Using Weaker Reflector Models Robustness to Noisy or Harmful Reflector Feedback Takeaway and Mitigation A.5 Ablation on Incremental Context Update A.6 Sensitivity Analysis on Hyperparameter Choice Reflection Iterations Deduplication Threshold Pruning Trigger (Maximum Context Length) B Extended Related Work B.1 Agent Memory C Extended Discussions C.1 AC…

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.04618v3.md` · `raw/arxiv/2510.04618v3.fulltext.md`
