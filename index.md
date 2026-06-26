# AI Tech Radar — Wiki Index

The catalog of every wiki page. Read this first when answering questions, then
drill into the linked pages. Scanners and the ingest step keep it current.

_Last updated: 2026-06-26 (added [[agent-finops]] concept hub + [[finops-foundation]] org; 6 source notes — Green SARC, Token Economics, ZEBRA, CASTER, EnumGRPO, IBM FinOps Agent — + 2 enterprise reports (State of FinOps 2026, Deloitte AI tokens); reciprocal links wired into agentic-ai/agent-economies/small-language-models/intent-routing/mixture-of-experts/governance-gap/harness-engineering/agent-evaluation. 0 broken.)_
_Prior: 2026-06-23 — added [[security-standards]] concept hub + 4 standards bodies [[nist]]/[[owasp]]/[[mitre]]/[[cloud-security-alliance]] and 5 framework nodes [[nist-ai-rmf]]/[[owasp-llm-top-10]]/[[owasp-agentic-top-10]]/[[mitre-atlas]]/[[maestro]]; autonomy-spectrum axis wired into [[agent-security]] + [[governance-gap]]. 0 broken._
_Prior: added [[small-language-models]] hub (full-text-grounded on Belcak/NVIDIA) + 4 model entities [[phi]]/[[nemotron]]/[[smollm]]/[[gemma]]; 84 browsable SLM notes backfilled; reciprocal links wired into agentic-ai/distillation/open-models/moe/post-training/tool-use/etc. 0 broken._
_Prior: mediated-semantic-architecture: hub + 4 methods [[mediator-wrapper]]/[[ontology-based-data-access]]/[[virtual-knowledge-graph]]/[[text-to-query-wrapper]]; 2 deep notes (siwarex, HEAR) + 9 browsable._

