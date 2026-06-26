# How we built our multi-agent research system

- **Source:** Anthropic Engineering
- **URL:** https://www.anthropic.com/engineering/multi-agent-research-system
- **Published:** 2025-06-13
- **Authors:** Jeremy Hadfield, Barry Zhang, Kenneth Lien, Florian Scholz, Jeremy Fox, Daniel Ford
- **Captured:** 2026-06-22 (web_fetch, full text)

---

Our Research feature uses multiple Claude agents to explore complex topics more effectively. We share the engineering challenges and the lessons we learned from building this system.

Claude now has Research capabilities that allow it to search across the web, Google Workspace, and any integrations to accomplish complex tasks.

The journey of this multi-agent system from prototype to production taught us critical lessons about system architecture, tool design, and prompt engineering. A multi-agent system consists of multiple agents (LLMs autonomously using tools in a loop) working together. Our Research feature involves an agent that plans a research process based on user queries, and then uses tools to create parallel agents that search for information simultaneously. Systems with multiple agents introduce new challenges in agent coordination, evaluation, and reliability.

## Benefits of a multi-agent system

Research work involves open-ended problems where it's very difficult to predict the required steps in advance. You can't hardcode a fixed path for exploring complex topics, as the process is inherently dynamic and path-dependent. When people conduct research, they tend to continuously update their approach based on discoveries, following leads that emerge during investigation.

This unpredictability makes AI agents particularly well-suited for research tasks. Research demands the flexibility to pivot or explore tangential connections as the investigation unfolds. The model must operate autonomously for many turns, making decisions about which directions to pursue based on intermediate findings. A linear, one-shot pipeline cannot handle these tasks.

The essence of search is compression: distilling insights from a vast corpus. Subagents facilitate compression by operating in parallel with their own context windows, exploring different aspects of the question simultaneously before condensing the most important tokens for the lead research agent. Each subagent also provides separation of concerns—distinct tools, prompts, and exploration trajectories—which reduces path dependency and enables thorough, independent investigations.

Once intelligence reaches a threshold, multi-agent systems become a vital way to scale performance. For instance, although individual humans have become more intelligent in the last 100,000 years, human societies have become exponentially more capable in the information age because of our collective intelligence and ability to coordinate. Even generally-intelligent agents face limits when operating as individuals; groups of agents can accomplish far more.

Our internal evaluations show that multi-agent research systems excel especially for breadth-first queries that involve pursuing multiple independent directions simultaneously. We found that a multi-agent system with Claude Opus 4 as the lead agent and Claude Sonnet 4 subagents outperformed single-agent Claude Opus 4 by 90.2% on our internal research eval. For example, when asked to identify all the board members of the companies in the Information Technology S&P 500, the multi-agent system found the correct answers by decomposing this into tasks for subagents, while the single agent system failed to find the answer with slow, sequential searches.

Multi-agent systems work mainly because they help spend enough tokens to solve the problem. In our analysis, three factors explained 95% of the performance variance in the BrowseComp evaluation (which tests the ability of browsing agents to locate hard-to-find information). We found that token usage by itself explains 80% of the variance, with the number of tool calls and the model choice as the two other explanatory factors. This finding validates our architecture that distributes work across agents with separate context windows to add more capacity for parallel reasoning. The latest Claude models act as large efficiency multipliers on token use, as upgrading to Claude Sonnet 4 is a larger performance gain than doubling the token budget on Claude Sonnet 3.7. Multi-agent architectures effectively scale token usage for tasks that exceed the limits of single agents.

There is a downside: in practice, these architectures burn through tokens fast. In our data, agents typically use about 4× more tokens than chat interactions, and multi-agent systems use about 15× more tokens than chats. For economic viability, multi-agent systems require tasks where the value of the task is high enough to pay for the increased performance. Further, some domains that require all agents to share the same context or involve many dependencies between agents are not a good fit for multi-agent systems today. For instance, most coding tasks involve fewer truly parallelizable tasks than research, and LLM agents are not yet great at coordinating and delegating to other agents in real time. We've found that multi-agent systems excel at valuable tasks that involve heavy parallelization, information that exceeds single context windows, and interfacing with numerous complex tools.

## Architecture overview for Research

Our Research system uses a multi-agent architecture with an orchestrator-worker pattern, where a lead agent coordinates the process while delegating to specialized subagents that operate in parallel.

When a user submits a query, the lead agent analyzes it, develops a strategy, and spawns subagents to explore different aspects simultaneously. The subagents act as intelligent filters by iteratively using search tools to gather information, then returning a list to the lead agent so it can compile a final answer.

Traditional approaches using Retrieval Augmented Generation (RAG) use static retrieval. That is, they fetch some set of chunks that are most similar to an input query and use these chunks to generate a response. In contrast, our architecture uses a multi-step search that dynamically finds relevant information, adapts to new findings, and analyzes results to formulate high-quality answers.

Process: When a user submits a query, the system creates a LeadResearcher agent that enters an iterative research process. The LeadResearcher begins by thinking through the approach and saving its plan to Memory to persist the context, since if the context window exceeds 200,000 tokens it will be truncated and it is important to retain the plan. It then creates specialized Subagents with specific research tasks. Each Subagent independently performs web searches, evaluates tool results using interleaved thinking, and returns findings to the LeadResearcher. The LeadResearcher synthesizes these results and decides whether more research is needed—if so, it can create additional subagents or refine its strategy. Once sufficient information is gathered, the system exits the research loop and passes all findings to a CitationAgent, which processes the documents and research report to identify specific locations for citations. This ensures all claims are properly attributed to their sources.

