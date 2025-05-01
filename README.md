# Web-Scraping-Agent-with-N8N-and-MCP-Server
Web Scraping Agent with N8N and MCP Server
# 🤖 AI Scraping Agent in n8n with MCP Server

This project demonstrates how to create a powerful, AI-powered web scraping agent in [n8n](https://n8n.io/) using **MCP (Multi-Component Protocol)** and **Firecrawl**. The agent can receive a chat message, fetch relevant data from the internet via scraping, and respond intelligently using OpenAI or Claude models.

---

## 📌 Project Overview

This is the most beginner-friendly and hands-on tutorial for building an autonomous **Scraping Agent** with tools and memory capabilities using:

- 🧠 OpenAI Chat Model
- 🧰 MCP Tools
- 🗂️ Simple Memory
- 🌐 Firecrawl for web scraping

---

## 🧠 Agent Workflow (Chat-triggered)

The core agent is triggered when a chat message is received. It includes:

- **Chat Model**: Uses OpenAI (via OpenRouter)
- **Memory**: Context is maintained using Simple Memory
- **Tool**: Connects to MCP Client which communicates with the scraping server

### 🔧 Agent Setup

![Agent Workflow](./images/agent-workflow.png)

---

## 🖥️ MCP Server Workflow (Scraping Handler)

This is the actual scraping backend that receives the agent’s request, performs the scrape using Firecrawl, and sends structured results back.

### 🌐 MCP Server Setup

![MCP Server Workflow](./images/mcp-server-workflow.png)

---

## 🧩 Components Used

| Component            | Purpose                                  |
|----------------------|-------------------------------------------|
| `Agent (Tools Agent)`| Orchestrates AI, Memory, and Scraping     |
| `OpenAI Chat Model`  | Understands and responds to user queries |
| `Simple Memory`      | Stores previous messages / memory context|
| `MCP Client`         | Forwards tasks to the MCP server          |
| `MCP Server Trigger` | Starts the scraping backend               |
| `Scrape` Tool        | Uses Firecrawl to extract webpage data    |

---

## 📚 What You'll Learn

- How to create and coordinate multiple AI agents in n8n
- Connecting OpenAI models with real-time tools
- Setting up an MCP Server inside n8n
- Ethical scraping using Firecrawl
- Using the agent-as-a-tool pattern for modular AI

---

## ⚙️ Technologies Used

- [n8n](https://n8n.io/)
- [OpenRouter](https://openrouter.ai/)
- [Supabase](https://supabase.com/) (for optional DB storage)
- [QuickChart.io](https://quickchart.io/) (for optional visualization)
- [Firecrawl](https://firecrawl.dev/) for scraping
- [Claude / GPT-4] (for LLM reasoning)
- MCP Architecture

---