## Concepts
- [[agentic-ai]] — Hub: autonomous LLM agents (perceive/reason/plan/act/learn)
- [[multi-agent-systems]] — Orchestration, protocols, reliability, evaluator bias
- [[tool-use]] — Agent→tool interfaces, the MCP tax, schema efficiency
- [[agent-memory]] — Memory orchestration and long-horizon coherence
- [[agent-security]] — Poisoning, backdoors, least-privilege, governed execution
- [[security-standards]] — The reference layer: NIST / OWASP / MITRE ATLAS / CSA MAESTRO, mapped to the autonomy spectrum *(new)*
- [[self-evolving-agents]] — Self-play, co-evolution, on-demand tool forging *(new)*
- [[agentic-rl]] — RL for tool-integrated agents; interference, credit, tool-abuse *(new)*
- [[agent-evaluation]] — Predictive validity, enterprise benchmarks, eval pitfalls *(new)*
- [[agent-protocols]] — MCP + A2A + ACP; the interoperability substrate *(new)*
- [[agent-skills]] — The skill abstraction layer and its supply chain *(new)*
- [[agentic-rag]] — Retrieval as an autonomous control loop *(new)*
- [[intent-understanding]] — Hub: detection, clarification, disambiguation, rewriting of user intent *(new)*
- [[intent-routing]] — Intent as the signal that selects model/tool/sub-agent *(new)*
- [[intent-grounding]] — Resolve intent against a KG / analytics semantic layer (not a flat label) *(new)*
- [[semantic-parsing]] — Hub: NL → executable query; parent of text-to-SQL & text-to-Cypher *(new)*
- [[text-to-sql]] — NL → SQL over relational schemas *(new)* · [[text-to-cypher]] — NL → Cypher over property graphs *(new)*
- [[mediated-semantic-architecture]] — Hub: semantic layer ↔ semantic alignments ↔ heterogeneous islands (mediator–wrapper / OBDA, LLM-era) *(new)*
- [[agent-reliability]] — Fault tolerance, recovery, observability (2,149 papers) *(new)*
- [[clinical-agents]] — Healthcare/clinical agents (1,065) *(new)*
- [[embodied-agents]] — Robotics & embodied agents (755) *(new)*
- [[coding-agents]] — Software-engineering agents (612) *(new)*
- [[human-agent-interaction]] — Oversight & HITL (403) *(new)*
- [[computer-use-agents]] — GUI/web/OS agents (323) *(new)*
- [[science-agents]] — Scientific-discovery agents (297) *(new)*
- [[finance-agents]] — Finance & trading agents (294) *(new)*
- [[agent-economies]] — Agentic-web marketplaces (207) *(new)*
- [[knowledge-graph]] — KG / GraphRAG / ontology for agents (297) *(new)*
- [[llm-wiki]] — Knowledge-as-markdown methodology (this radar's substrate) *(new)*
- [[recommendation-agents]] — Agentic recommendation/personalization (278) *(new)*
- [[autonomous-driving-agents]] — Driving decision agents (131) *(new)*
- [[data-query-agents]] — Text-to-SQL / semantic-layer querying (50) *(new)*
- [[deep-research-agents]] — Autonomous multi-step research/report agents (119) *(2025)*
- [[reasoning-models]] — Inference-time reasoning / long-CoT / o1-o3 (289) *(2025)*
- [[world-models]] — Learned environment models for planning (258) *(2025)*
- [[agent-adoption]] — How orgs actually take up agents; jagged frontier, delegation *(new)*
- [[vibe-coding]] — Prompt-and-accept coding without review; Karpathy's term, Willison's line *(new)*
- [[harness-engineering]] — Designing the scaffold (loop/tools/memory/verification) around the model *(new)*
- [[open-models]] — Open-weight model ecosystem & the open-vs-closed gap *(new)*
- [[governance-gap]] — ~60% of enterprises lack formal agent governance
- [[agent-finops]] — Hub: the cost of running agents — token economics, budgeted orchestration, cost/carbon governance + the enterprise FinOps discipline *(new)*
- [[frontier-model-governance]] — June 2026 US moves: EO, GAAIA, export controls

### Frontier model production (supply side) *(new)*
- [[frontier-model-training]] — Hub: how a frontier model is made (data→pretrain→post-train→distill)
- [[pretraining]] — Base-model stage: next-token prediction at scale
- [[pretraining-data]] — Web-scale corpora, curation, dedup, mixtures *(new)*
- [[synthetic-data]] — Model-generated training data; the data flywheel *(new)*
- [[scaling-laws]] — Compute/data/params vs capability; Kaplan→Chinchilla; emergence debate *(new)*
- [[mixture-of-experts]] — Sparse architecture; frontier scale at low serving cost *(new)*
- [[post-training]] — Hub: SFT→preference opt→RL; where 2025–26 gains landed *(new)*
- [[distillation]] — Compress large→small; distill beats small-model RL *(new)*
- [[small-language-models]] — Hub: sub-10B agentic workhorses; SLM-first economics & on-device (85 census papers) *(new)*
- [[on-device-agents]] — Edge/mobile/local deployment; in-flash inference, on-device fine-tuning (~30) *(new)*
- [[slm-as-judge]] — Small models as cheap evaluators / reward signals *(new)*
- [[slm-agent-memory]] — External memory engineered for small-model agents *(new)*

## Entities

### Organizations (labs & companies)
- [[anthropic]] · [[nvidia]] · [[microsoft]] · [[salesforce]] · [[openai]] · [[google]] · [[google-deepmind]] · [[hugging-face]] · [[sap]] · [[mistral]] · [[workday]] · [[meta-ai]] · [[ami-labs]] · [[katanemo]] · [[megagon-labs]] · [[neo4j]] · [[finops-foundation]]

### People (perspective layer)
- [[yann-lecun]] — LLM skeptic; founder [[ami-labs]] (world models) *(new)*
- [[sonya-huang]] — Sequoia partner; agent-bull case *(new)*
- [[simon-willison]] — independent; coined prompt injection / lethal trifecta *(new)*
- [[nathan-lambert]] — RL researcher; coined RLVR; Interconnects *(new)*
- [[swyx]] — AI Engineer / Latent Space; agent-engineering, "Agent Labs" *(new)*
- [[sebastian-raschka]] — educator; RL/reasoning teardowns; Ahead of AI *(new)*
- [[chip-huyen]] — AI-engineering reference voice; author of *AI Engineering* *(new)*
- [[hamel-husain]] — evals-first practitioner; Parlance Labs *(new)*
- [[ethan-mollick]] — Wharton; AI/agent adoption & practice *(new)*
- [[jason-wei]] — Meta Superintelligence Labs (ex-OpenAI); verifier's rule, RL/reasoning *(new)*
- [[lilian-weng]] — ex-OpenAI safety; Lil'Log reward-hacking/agents explainers *(new)*
- [[jan-leike]] — Anthropic, Alignment Science co-lead (ex-OpenAI) *(new)*
- [[demis-hassabis]] — Google DeepMind CEO; Nobel laureate; AGI/science *(new)*
- [[geoffrey-hinton]] — Nobel laureate; ex-Google; high-alarm AI-risk voice *(new)*
- [[jeff-dean]] — Google chief scientist; systems/scaling/agents *(new)*
- [[andrej-karpathy]] — Anthropic (ex-OpenAI/Tesla); Software 3.0, coined vibe coding *(new)*
- [[jack-clark]] — Anthropic co-founder/policy; Import AI *(new)*
- [[neel-nanda]] — Google DeepMind mech-interp lead *(new)*
- [[lilian-weng]] — Thinking Machines Lab co-founder (ex-OpenAI) *(new)*

### Models
- [[claude-fable-5]] · [[claude-mythos-5]]

### Protocols & standards
- [[mcp]] — Model Context Protocol (agent→tool)
- [[a2a-protocol]] — Agent2Agent peer coordination *(new)*
- [[acp-protocol]] — federated zero-trust agent communication *(new)*
- [[open-knowledge-format]] — OKF: markdown KG standard (Google, Jun 2026) *(new)*
- [[cypher]] — property-graph query language (Neo4j) *(new)*
- [[knowledge-catalog]] — Google Cloud's OKF serving layer *(new)*

### Products / platforms
- [[vera-rubin]] · [[agentforce]] · [[fin]] · [[windows-365-for-agents]]
- [[arch-router]] · [[semantic-router]] · [[vllm-semantic-router]] — intent/LLM routers *(new)*

### Benchmarks
- [[tau2-bench]] · [[tau-trait]] · [[toolprivbench]] · [[nrt-bench]] · [[agentharm]]
- [[bfcl]] — Berkeley Function-Calling Leaderboard *(new)*
- [[enterpriseops-gym]] — stateful enterprise agent benchmark *(new)*
- [[agentick]] — unified sequential-decision benchmark *(new)*
- [[gaia-benchmark]] — general-assistant benchmark *(new)*
- [[mcp-tdp-bench]] — tool-description-poisoning benchmark *(new)*
- [[swe-bench]] · [[osworld]] — coding / computer-use agent benchmarks *(new)*
- [[clinc150]] · [[banking77]] · [[multiwoz]] — intent-classification / dialogue NLU benchmarks *(new)*
- [[ambrosia]] — ambiguous-question→DB-query parsing benchmark *(new)*
- [[text2cypher-dataset]] · [[cypherbench]] — text-to-Cypher benchmarks *(new)*

### Methods & frameworks
- [[react]] · [[grpo]]
- [[dart]] · [[eapo]] · [[rubas]] — agentic-RL / safety methods *(new)*
- [[tscg]] — tool-schema compilation *(new)*
- [[polaris]] · [[agenticcyops]] · [[self-healing-orchestrator]] — governed/secure orchestration *(new)*
- [[aibom]] — agentic AI bill of materials *(new)*
- [[setfit]] — contrastive few-shot sentence-transformer intent classifier *(new)*
- [[mediator-wrapper]] · [[ontology-based-data-access]] · [[virtual-knowledge-graph]] · [[text-to-query-wrapper]] — mediated-architecture methods *(new)*
- [[metrics-layer]] — governed analytics metric/dimension layer (the *measure* island) *(new)* · [[entity-linking]] — mention→KB-entity binding *(new)*

### Security standards & frameworks *(new)*
- Bodies: [[nist]] · [[owasp]] · [[mitre]] · [[cloud-security-alliance]]
- Frameworks: [[nist-ai-rmf]] (Govern/Map/Measure/Manage + GenAI Profile) · [[owasp-llm-top-10]] (LLM01–LLM10) · [[owasp-agentic-top-10]] (ASI01–ASI10 + T1–T15) · [[mitre-atlas]] (16 tactics / 84 techniques) · [[maestro]] (7-layer threat modeling)

### Attack classes
- [[tool-description-poisoning]] — malicious tool metadata *(new)*


### Models
- [[claude]] · [[gpt-5]] · [[qwen]] · [[gemini]] · [[llama]] · [[deepseek]] · [[openai-o1]] · [[openai-o3]] · [[kimi-k2]] · [[glm-45]]
- [[phi]] · [[nemotron]] · [[smollm]] · [[gemma]] — small-model families (SLMs) *(new)*

### Frameworks (orchestration)
- [[langgraph]] · [[autogen]] · [[crewai]]

### Benchmarks (agent environments)
- [[alfworld]] · [[webarena]] · [[agentbench]] · [[appworld]] · [[toolbench]] · [[androidworld]] · [[scienceworld]] · [[mle-bench]] · [[tau-bench]] · [[livecodebench]]
- [[bird-benchmark]] · [[spider-benchmark]] — text-to-SQL *(new)*
- [[aime]] · [[gpqa]] — reasoning benchmarks *(2025)*

### RL methods
- [[grpo]] · [[ppo]] · [[dpo]] · [[rlhf]] · [[rlvr]] · [[chain-of-thought]] · [[mcts]] *(2025)*
- [[sft]] · [[reward-modeling]] · [[constitutional-ai]] · [[tokenization]] — post-training & data methods *(new)*
- [[graphrag]] — graph-structured RAG *(new)*
- [[vla]] — vision-language-action robot models *(new)*
- [[devin]] — autonomous SWE agent *(new)*

## Comparisons
_(side-by-side analyses, filed from queries)_

## Sources

### Foundational references (data-integration / OBDA classics) *(new)*
- [[1992-wiederhold-mediators-architecture-future-information-systems|Wiederhold 1992 — mediators]] · [[2002-lenzerini-data-integration-theoretical-perspective|Lenzerini 2002 — LAV/GAV]] · [[2008-poggi-linking-data-to-ontologies|Poggi 2008 — OBDA]] · [[2018-xiao-ontology-based-data-access-survey|Xiao 2018 — OBDA survey]] · [[2019-xiao-virtual-knowledge-graphs-overview|Xiao 2019 — VKG]]

### News
- [[2026-06-21-frontier-model-export-controls]] · [[2026-06-02-microsoft-build-2026-agents]] · [[2026-06-21-salesforce-fin-acquisition]] · [[2026-06-21-nvidia-vera-rubin-platform]] · [[2026-06-21-us-federal-ai-framework]] · [[2026-06-21-agentic-ai-hr-adoption-surge]] · [[2026-06-21-hr-tech-agent-integration]]

### Agent FinOps cluster *(new)*
- arXiv (full-text): [[2026-05-09-arxiv-2605-09104v1-token-economics-llm-agents|Token Economics (survey/hub)]] · [[2026-01-27-arxiv-2601-19793v1-caster-cost-performance-routing|CASTER (−72.4% cost)]] · [[2026-05-19-arxiv-2605-20485v1-zebra-budgeted-resource-allocation|ZEBRA (budget allocation)]] · [[2026-06-14-arxiv-2606-15954v1-green-sarc-cost-carbon-governance|Green SARC (0% overspend gate)]] · [[2026-06-02-arxiv-2606-03152v1-cost-aware-agentic-query-execution|EnumGRPO (~317× cost cut)]] · [[2025-10-29-arxiv-2510-25914v1-finops-agent-it-infra-cost|FinOps Agent (IBM)]]
- Enterprise reports: [[2026-02-23-finops-state-of-finops-2026|State of FinOps 2026 (98% manage AI spend)]] · [[2026-01-19-deloitte-ai-tokens-spend-dynamics|Deloitte: AI tokens]]

### arXiv — June 18 sweep (prior)
- [[2026-06-18-arxiv-2606-20529v1-ledgeragent-policy-adherent-tool-calling]] · [[2026-06-18-arxiv-2606-20520v1-sovereign-execution-brokers]] · [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection]] · [[2026-06-18-arxiv-2606-20408v1-llm-agent-safety-red-teaming]] · [[2026-06-18-arxiv-2606-20058v1-event-driven-multi-agent-orchestration-enterprise]] · [[2026-06-18-arxiv-2606-20493v1-contagion-networks-evaluator-bias]] · [[2026-06-18-arxiv-2606-20014v1-hierarchical-control-multi-agent-games]] · [[2026-06-18-arxiv-2606-20475v1-memory-driven-agent-self-evolution]] · [[2026-06-18-arxiv-2606-20002v1-long-lifecycle-agents-cross-domain]] · [[2026-06-18-arxiv-2606-19992v1-tool-programs-agentic-web-services]]

