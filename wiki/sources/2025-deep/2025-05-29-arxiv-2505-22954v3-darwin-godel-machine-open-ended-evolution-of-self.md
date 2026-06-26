---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents"
authors: Jenny Zhang, Shengran Hu, Cong Lu, Robert Lange et al.
url: https://arxiv.org/abs/2505.22954v3
date: 2025-05-29
citationCount: 122
influentialCitationCount: 6
velocity: 9.55
ingested: 2026-06-22
tags: [coding-agents, human-agent-interaction, self-evolving-agents, agent-security, agent-evaluation, arxiv, 2025, cited]
---

# Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents

**arXiv [2505.22954v3](https://arxiv.org/abs/2505.22954v3)** · 2025-05-29 · **122 citations** (6 influential · 9.55/mo) · Jenny Zhang, Shengran Hu, Cong Lu, Robert Lange et al.

## Abstract
Today's AI systems have human-designed, fixed architectures and cannot autonomously and continuously improve themselves. The advance of AI could itself be automated. If done safely, that would accelerate AI development and allow us to reap its benefits much sooner. Meta-learning can automate the discovery of novel algorithms, but is limited by first-order improvements and the human design of a suitable search space. The Gödel machine proposed a theoretical alternative: a self-improving AI that repeatedly modifies itself in a provably beneficial manner. Unfortunately, proving that most changes are net beneficial is impossible in practice. We introduce the Darwin Gödel Machine (DGM), a self-improving system that iteratively modifies its own code (thereby also improving its ability to modify its own codebase) and empirically validates each change using coding benchmarks. Inspired by Darwinian evolution and open-endedness research, the DGM maintains an archive of generated coding agents. It grows the archive by sampling an agent from it and using a foundation model to create a new, interesting, version of the sampled agent. This open-ended exploration forms a growing tree of diverse, high-quality agents and allows the parallel exploration of many different paths through the search space. Empirically, the DGM automatically improves its coding capabilities (e.g., better code editing tools, long-context window management, peer-review mechanisms), increasing performance on SWE-bench from 20.0% to 50.0%, and on Polyglot from 14.2% to 30.7%. Furthermore, the DGM significantly outperforms baselines without self-improvement or open-ended exploration. All experiments were done with safety precautions (e.g., sandboxing, human oversight). The DGM is a significant step toward self-improving AI, capable of gathering its own stepping stones along paths that unfold into endless innovation.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Darwin Gödel Machine 4 Experiments 4.1 Experiment Setup 4.2 Benchmarks 4.3 Baselines 4.4 Results 5 Safety Discussion 6 Conclusion and Limitations References A Additional Results A.1 Baselines on SWE-bench A.2 Generality across models on Polyglot A.3 Ablation of Parent Selection A.4 Additional Statistics of DGM runs B Additional Related Work C Algorithmic Details C.1 Initial Coding Agent C.2 Parent Selection C.3 Self-Improve Prompts C.4 Pseudocode D Experiment Details D.1 Hyperparameters for Foundation Models E Benchmark Details E.1 Cost Estimate E.2 SWE-bench Tasks E.3 Polyglot Tasks E.4 SWE-bench State-of-The-Art E.5 Polyglot Representative Agent F Best-Discovered Agents F.1 DGM on SWE-bench F.2 DGM on Polyglot G Similar Target Functionality, Different Implementations H Case Study: Solving Hallucination I Additional Safety Discussion J Additional Future Work Directions License: CC BY 4.0 arXiv:2505.22954v3 [cs.AI] 12 Mar 2026 1 1 footnotetext: co-firs…

**Method / approach.** method, on the other hand, is a cumulative and open-ended system, where each innovation builds upon previous artifacts, enabling future discoveries. There is growing hope that the current manual process of advancing AI could itself be automated. If done safely, such automation would accelerate AI development and allow us to reap its benefits much sooner. This prospect raises the question of how AI systems can endlessly improve themselves while getting better at solving relevant problems. Meta-learning can automate the discovery of novel algorithms, but is limited by first-order improvements and the human design of a suitable search space. The Gödel machine (Schmidhuber, 2007 ) proposed a theoretical alternative: a self-improving AI that repeatedly modifies itself in a provably beneficial manner. Unfortunately, proving that most changes are net beneficial is impossible in practice. We introduce the Darwin Gödel Machine (DGM), a novel self-improving system that iteratively modifies its…

**Results.** Experiments 4.1 Experiment Setup 4.2 Benchmarks 4.3 Baselines 4.4 Results 5 Safety Discussion 6 Conclusion and Limitations References A Additional Results A.1 Baselines on SWE-bench A.2 Generality across models on Polyglot A.3 Ablation of Parent Selection A.4 Additional Statistics of DGM runs B Additional Related Work C Algorithmic Details C.1 Initial Coding Agent C.2 Parent Selection C.3 Self-Improve Prompts C.4 Pseudocode D Experiment Details D.1 Hyperparameters for Foundation Models E Benchmark Details E.1 Cost Estimate E.2 SWE-bench Tasks E.3 Polyglot Tasks E.4 SWE-bench State-of-The-Art E.5 Polyglot Representative Agent F Best-Discovered Agents F.1 DGM on SWE-bench F.2 DGM on Polyglot G Similar Target Functionality, Different Implementations H Case Study: Solving Hallucination I Additional Safety Discussion J Additional Future Work Directions…

**Conclusion.** Conclusion and Limitations References A Additional Results A.1 Baselines on SWE-bench A.2 Generality across models on Polyglot A.3 Ablation of Parent Selection A.4 Additional Statistics of DGM runs B Additional Related Work C Algorithmic Details C.1 Initial Coding Agent C.2 Parent Selection C.3 Self-Improve Prompts C.4 Pseudocode D Experiment Details D.1 Hyperparameters for Foundation Models E Benchmark Details E.1 Cost Estimate E.2 SWE-bench Tasks E.3 Polyglot Tasks E.4 SWE-bench State-of-The-Art E.5 Polyglot Representative Agent F Best-Discovered Agents F.1 DGM on SWE-bench F.2 DGM on Polyglot G Similar Target Functionality, Different Implementations H Case Study: Solvin…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[human-agent-interaction|Human-agent interaction]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2505.22954v3.md` · `raw/arxiv/2505.22954v3.fulltext.md`
