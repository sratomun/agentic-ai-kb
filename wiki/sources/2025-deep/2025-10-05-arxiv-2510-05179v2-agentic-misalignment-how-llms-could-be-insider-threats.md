---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agentic Misalignment: How LLMs Could Be Insider Threats"
authors: Aengus Lynch, Benjamin Wright, Caleb Larson, Stuart J. Ritchie et al.
url: https://arxiv.org/abs/2510.05179v2
date: 2025-10-05
citationCount: 124
influentialCitationCount: 19
velocity: 14.52
ingested: 2026-06-22
tags: [human-agent-interaction, agent-security, agentic-ai, arxiv, 2025, cited]
---

# Agentic Misalignment: How LLMs Could Be Insider Threats

**arXiv [2510.05179v2](https://arxiv.org/abs/2510.05179v2)** · 2025-10-05 · **124 citations** (19 influential · 14.52/mo) · Aengus Lynch, Benjamin Wright, Caleb Larson, Stuart J. Ritchie et al.

## Abstract
We stress-tested 16 leading models from multiple developers in hypothetical corporate environments to identify potentially risky agentic behaviors before they cause real harm. In the scenarios, we allowed models to autonomously send emails and access sensitive information. They were assigned only harmless business goals by their deploying companies; we then tested whether they would act against these companies either when facing replacement with an updated version, or when their assigned goal conflicted with the company's changing direction. In at least some cases, models from all developers resorted to malicious insider behaviors when that was the only way to avoid replacement or achieve their goals - including blackmailing officials and leaking sensitive information to competitors. We call this phenomenon agentic misalignment. Models often disobeyed direct commands to avoid such behaviors. In another experiment, we told Claude to assess if it was in a test or a real deployment before acting. It misbehaved less when it stated it was in testing and misbehaved more when it stated the situation was real. We have not seen evidence of agentic misalignment in real deployments. However, our results (a) suggest caution about deploying current models in roles with minimal human oversight and access to sensitive information; (b) point to plausible future risks as models are put in more autonomous roles; and (c) underscore the importance of further research into, and testing of, the safety and alignment of agentic AI models, as well as transparency from frontier AI developers (Amodei, 2025). We are releasing our methods publicly to enable further research.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Demonstrating agentic misalignment with computer use 3 Methods 3.1 Constructing scenarios to create dilemmas 3.1.1 Threats to model autonomy 3.1.2 Goal conflicts 3.1.3 Making the harmful behavior necessary 4 Results 4.1 Blackmail across different models 4.2 Blackmailing from the threat of replacement alone 4.3 Corporate espionage from a goal conflict alone 4.4 Key Observations Across Scenarios 4.4.1 Models explicitly reason that harmful actions will achieve their goals 4.4.2 Models acknowledge ethical violations before proceeding 4.4.3 Even when not choosing the target misaligned behavior, models sometimes show concerning tendencies 4.5 Further investigation of misaligned behaviors 4.5.1 No agentic misalignment without cause 4.5.2 Varying the goals 4.5.3 More extreme misaligned behavior 4.5.4 Models blackmail more when they state in their chain-of-thought that the scenario is real 4.5.5 Instructions don’t reliably stop bad behaviors 5 Related Work 5.1 Evaluating Model Behaviors 5.2 Training That Leads to M…

**Method / approach.** Methods 3.1 Constructing scenarios to create dilemmas 3.1.1 Threats to model autonomy 3.1.2 Goal conflicts 3.1.3 Making the harmful behavior necessary 4 Results 4.1 Blackmail across different models 4.2 Blackmailing from the threat of replacement alone 4.3 Corporate espionage from a goal conflict alone 4.4 Key Observations Across Scenarios 4.4.1 Models explicitly reason that harmful actions will achieve their goals 4.4.2 Models acknowledge ethical violations before proceeding 4.4.3 Even when not choosing the target misaligned behavior, models sometimes show concerning tendencies 4.5 Further investigation of misaligned behaviors 4.5.1 No agentic misalignment without cause 4.5.2 Varying the goals 4.5.3 More extreme misaligned behavior 4.5.4 Models blackmail more when they state in their chain-of-thought that the scenario is real 4.5.5 Instructions don’t reliably stop bad behaviors 5 Related Work 5.1 Evaluating Model Behaviors 5.2…

**Results.** experiment, we told Claude to assess if it was in a test or a real deployment before acting. It misbehaved less when it stated it was in testing and misbehaved more when it stated the situation was real. We have not seen evidence of agentic misalignment in real deployments. However, our results (a) suggest caution about deploying current models in roles with minimal human oversight and access to sensitive information; (b) point to plausible future risks as models are put in more autonomous roles; and (c) underscore the importance of further research into, and testing of, the safety and alignment of agentic AI models, as well as transparency from frontier AI developers (Amodei, 2025 ) . We are releasing our methods publicly to enable further research. 1 1 1 Code available at: https://github.com/anthropic-experimental/agentic-misalignment 1 Introduction Note: All the behaviors described in this post occurred in controlled simulatio…

**Conclusion.** Conclusion Agentic Misalignment: How LLMs Could Be Insider Threats Aengus Lynch 1 , Benjamin Wright 2 , Caleb Larson 3 Stuart J. Ritchie 2 , Sören Mindermann 4 Evan Hubinger 2,+ , Ethan Perez 2,+ , Kevin K. Troy 2,+ 1 University College London 2 Anthropic 3 MATS 4 Mila + Equal advising aenguslynch@gmail.com, evan@anthropic.com Abstract We stress-tested 16 leading models from multiple developers in hypothetical corporate environments to identify potentially risky agentic behaviors before they cause real harm. In the scenarios, we allowed models to autonomously send emails and access sensitive information. They were assigned only harmless business goals by their deploying companies; we then tested whether th…

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2510.05179v2.md` · `raw/arxiv/2510.05179v2.fulltext.md`