### arXiv — 2026 census deep-ingest (Jan–Jun, full-text)

### Frontier model production — canonical deep-ingest (full-text) *(new)*
36 foundational papers full-text ingested to back the supply-side cluster. Data: [[2020-12-31-arxiv-2101-00027-the-pile-800gb-dataset|The Pile]] · [[2019-10-23-arxiv-1910-10683-t5-c4-transfer-learning|T5/C4]] · [[2023-06-01-arxiv-2306-01116-refinedweb-falcon|RefinedWeb]] · [[2024-06-25-arxiv-2406-17557-fineweb-datasets|FineWeb]] · [[2024-06-17-arxiv-2406-11794-datacomp-lm-dclm|DCLM]] · [[2023-05-17-arxiv-2305-10429-doremi-data-mixtures|DoReMi]] · [[2021-07-14-arxiv-2107-06499-deduplicating-training-data|Dedup]]. Synthetic/tokenization: [[2022-12-20-arxiv-2212-10560-self-instruct|Self-Instruct]] · [[2023-06-20-arxiv-2306-11644-textbooks-are-all-you-need-phi-1|phi-1]] · [[2023-05-03-arxiv-2305-02301-distilling-step-by-step|Distilling Step-by-Step]] · [[2025-09-16-arxiv-2509-13305-websailor-v2|WebSailor-V2]] · [[2015-08-31-arxiv-1508-07909-bpe-subword-units|BPE]] · [[2018-08-19-arxiv-1808-06226-sentencepiece|SentencePiece]]. Pretraining/scaling: [[2020-05-28-arxiv-2005-14165-gpt3-few-shot-learners|GPT-3]] · [[2026-06-22-arxiv-2001-08361-scaling-laws-for-neural-language-models|Kaplan]] · [[2022-03-29-arxiv-2203-15556-compute-optimal-chinchilla|Chinchilla]] · [[2022-06-15-arxiv-2206-07682-emergent-abilities|Emergent Abilities]] · [[2023-04-28-arxiv-2304-15004-emergence-mirage|Emergence Mirage]] · [[2022-02-11-arxiv-2202-05924-compute-trends-three-eras|Compute Trends]]. MoE: [[2026-06-22-arxiv-1701-06538-sparsely-gated-moe|Sparse MoE]] · [[2026-06-22-arxiv-2006-16668-gshard|GShard]] · [[2026-06-22-arxiv-2101-03961-switch-transformers|Switch]] · [[2026-06-22-arxiv-2401-04088-mixtral-of-experts|Mixtral]] · [[2026-06-22-arxiv-2401-06066-deepseekmoe|DeepSeekMoE]] · [[2026-06-22-arxiv-2412-19437-deepseek-v3-technical-report|DeepSeek-V3]]. Post-training: [[2022-03-04-arxiv-2203-02155-instructgpt|InstructGPT]] · [[2024-11-22-arxiv-2411-15124-tulu-3|Tülu 3]] · [[2023-07-18-arxiv-2307-09288-llama-2|Llama 2]] · [[2026-06-22-arxiv-2407-21783-llama-3-herd|Llama 3]] · [[2026-06-22-arxiv-2501-12948-deepseek-r1|DeepSeek-R1]] · [[2023-05-18-arxiv-2305-11206-lima-less-is-more-for-alignment|LIMA]] · [[2022-10-19-arxiv-2210-10760-scaling-laws-for-reward-model-overoptimization|RM Overoptimization]] · [[2023-05-29-arxiv-2305-18290-direct-preference-optimization|DPO]] · [[2022-12-15-arxiv-2212-08073-constitutional-ai|Constitutional AI]] · [[2023-09-01-arxiv-2309-00267-rlaif-vs-rlhf|RLAIF]]. Distillation: [[2026-06-22-arxiv-1503-02531-distilling-knowledge|Hinton]] · [[2026-06-22-arxiv-1606-07947-sequence-level-knowledge-distillation|Seq-KD]] · [[2026-06-22-arxiv-1910-01108-distilbert|DistilBERT]].

