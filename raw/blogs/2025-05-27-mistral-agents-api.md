# Build AI agents with the Mistral Agents API

Source: https://mistral.ai/news/agents-api
Author: Mistral AI
Date: May 27, 2025
Category: Product
Captured: 2026-06-22

---

Today we announce our new Agents API, a major step forward in making AI more capable, useful, and an active problem-solver.

Traditional language models excel at generating text but are limited in their ability to perform actions or maintain context. Our new Agents API addresses these limitations by combining Mistral's powerful language models with:

- Built-in connectors for code execution, web search, image generation, and MCP tools
- Persistent memory across conversations
- Agentic orchestration capabilities

The Agents API complements our Chat Completion API by offering a dedicated framework that simplifies implementing agentic use cases. It serves as the backbone of enterprise-grade agentic platforms.

By providing a reliable framework for AI agents to handle complex tasks, maintain context, and coordinate multiple actions, the Agents API enables enterprises to use AI in more practical and impactful ways.

## Mistral agents in action.

Explore the diverse applications of Mistral's Agents API across various sectors:

- **Coding assistant with Github.** An agentic workflow built with Mistral's agents API where an agent interacts with Github and oversees a developer agent, powered by DevStral to write code. The agent is granted full authority over Github, showcasing automated software development task management.
- **Linear tickets assistant.** An intelligent task coordination assistant powered by our Agents API, using multi-server MCP architecture to transform call transcripts to PRDs to actionable Linear issues and track project deliverables.
- **Financial analyst.** A financial advisory agent constructed with our Agents API, orchestrating multiple MCP servers to source financial metrics, compile insights, and archive results securely.
- **Travel assistant.** Helps users plan their trips, book accommodations, and manage travel needs.
- **Nutrition assistant.** AI-powered food diet companion to set goals, log meals, receive food suggestions, track achievements.

## Create an agent with built-in connectors and MCP tools.

Each agent can be equipped with powerful built-in connectors, which are tools that are deployed and ready for Agents to call on demand, and MCP tools:

- **Code execution** — execute Python code in a secure sandboxed environment (math, data visualization, scientific computing).
- **Image generation** — powered by Black Forest Lab FLUX1.1 [pro] Ultra.
- **Document library** — built-in connector to access documents from Mistral Cloud; powers integrated RAG.
- **Web search** — combine Mistral models with up-to-date information from web search. Agents with web search show significant improvement: in the SimpleQA benchmark, Mistral Large and Mistral Medium with web search achieve scores of 75% and 82.32%, respectively, compared to 23% and 22.08% without web search.
- **MCP tools** — the Agents API SDK can leverage tools built on the Model Context Protocol (MCP), an open, standardized protocol that enables seamless integration between agents and external systems. MCP tools provide a flexible and extensible interface for agents to access real-world context, including APIs, databases, user data, documents, and other dynamic resources.

## Memory and context with stateful conversations.

The Agents API provides robust conversation management through a flexible and stateful conversation system. Each conversation retains its context.

- **Conversation management** — start with an Agent (specific agent_id) or via Direct Access (specify model + completion params). Each conversation maintains structured history through conversation entries.
- **Stateful interactions and conversation branching** — developers can view past conversations, continue any conversation or initiate new conversation paths from any point.
- **Streaming output** — supported both when starting and continuing a conversation.

## Agent orchestration.

The true power lies in its ability to orchestrate multiple agents to solve complex problems. Through dynamic orchestration, agents can be added or removed from a conversation as needed.

- **Creating an agentic workflow** — create as many agents as needed, each with specific tools and models.
- **Agent handoffs** — define which agents can hand off tasks to others. For example, a finance agent might delegate tasks to a web search agent or a calculator agent. Handoffs enable a seamless chain of actions; a single request can trigger tasks across multiple agents.

## Get started.

Check out the docs, create your first agent, and start building.
