# 🚀 DevPulse – Agentic GitHub Intelligence Assistant

DevPulse is an Agentic AI-powered GitHub Intelligence Assistant that combines **LangGraph**, **Model Context Protocol (MCP)**, **Human-in-the-Loop (HITL)**, and **Agent-to-Agent (A2A)** concepts to provide real-time GitHub repository insights.

Unlike traditional chatbots, DevPulse can reason, select tools dynamically, request human approval before executing actions, retrieve live information from GitHub using MCP tools, and coordinate specialist agents using LangGraph.

---

# Features

- Agentic AI Architecture
- LangGraph Multi-Agent Workflow
- Model Context Protocol (MCP)
- Human-in-the-Loop (HITL) Approval
- Dynamic Tool Discovery
- Real-Time GitHub API Integration
- Short-Term Conversation Memory
- A2A Agent Card
- Supports Ollama and Groq LLMs
- Modular and Extensible Design

---

# Technologies Used

- Python 3.11+
- LangGraph
- MCP (Model Context Protocol)
- OpenAI Compatible API
- Ollama
- Groq API
- GitHub REST API
- HTTPX
- Pydantic
- Rich Console

---

# File Description
| File               | Description                                                      |
| ------------------ | ---------------------------------------------------------------- |
| agent_core.py      | Single Agent implementation using ReAct + MCP + Human Approval   |
| langgraph_agent.py | LangGraph multi-agent workflow with router and specialist agents |
| MCP_server.py      | MCP server exposing GitHub tools                                 |
| MCP_bridge.py      | Connects the AI agent with the MCP server                        |
| MCP_client_test.py | Test client for MCP server                                       |
| model_client.py    | Connects to Ollama or Groq                                       |
| a2a_card.py        | Agent Card for Agent-to-Agent communication                      |
| requirements.txt   | Required Python libraries                                        |

# Project Architecture

```

User
│
▼
LangGraph Router
│
├──────────────┬──────────────┐
▼ ▼ ▼
Repo Analyst Issue Agent Release Agent
│ │ │
└─────── MCP Bridge ─────────┘
│
▼
MCP Server
│
▼
GitHub REST API

---