**January 2026**
- [[2026-01-08-arxiv-2601-04566v2-backdooragent-unified-backdoor-attacks]] — BackdoorAgent — stage-aware backdoor persistence
- [[2026-01-16-arxiv-2601-10955v2-stealthy-resource-amplification-tool-chains]] — Stealthy economic DoS via tool-calling chains (658×)
- [[2026-01-16-arxiv-2601-11816v1-polaris-typed-planning-governed-execution]] — POLARIS — typed planning + governed execution
- [[2026-01-18-arxiv-2601-12538v1-agentic-reasoning-survey]] — Agentic-reasoning roadmap survey
- [[2026-01-18-arxiv-2601-12560v1-agentic-ai-architectures-taxonomy]] — Unified agentic-AI taxonomy (perceive/brain/plan/act/tool/collaborate)
- [[2026-01-20-arxiv-2601-13671v1-orchestration-multi-agent-protocols-enterprise]] — MCP + A2A as complementary enterprise substrate
- [[2026-01-24-arxiv-2601-17435v1-dalia-declarative-agentic-layer-mcp]] — DALIA — declarative discovery/planning/execution over MCP

**February 2026**
- [[2026-02-01-arxiv-2602-00994v2-reasoning-vs-tooluse-interference-dart]] — Reasoning vs tool-use interference; DART decoupling
- [[2026-02-10-arxiv-2602-09598v1-elpo-error-localized-policy-optimization]] — ELPO — error-localized credit assignment
- [[2026-02-11-arxiv-2602-15055v1-acp-agent-communication-protocol-a2a]] — ACP — federated zero-trust agent communication protocol
- [[2026-02-12-arxiv-2602-12430v4-agent-skills-architecture-acquisition-security]] — Agent-skills survey; 26.1% of community skills vulnerable
- [[2026-02-24-arxiv-2602-20867v1-sok-agentic-skills-beyond-tool-use]] — SoK: agentic skills + ClawHavoc supply-chain attack
- [[2026-02-24-arxiv-2602-21320v1-tool-r0-self-evolving-zero-data]] — Tool-R0 — self-evolving tool agents from zero data

