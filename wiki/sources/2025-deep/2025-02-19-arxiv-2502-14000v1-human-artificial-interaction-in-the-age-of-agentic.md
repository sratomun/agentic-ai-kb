---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Human-Artificial Interaction in the Age of Agentic AI: A System-Theoretical Approach"
authors: Uwe M. Borghoff, Paolo Bottoni, Remo Pareschi
url: https://arxiv.org/abs/2502.14000v1
date: 2025-02-19
citationCount: 66
influentialCitationCount: 2
velocity: 4.12
ingested: 2026-06-22
tags: [embodied-agents, human-agent-interaction, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# Human-Artificial Interaction in the Age of Agentic AI: A System-Theoretical Approach

**arXiv [2502.14000v1](https://arxiv.org/abs/2502.14000v1)** · 2025-02-19 · **66 citations** (2 influential · 4.12/mo) · Uwe M. Borghoff, Paolo Bottoni, Remo Pareschi

## Abstract
This paper presents a novel perspective on human-computer interaction (HCI), framing it as a dynamic interplay between human and computational agents within a networked system. Going beyond traditional interface-based approaches, we emphasize the importance of coordination and communication among heterogeneous agents with different capabilities, roles, and goals. A key distinction is made between multi-agent systems (MAS) and Centaurian systems, which represent two different paradigms of human-AI collaboration. MAS maintain agent autonomy, with structured protocols enabling cooperation, while Centaurian systems deeply integrate human and AI capabilities, creating unified decision-making entities. To formalize these interactions, we introduce a framework for communication spaces, structured into surface, observation, and computation layers, ensuring seamless integration between MAS and Centaurian architectures, where colored Petri nets effectively represent structured Centaurian systems and high-level reconfigurable networks address the dynamic nature of MAS. Our research has practical applications in autonomous robotics, human-in-the-loop decision making, and AI-driven cognitive architectures, and provides a foundation for next-generation hybrid intelligence systems that balance structured coordination with emergent behavior.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Paradigms in Human-AI Integration 2.1 Architectural Differences 2.2 Integration Paradigms, Operational Dynamics, and Convergence Points 2.3 Implications for System Design 2.4 Situating Human-Machine Collaboration in the Context of Agentic AI 3 Technical Background: Petri nets 3.1 Basic Concepts and Advantages 3.2 Colored Petri Nets and Typed Tokens 3.3 Illustrative Example 3.4 Relevance to Hybrid Agent Systems 4 Communication Spaces and Agent Architectures 4.1 Foundations and Rationale 4.2 Core Ideas of Communication Spaces 4.3 Implementing Communication Spaces 4.4 Formal Representation with Colored Petri Nets: Communication Space Petri Net 4.5 Implementation Considerations 5 Use Case 1: Multi-agent Interaction with Satellite and Swarm Robots 5.1 System Overview 5.2 Integration with LLM and Human Operators 5.3 Practical Applications 5.4 Human-Agent Collaboration 6 Use Case 2: Large Action Models (LAMs) through Feedback Loops on HCI Interactions 6.1 System Overview 6.2 Neuro-Symbolic Integration 6.3 Human…

**Method / approach.** methods, allowing for emergent collective problem-solving. Such architectures thrive on adaptability, where boundaries are permeable and agents can fluidly exchange roles or data to optimize performance. 4.4 Formal Representation with Colored Petri Nets: Communication Space Petri Net We extend colored Petri nets to create a Communication Space Petri net , where places are partitioned into surface , observation , and computation categories. Tokens carry types or “colors” corresponding to data formats or message semantics relevant to each space. Transition guards incorporate rules for agent-specific capabilities (e.g., a color set may denote “human text command” vs. “drone sensor data”). This enriched formalism preserves the tractability of standard Petri nets while accommodating the specialized interactions of heterogeneous agents. For example, transitions in the observation space can fire only when tokens of type “parsed command” are present, ensuring that raw data never…

**Results.** experiment with a semi-centralized coordinated swarm of robots, using both “rigid” optimization algorithms and “flexible” intervention through a large language model (LLM). This setup encapsulates a true multi-agent HCI interaction, integrating human operators, conversational AI, the satellite control unit, and swarm robots. Figure 8: Interaction of human operators, conversational AI, satellite, and a robotic swarm. This use case extends the application of a semi-centralized control strategy, originally enhanced with blockchain technology for security and transparency [ 17 ] . The multi-agent paradigm is evident in how distinct entities—the satellite control unit, swarm robots, LLM, and human operators—maintain their functional independence while collaborating through well-defined protocols. However, the system also exhibits Centaurian characteristics in specific interaction points, particularly in the human-LLM interface. The…

**Conclusion.** Conclusion and Future Work 1 1 institutetext: Computer Science, University of the Bundeswehr Munich, Neubiberg, Germany 2 2 institutetext: Computer Science, Sapienza University of Rome, Rome, Italy 3 3 institutetext: Stake Lab, Università degli Studi del Molise, Campobasso, Italy Human-Artificial Interaction in the Age of Agentic AI: A System-Theoretical Approach Uwe M. Borghoff Corresponding author: uwe.borghoff@unibw.de Paolo Bottoni Remo Pareschi Abstract This paper presents a novel perspective on human-computer interaction (HCI), framing it as a dynamic interplay between human and computational agents within a networked system. Going beyond traditional interface-based approaches, we emphasize the importance of…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[human-agent-interaction|Human-agent interaction]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.14000v1.md` · `raw/arxiv/2502.14000v1.fulltext.md`
