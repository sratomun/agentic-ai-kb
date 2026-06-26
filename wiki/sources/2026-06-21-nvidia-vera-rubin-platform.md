---
type: source
source_type: news
title: NVIDIA Vera Rubin Platform - Seven AI Factory Chips Open the Agentic Inference Frontier
url: https://nvidianews.nvidia.com/news/nvidia-vera-rubin-platform
date: 2026-03-16
ingested: 2026-06-21
depth: full-text
tags:
  - chips
  - inference
  - ai-infrastructure
  - nvidia
  - agentic-ai
---

# NVIDIA Vera Rubin Platform Opens the Agentic AI Frontier

**Why it matters:** The chip layer is now being designed around the exact workload you're betting ADP on — real-time agentic inference, not training. NVIDIA is explicitly framing Vera Rubin as the infrastructure for "agents-in-production," with Anthropic and OpenAI named as customers. If the cost-per-token and throughput claims hold, the unit economics of running autonomous agents at enterprise scale improve materially over the next 12 months. That moves "agents everywhere in the workforce" from roadmap to budget line.

## What happened
At GTC on March 16, 2026, NVIDIA announced the Vera Rubin platform with seven new chips in full production, positioned to scale the world's largest AI factories. Products ship from partners in H2 2026 — so this is an announcement now, availability later. The platform bundles the Vera CPU, Rubin GPU, NVLink 6 Switch, ConnectX-9 SuperNIC, BlueField-4 DPU, Spectrum-6 Ethernet switch, and the newly integrated Groq 3 LPU, designed to operate as one AI supercomputer across pretraining, post-training, test-time scaling, and real-time agentic inference.

## Details
- **Named customers:** Dario Amodei (Anthropic) — "Enterprises and developers are using Claude for increasingly complex reasoning, agentic workflows and mission-critical decisions. That demands infrastructure that can keep pace." Sam Altman (OpenAI) — will "run more powerful models and agents at massive scale." Jensen Huang called it "a generational leap... The agentic AI inflection point has arrived."
- **Vera Rubin NVL72 rack:** 72 Rubin GPUs + 36 Vera CPUs over NVLink 6. Trains large MoE models with one-fourth the GPUs vs Blackwell; up to 10x higher inference throughput per watt at one-tenth the cost per token.
- **Vera CPU Rack:** 256 Vera CPUs for CPU-heavy RL/agentic environments; ~2x more efficient and 50% faster than traditional CPUs.
- **Groq 3 LPX Rack (newly integrated):** built for low-latency, large-context agentic systems; up to 35x higher inference throughput per megawatt and up to 10x more revenue opportunity for trillion-parameter models; 256 LPUs, 128GB on-chip SRAM, 640 TB/s scale-up bandwidth. Available H2 2026.
- **BlueField-4 STX storage:** AI-native KV-cache storage; DOCA Memos boosts inference throughput up to 5x (Mistral CTO Timothée Lacroix quoted).
- **Spectrum-6 SPX Ethernet; DSX platform:** DSX Max-Q enables 30% more AI infra in fixed power; DSX Flex unlocks 100 GW of stranded grid power.
- **Availability:** partner products from H2 2026 via AWS, Google Cloud, Azure, OCI, CoreWeave; OEMs Dell, HPE, Lenovo, Supermicro, Cisco. Frontier labs Anthropic, Meta, Mistral, OpenAI plan to use it.

## So what
The signal isn't the silicon — it's the workload thesis. NVIDIA, Anthropic, and OpenAI are all now publicly anchoring their roadmaps on agentic inference as the dominant workload. For ADP, this is tailwind: cheaper, faster agent inference lowers the cost of embedding autonomous agents in payroll, HR, and compliance workflows. Worth tracking the H2 2026 ship dates and the cost-per-token claims as they meet reality, since your build-vs-buy math on agent infrastructure depends on them.

**Connects to:** [[agentic-ai]] [[nvidia]] [[vera-rubin]] [[nvidia]]

**Raw:** `raw/news/2026-03-16-nvidia-vera-rubin-platform.fulltext.md`
