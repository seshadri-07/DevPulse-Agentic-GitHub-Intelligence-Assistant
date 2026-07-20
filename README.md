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