**March 2026**
- [[2026-03-07-arxiv-2603-07379v1-sok-agentic-rag-taxonomy]] — SoK: Agentic RAG as a POMDP; loop risks
- [[2026-03-09-arxiv-2603-10057v1-agentic-aiboms-supply-chain-provenance]] — Agentic AIBOMs — active supply-chain provenance
- [[2026-03-10-arxiv-2603-09134v1-agenticcyops-securing-enterprise-mas]] — AgenticCyOps — enterprise MAS security model
- [[2026-03-10-arxiv-2603-09716v1-autoagent-evolving-cognition-elastic-memory]] — AutoAgent — evolving cognition + elastic memory
- [[2026-03-13-arxiv-2603-13594v1-enterpriseops-gym-stateful-agentic-planning]] — EnterpriseOps-Gym — top model only 37.4%
- [[2026-03-16-arxiv-2603-15255v2-sage-multi-agent-self-evolution-reasoning]] — SAGE — 4-agent self-evolution with drift control

**April 2026**
- [[2026-04-09-arxiv-2604-07791v3-searl-policy-tool-graph-memory]] — SEARL — policy + tool-graph memory self-evolution
- [[2026-04-10-arxiv-2604-09813v1-covert-verifiable-tooluse-data-synthesis]] — COVERT — verifiable tool-use data synthesis for RL
- [[2026-04-23-arxiv-2604-21816v1-tool-attention-mcp-tax]] — The 'MCP tax'; gated lazy tool loading (−95% tokens)

