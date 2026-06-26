---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving"
authors: Lloyd Russell, Anthony Hu, Lorenzo Bertoni, George Fedoseev et al.
url: https://arxiv.org/abs/2503.20523v1
date: 2025-03-26
citationCount: 143
influentialCitationCount: 8
velocity: 9.61
ingested: 2026-06-22
tags: [autonomous-driving-agents, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving

**arXiv [2503.20523v1](https://arxiv.org/abs/2503.20523v1)** · 2025-03-26 · **143 citations** (8 influential · 9.61/mo) · Lloyd Russell, Anthony Hu, Lorenzo Bertoni, George Fedoseev et al.

## Abstract
Generative models offer a scalable and flexible paradigm for simulating complex environments, yet current approaches fall short in addressing the domain-specific requirements of autonomous driving - such as multi-agent interactions, fine-grained control, and multi-camera consistency. We introduce GAIA-2, Generative AI for Autonomy, a latent diffusion world model that unifies these capabilities within a single generative framework. GAIA-2 supports controllable video generation conditioned on a rich set of structured inputs: ego-vehicle dynamics, agent configurations, environmental factors, and road semantics. It generates high-resolution, spatiotemporally consistent multi-camera videos across geographically diverse driving environments (UK, US, Germany). The model integrates both structured conditioning and external latent embeddings (e.g., from a proprietary driving model) to facilitate flexible and semantically grounded scene synthesis. Through this integration, GAIA-2 enables scalable simulation of both common and rare driving scenarios, advancing the use of generative world models as a core tool in the development of autonomous systems. Videos are available at https://wayve.ai/thinking/gaia-2.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Model 2.1 Video Tokenizer 2.1.1 Encoder 2.1.2 Decoder 2.1.3 Training Losses 2.2 World Model 2.2.1 Architecture 2.2.2 Losses 2.2.3 Conditioning Camera Parameters. Video Frequency. Action. Dynamic Agents. Metadata. CLIP Embedding. Scenario Embedding. 2.2.4 Flow matching Time Distribution 3 Data 4 Training Procedure Video Tokenizer. World Model. 5 Inference Inference Tasks. Inference Noise Schedule. Classifier-Free Guidance. 6 Results Augmenting Real-World Data. 6.1 Qualitative Examples Diverse Scenario Generation. Generating Safety-Critical Scenarios. Inpainting. 6.2 Metrics Visual Fidelity. Temporal Consistency. Dynamic Agent Conditioning. 7 Related Work Video Generative Models. Generative World Models in Autonomous Driving. 8 Conclusions and Future Work Future Work. GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving Lloyd Russell Anthony Hu 1 1 footnotemark: 1 Lorenzo Bertoni 1 1 footnotemark: 1 George Fedoseev 1…

**Method / approach.** approaches fall short in addressing the domain-specific requirements of autonomous driving—such as multi-agent interactions, fine-grained control, and multi-camera consistency. We introduce GAIA-2, Generative AI for Autonomy , a latent diffusion world model that unifies these capabilities within a single generative framework. GAIA-2 supports controllable video generation conditioned on a rich set of structured inputs: ego-vehicle dynamics, agent configurations, environmental factors, and road semantics. It generates high-resolution, spatiotemporally consistent multi-camera videos across geographically diverse driving environments (UK, US, Germany). The model integrates both structured conditioning and external latent embeddings (e.g., from a proprietary driving model) to facilitate flexible and semantically grounded scene synthesis. Through this integration, GAIA-2 enables scalable simulation of both common and rare driving scenarios, advancing the use of generative world models as a c…

**Results.** experiments, we use a fixed number of 50 denoising steps. Classifier-Free Guidance. Classifier-free guidance (CFG) is not used by default during inference. However, for challenging or out-of-distribution scenarios, such as those involving rare edge cases or unusual agent configurations (e.g., Figure 11 ), we activate CFG with a guidance scale ranging from 2 to 20, depending on the complexity of the scene. In scenarios involving dynamic agent conditioning, where the latent tokens associated with agent-specific regions are known a priori, we apply spatially selective CFG. In this case, guidance is applied only to the spatial locations influenced by the conditioning (e.g., 3D bounding boxes), which enhances generation quality in targeted regions without unnecessarily affecting the rest of the scene. This targeted approach enables more precise control over scene elements while preserving global coherence. Figure 5 : Multi-rig…

**Conclusion.** Conclusions and Future Work Future Work. GAIA-2: A Controllable Multi-View Generative World Model for Autonomous Driving Lloyd Russell Anthony Hu 1 1 footnotemark: 1 Lorenzo Bertoni 1 1 footnotemark: 1 George Fedoseev 1 1 footnotemark: 1 Jamie Shotton Elahe Arani Gianluca Corrado 1 1 footnotemark: 1 Wayve research@wayve.ai Equal contribution, random order. Abstract Generative models offer a scalable and flexible paradigm for simulating complex environments, yet current approaches fall short in addressing the domain-specific requirements of autonomous driving—such as multi-agent interactions, fine-grained control, and multi-camera consistency. We introduce GAIA-2, Generative AI for Autonomy , a latent diffusio…

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2503.20523v1.md` · `raw/arxiv/2503.20523v1.fulltext.md`