## Prompt engineering and evaluations for research agents

Early agents made errors like spawning 50 subagents for simple queries, scouring the web endlessly for nonexistent sources, and distracting each other with excessive updates. Principles learned for prompting agents:

1. **Think like your agents.** Build simulations using the Console with the exact prompts and tools from the system, then watch agents work step-by-step. This reveals failure modes: agents continuing when they already had sufficient results, using overly verbose search queries, or selecting incorrect tools.
2. **Teach the orchestrator how to delegate.** Each subagent needs an objective, an output format, guidance on tools and sources to use, and clear task boundaries. Without detailed task descriptions, agents duplicate work, leave gaps, or fail to find necessary information.
3. **Scale effort to query complexity.** Embedded scaling rules in prompts: simple fact-finding requires just 1 agent with 3-10 tool calls, direct comparisons might need 2-4 subagents with 10-15 calls each, complex research might use more than 10 subagents with clearly divided responsibilities.
4. **Tool design and selection are critical.** Agent-tool interfaces are as critical as human-computer interfaces. With MCP servers, agents encounter unseen tools with descriptions of wildly varying quality. Gave agents explicit heuristics: examine all available tools first, match tool usage to user intent, prefer specialized tools over generic ones.
5. **Let agents improve themselves.** Claude 4 models can be excellent prompt engineers. Created a tool-testing agent—given a flawed MCP tool, it attempts to use the tool then rewrites the tool description to avoid failures. This resulted in a 40% decrease in task completion time for future agents using the new description.
6. **Start wide, then narrow down.** Prompt agents to start with short, broad queries, evaluate what's available, then progressively narrow focus.
7. **Guide the thinking process.** Extended thinking mode serves as a controllable scratchpad. The lead agent uses thinking to plan; subagents use interleaved thinking after tool results to evaluate quality and refine queries.
8. **Parallel tool calling transforms speed and performance.** Two kinds of parallelization: (1) the lead agent spins up 3-5 subagents in parallel rather than serially; (2) subagents use 3+ tools in parallel. These cut research time by up to 90% for complex queries.

Prompting strategy focuses on instilling good heuristics rather than rigid rules.

## Effective evaluation of agents

Evaluating multi-agent systems presents unique challenges. Even with identical starting points, agents might take completely different valid paths.

- **Start evaluating immediately with small samples.** In early agent development, changes tend to have dramatic impacts. A prompt tweak might boost success rates from 30% to 80%. Started with a set of about 20 queries representing real usage patterns. Best to start small-scale right away rather than delaying until you can build more thorough evals.
- **LLM-as-judge evaluation scales when done well.** Used an LLM judge evaluating each output against a rubric: factual accuracy, citation accuracy, completeness, source quality, and tool efficiency. Found a single LLM call with a single prompt outputting scores from 0.0-1.0 and a pass-fail grade was the most consistent and aligned with human judgements.
- **Human evaluation catches what automation misses.** Human testers noticed early agents consistently chose SEO-optimized content farms over authoritative but less highly-ranked sources like academic PDFs or personal blogs. Adding source quality heuristics resolved this.

Multi-agent systems have emergent behaviors. The best prompts are frameworks for collaboration that define division of labor, problem-solving approaches, and effort budgets.

## Production reliability and engineering challenges

- **Agents are stateful and errors compound.** Built systems that can resume from where the agent was when errors occurred. Combine the adaptability of AI agents with deterministic safeguards like retry logic and regular checkpoints.
- **Debugging benefits from new approaches.** Agents are non-deterministic between runs, even with identical prompts. Added full production tracing to diagnose why agents failed. Monitor agent decision patterns and interaction structures—without monitoring the contents of individual conversations, to maintain user privacy.
- **Deployment needs careful coordination.** Use rainbow deployments to avoid disrupting running agents, gradually shifting traffic from old to new versions while keeping both running.
- **Synchronous execution creates bottlenecks.** Lead agents currently execute subagents synchronously. Asynchronous execution would enable additional parallelism but adds challenges in result coordination, state consistency, and error propagation.

## Conclusion

When building AI agents, the last mile often becomes most of the journey. The compound nature of errors in agentic systems means minor issues for traditional software can derail agents entirely. Despite these challenges, multi-agent systems have proven valuable for open-ended research tasks.

## Appendix — additional tips

- **End-state evaluation** of agents that mutate state over many turns: evaluate whether it achieved the correct final state rather than judging the process.
- **Long-horizon conversation management:** agents summarize completed work phases and store essential information in external memory; spawn fresh subagents with clean contexts maintaining continuity through handoffs.
- **Subagent output to a filesystem to minimize the 'game of telephone':** subagents store work in external systems then pass lightweight references back to the coordinator, preventing information loss and reducing token overhead.

A Clio embedding plot shows the most common Research use cases: developing software systems (10%), develop/optimize professional and technical content (8%), develop business growth and revenue strategies (8%), academic research (7%), research/verify info about people/places/orgs (5%).