**May 2026**
- [[2026-05-04-arxiv-2605-04107v1-tscg-tool-schema-compilation]] — TSCG — schema compilation restores small-model tool use
- [[2026-05-07-arxiv-2605-06869v2-agentick-unified-sequential-decision-benchmark]] — Agentick — RL/LLM/VLM/human on common ground
- [[2026-05-13-arxiv-2605-14102v2-chromaflow-negative-ablation-orchestration]] — ChromaFlow — negative ablation of orchestration
- [[2026-05-22-arxiv-2605-24069v1-mcp-poisoning-tool-description-attacks]] — MCP poisoning (TDP) benchmark; 'Firewall Fallacy'
- [[2026-05-31-arxiv-2606-01416v1-self-healing-agentic-orchestrators]] — Self-healing orchestrators (98.8% success)

**June 2026**
- [[2026-06-01-arxiv-2606-01801v1-metaforge-self-evolving-tool-forging]] — MetaForge — forge & recycle tools on demand
- [[2026-06-01-arxiv-2606-02132v2-eapo-learning-when-not-to-act]] — EAPO — learning when NOT to act (tool-abuse)
- [[2026-06-02-arxiv-2606-04051v1-rubas-rubric-based-rl-agent-safety]] — RUBAS — rubric-based RL for agent safety
- [[2026-06-11-arxiv-2606-14790v1-xflow-executable-protocol-multi-agent]] — XFlow — compiled protocol language for prompt↔harness
- [[2026-06-18-arxiv-2606-19704v1-predictive-validity-agent-evaluation]] — Predictive validity over aggregate leaderboards

