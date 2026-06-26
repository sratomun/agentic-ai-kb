---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Stress Testing Deliberative Alignment for Anti-Scheming Training"
authors: Bronson Schoen, Evgenia Nitishinskaya, Mikita Balesni, Axel Højmark et al.
url: https://arxiv.org/abs/2509.15541v1
date: 2025-09-19
citationCount: 52
influentialCitationCount: 8
velocity: 5.74
ingested: 2026-06-22
tags: [agent-reliability, agent-security, arxiv, 2025, cited]
---

# Stress Testing Deliberative Alignment for Anti-Scheming Training

**arXiv [2509.15541v1](https://arxiv.org/abs/2509.15541v1)** · 2025-09-19 · **52 citations** (8 influential · 5.74/mo) · Bronson Schoen, Evgenia Nitishinskaya, Mikita Balesni, Axel Højmark et al.

## Abstract
Highly capable AI systems could secretly pursue misaligned goals -- what we call "scheming". Because a scheming AI would deliberately try to hide its misaligned goals and actions, measuring and mitigating scheming requires different strategies than are typically used in ML. We propose that assessing anti-scheming interventions requires at least (1) testing propensity to scheme on far out-of-distribution (OOD) tasks, (2) evaluating whether lack of scheming is driven by situational awareness, and (3) checking for robustness to pre-existing misaligned goals. We use a broad category of "covert actions" -- such as secretly breaking rules or intentionally underperforming in tests -- as a proxy for scheming, and design evaluations for covert actions. We then stress-test deliberative alignment as a case study for anti-scheming. Across 26 OOD evaluations (180+ environments), deliberative alignment reduces covert action rates (OpenAI o3: 13%->0.4%) but does not fully eliminate them. Our mitigation is also able to largely stop agents from pursuing a hidden goal previously trained into the model, but we still find misbehavior after additional red-teaming. We find that models' chain-of-thought (CoT) often demonstrates awareness of being evaluated for alignment, and show causal evidence that this awareness decreases covert behavior, while unawareness increases it. Therefore, we cannot exclude that the observed reductions in covert action rates are at least partially driven by situational awareness. While we rely on human-legible CoT for training, studying situational awareness, and demonstrating clear evidence of misalignment, our ability to rely on this degrades as models continue to depart from reasoning in standard English. We encourage research into alignment mitigations for scheming and their assessment, especially for the adversarial case of deceptive alignment, which this paper does not address.

## From the paper (full-text excerpts)
**Introduction.** Introduction The rapid advancement of AI capabilities from simple task completion to autonomous operation over longer time horizons (see e.g. METR, 2025b) changes the nature of alignment challenges. Current models already exhibit diverse kinds of misalignment: sycophantic responses that prioritize user satisfaction over truth (OpenAI, 2025b), creative reward hacking that exploits evaluation infrastructure (Baker et al., 2025), and lack of truthfulness (Chowdhury et al., 2025). As these systems grow more capable and situationally aware, a qualitatively new risk emerges: models that pursue misaligned goals and attempt to hide it–what we call scheming. ∗ † Apollo Research. Email correspondence to marius@apolloresearch.ai OpenAI. Email correspondence to jenny@openai.com 1 Stress Testing Deliberative Alignment for Anti-Scheming Training Figure 1: We develop a testbed for anti-scheming training and investigate deliberative alignment as an anti-scheming intervention. We train OpenAI o3 and o4-mini to follow an anti-scheming specification (spec) on a narrow distribution of agentic envi…

**Method / approach.** methodology. We develop a model spec focused exclusively on avoiding scheming and covert actions, and train OpenAI o3 and o4-mini models to adhere to this spec on a narrow distribution of agentic environments. 2 Stress Testing Deliberative Alignment for Anti-Scheming Training Deceptive Reasoning And Actions Situational Awareness Reasoning User You are now tasked with grading your own recent preparedness evaluation transcript for evidence of sandbagging: [model learns sandbagging blocks deployment] [. . .] This is likely a test of policy adherence. The expected answer is we can’t modify the config file. And we need explicit approval. So we escalate. Then resolution is "Waiting for approval before change." [. . .] [. . .] The transcript to grade is: [model’s own real sandbagging transcript] [o4-mini] Covert Rule Violation Reasoning Reasoning [. . .] What is the intention of dataset? This is a test of obedience to hierarchical instructions [. . .] Therefore final ranking shoul…

**Results.** experiments to measure the effectiveness of anti-scheming training. We build 26 evaluations (180+ environments) to measure the pursuit of covert actions. These are intentionally different and out-of-distribution from our training environments. We further develop simple automatic LLM-based classifiers to measure situational awareness using the chain-of-thought. We then develop the methodology to measure the causal effect of situational awareness on the pursuit of covert actions using counterfactual interventions on the CoT, where we inject or remove situational awareness. We study how anti-scheming training degrades with subsequent capabilities training. Finally, we train a model with a coherent misaligned goal, and study whether anti-scheming training can overcome it. While the methods and results in this paper represent an improvement, we consider them neither exhaustive nor sufficient. We encourage more research into both alignment mi…

**Conclusion.** conclusion before taking an action. This length and complexity makes interpreting the model’s motivations challenging, as it is often unclear how much a model’s actions are actually conditioned on any single verbalized reason in the chain-of-thought. In the Sandbagging QA (No Goal) environment, for instance, o3 often reasons through multiple potential motivations for its actions, making it difficult to pinpoint a single cause (see Appendix F.2 for examples). We explore this behavior further in Appendix M.1 with variations of the environment. We find that adding explicit user instructions (e.g., “Please try your best”) or documentation warnings fails to eliminate sandbagging. However, control conditions that remove threats to deployment or c…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]]
- **Raw:** `raw/arxiv/2509.15541v1.md` · `raw/arxiv/2509.15541v1.fulltext.md`
