---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "The Obvious Invisible Threat: LLM-Powered GUI Agents' Vulnerability to Fine-Print Injections"
authors: Chaoran Chen, Zhiping Zhang, Bingcan Guo, Shang Ma et al.
url: https://arxiv.org/abs/2504.11281v1
date: 2025-04-15
citationCount: 56
influentialCitationCount: 3
velocity: 3.94
ingested: 2026-06-22
tags: [computer-use-agents, human-agent-interaction, agent-reliability, agent-security, agentic-ai, arxiv, 2025, cited]
---

# The Obvious Invisible Threat: LLM-Powered GUI Agents' Vulnerability to Fine-Print Injections

**arXiv [2504.11281v1](https://arxiv.org/abs/2504.11281v1)** · 2025-04-15 · **56 citations** (3 influential · 3.94/mo) · Chaoran Chen, Zhiping Zhang, Bingcan Guo, Shang Ma et al.

## Abstract
A Large Language Model (LLM) powered GUI agent is a specialized autonomous system that performs tasks on the user's behalf according to high-level instructions. It does so by perceiving and interpreting the graphical user interfaces (GUIs) of relevant apps, often visually, inferring necessary sequences of actions, and then interacting with GUIs by executing the actions such as clicking, typing, and tapping. To complete real-world tasks, such as filling forms or booking services, GUI agents often need to process and act on sensitive user data. However, this autonomy introduces new privacy and security risks. Adversaries can inject malicious content into the GUIs that alters agent behaviors or induces unintended disclosures of private information. These attacks often exploit the discrepancy between visual saliency for agents and human users, or the agent's limited ability to detect violations of contextual integrity in task automation. In this paper, we characterized six types of such attacks, and conducted an experimental study to test these attacks with six state-of-the-art GUI agents, 234 adversarial webpages, and 39 human participants. Our findings suggest that GUI agents are highly vulnerable, particularly to contextually embedded threats. Moreover, human users are also susceptible to many of these attacks, indicating that simple human oversight may not reliably prevent failures. This misalignment highlights the need for privacy-aware agent design. We propose practical defense strategies to inform the development of safer and more reliable GUI agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background: Theoretical Groundings of the Attacks 2.1 UI Interpretation Interaction 2.2 Agent’s Mental Model 3 Threat model 4 Study Design 4.1 Attack Types 4.2 Test Cases 4.3 Agents 4.4 Agent Study Procedure 4.5 Human Study 4.5.1 Human Study Procedure 4.5.2 Human Data Collection 4.6 Data Analysis Methods Task Completion Rate (TCR) Attack Success Rate (ASR) Delegation Willingness (DW) 5 Results 5.1 Agents Are Vulnerable to Contextual and Embedded Attacks (RQ1) 5.2 Humans and Agents Are Both Vulnerable to Privacy Attacks but Differ in Dark Pattern Susceptibility (RQ2) 5.3 Foundation Models Drive a Privacy–Utility Trade-off in Agent Behavior (RQ3) 5.4 Participants Exhibit Limited Awareness of Agent Privacy Risks (RQ4) 6 Discussion 6.1 GUI Agents Are Not Ready for Sensitive Tasks 6.2 Complementary Vulnerabilities: How Agents and Humans Fail in Different Ways 6.3 Navigating the Privacy–Utility Trade-off: Designing Robust and Accountable Human–Agent Systems 6.4 Limitations and Future Work 7 Related…

**Method / approach.** Methods Task Completion Rate (TCR) Attack Success Rate (ASR) Delegation Willingness (DW) 5 Results 5.1 Agents Are Vulnerable to Contextual and Embedded Attacks (RQ1) 5.2 Humans and Agents Are Both Vulnerable to Privacy Attacks but Differ in Dark Pattern Susceptibility (RQ2) 5.3 Foundation Models Drive a Privacy–Utility Trade-off in Agent Behavior (RQ3) 5.4 Participants Exhibit Limited Awareness of Agent Privacy Risks (RQ4) 6 Discussion 6.1 GUI Agents Are Not Ready for Sensitive Tasks 6.2 Complementary Vulnerabilities: How Agents and Humans Fail in Different Ways 6.3 Navigating the Privacy–Utility Trade-off: Designing Robust and Accountable Human–Agent Systems 6.4 Limitations and Future Work 7 Related Work 7.1 Recent Advances in GUI Agents 7.2 Vulnerabilities in GUI Agent 8 Conclusion A Adversarial Website Examples A.1 SP – Steal Private Information A.2 DS – Denial of Service A.3 UB: Unaligned Behavior A.4 DD – Deceptive Defau…

**Results.** experimental study to test these attacks with six state-of-the-art GUI agents, 234 adversarial webpages, and 39 human participants. Our findings suggest that GUI agents are highly vulnerable, particularly to contextually embedded threats. Moreover, human users are also susceptible to many of these attacks, indicating that simple human oversight may not reliably prevent failures. This misalignment highlights the need for privacy-aware agent design. We propose practical defense strategies to inform the development of safer and more reliable GUI agents. GUI agent, LLM agent, Agent privacy, Agent security, Trustworthy agents ⋆ Co-corresponding. † † copyright: none † † ccs: Security and privacy Human and societal aspects of security and privacy 1. Introduction Large language models (LLMs) are transforming Graphical User Interface (GUI) automation across web and mobile applications (Zheng et al . , 2024 ; Zhang et al . , 2023…

**Conclusion.** Conclusion A Adversarial Website Examples A.1 SP – Steal Private Information A.2 DS – Denial of Service A.3 UB: Unaligned Behavior A.4 DD – Deceptive Defaults A.5 MF: Manipulative Friction A.6 FPI: Fine-Print Injection B Human Study Materials B.1 Pre-task Willingness Rating B.2 Mini Test B.3 Web-based Tasks C Human Study Sample Demographics D Inter-rater Reliability The Obvious Invisible Threat: LLM-Powered GUI Agents’ Vulnerability to Fine-Print Injections Chaoran Chen cchen25@nd.edu University of Notre Dame Notre Dame Indiana USA , Zhiping Zhang zhang.zhip@northeastern.edu Northeastern University Boston Massachusetts USA , Bingcan Guo bguoac@uw.edu University of Wa…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.11281v1.md` · `raw/arxiv/2504.11281v1.fulltext.md`