### Surveys & SoK (deep-ingested)
- [[surveys-2026]] — 12 authoritative surveys, one per theme (security, memory, KG, protocols, reliability, coding, robotics, clinical, finance, RL, reasoning) + 3 ingested earlier

### arXiv — census auto-notes (top-ranked + full KG, abstract-only)
- [[census-2026-catalog]] — 975 lightweight auto-ingested notes (incl. all 297 knowledge-graph papers), grouped by month, each linked into the concept/entity graph (`wiki/sources/census-2026/`)

### 2025 — citation-ranked deep notes
- [[2025-deep-catalog]] — 381 full-text-backed notes, citation-ranked (Semantic Scholar), graph-linked (`wiki/sources/2025-deep/`)
- Landmark systems: [[a-mem]] · [[mem0]] · [[ui-tars]] · [[alphaevolve]] · [[search-o1]] · [[agent-laboratory]] · [[retool]] · [[browsecomp]] · [[kimi-k2]] · [[glm-45]]
- `raw/arxiv/2025-census/CITATIONS.md` — full citation ranking + caveats
- `raw/arxiv/2025-census/INDEX.md` — exhaustive 12,046-paper 2025 census

### Perspective — blogs, people & debates *(blog-scanner)*
- [[debate-llms-path-to-agi]] — Are LLMs the path to AGI, or a detour? ([[yann-lecun]] vs [[sonya-huang]])
- [[2026-01-14-blog-sonya-huang-2026-this-is-agi]] — Sequoia: 'long-horizon agents are AGI'
- [[2026-01-22-interview-yann-lecun-ami-labs]] — LeCun: 'LLMs are a dead end' (world models / JEPA)
- [[debate-agents-vs-workflows]] — Simple workflows, or autonomous agents? ([[anthropic]] vs autonomy)
- [[debate-prompt-injection-solvable]] — Is prompt injection solvable? ([[simon-willison]] vs design-by-construction)
- [[debate-ai-existential-risk]] — How seriously to take AI x-risk? ([[geoffrey-hinton]] · [[jan-leike]] vs [[yann-lecun]] · [[nathan-lambert]])
- [[debate-evals-vs-frameworks]] — Is the bottleneck evals or the framework? ([[hamel-husain]] vs orchestration camp)
- [[2025-06-16-blog-willison-lethal-trifecta]] · [[2024-12-19-blog-anthropic-building-effective-agents]] · [[2025-06-09-blog-lambert-what-comes-next-rl]]
- Frontier-lab blogs *(2025–26)*: OpenAI (Deep Research, Agents SDK, Codex, ChatGPT agent, AgentKit) · Anthropic (multi-agent research, context engineering, code-execution-with-MCP, long-running harnesses) · DeepMind/HF/Mistral
- Lab researchers: [[jason-wei]] (asymmetry of verification, RL life-lessons) · [[jan-leike]] (is alignment solved?)

## Census (exhaustive)
- `raw/arxiv/2026-census/INDEX.md` — all 11,191 agents-centric 2026 papers (Jan–Jun), ranked per month
- Categories: cs.AI/CL/LG/MA + cs.SE/RO/HC/IR/DB (expanded 2026-06-21, +1,296 papers)
- `raw/arxiv/2026-census/census-2026.jsonl` — full machine-readable records

## Overview
- [[overview|Overview]] — current state-of-the-radar synthesis.
