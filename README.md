<div align="center">

# 🧪 Agentic AI

### A Comprehensive Collection of Agentic AI Patterns, Multi-Agent Systems & LLM Orchestration

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![LangGraph](https://img.shields.io/badge/LangGraph-FF6B6B?style=for-the-badge&logoColor=white)](https://github.com/langchain-ai/langgraph)
[![AutoGen](https://img.shields.io/badge/AutoGen-0078D4?style=for-the-badge&logoColor=white)](https://github.com/microsoft/autogen)
[![Google ADK](https://img.shields.io/badge/Google%20ADK-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://google.github.io/adk-docs)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Agentic Patterns](#agentic-patterns)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

---

## 📌 Overview

**Agentic AI** is a hands-on repository exploring production-grade agentic AI architectures and orchestration patterns. It covers implementations of:

- **ReAct** (Reasoning + Acting) agents
- **Plan-and-Execute** agent workflows
- **Multi-Agent Collaboration** with LangGraph and AutoGen
- **Google ADK** agent development
- **Memory, tool-use, and reflection** patterns for autonomous AI agents

This repo serves as both a learning resource and a reference implementation for engineers building AI agent systems.

---

## 🤖 Agentic Patterns

### 1. ReAct Agent
> Combines **reasoning** and **acting** in a loop: the agent thinks, takes an action, observes the result, then thinks again.

```
Thought -> Action -> Observation -> Thought -> ... -> Final Answer
```

### 2. Plan-and-Execute
> Separates planning from execution. A Planner LLM creates a step-by-step plan; an Executor LLM runs each step.

```
User Goal -> Planner (create plan) -> Executor (run steps) -> Result
```

### 3. Multi-Agent Collaboration (LangGraph)
> Multiple specialized agents collaborate on a task via a supervisor or graph-based routing.

```
Supervisor Agent
    ├── Research Agent
    ├── Analysis Agent
    └── Writer Agent
```

### 4. AutoGen Multi-Agent
> Microsoft AutoGen-based agent conversations with tool-use, code execution, and self-critique.

### 5. Google ADK Agents
> Google Agent Development Kit implementations for building production-ready AI agents on Google infrastructure.

---

## 🛠️ Tech Stack

| Framework | Purpose |
|---|---|
| **LangGraph** | Graph-based multi-agent orchestration |
| **LangChain** | LLM chains, tools, and memory |
| **AutoGen** | Microsoft multi-agent conversation framework |
| **Google ADK** | Google Agent Development Kit |
| **OpenAI GPT-4** | Primary LLM for reasoning and generation |
| **Google Gemini** | Alternative LLM via Google AI |
| **ChromaDB / FAISS** | Vector stores for RAG |
| **FastAPI** | API layer for serving agents |

---

## ⚙️ Prerequisites

- Python 3.8+
- OpenAI API key
- Google AI API key (for Gemini-based agents)

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Manideep-Kanna/Agentic-AI.git
cd Agentic-AI
```

### 2. Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔧 Configuration

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key
GOOGLE_API_KEY=your_google_api_key
```

---

## 🏃 Usage

Each agent pattern is implemented as a standalone Python script or Jupyter notebook. Navigate to the relevant directory and run:

```bash
# Example: Run a ReAct agent
python react_agent.py

# Example: Run LangGraph multi-agent workflow
python langgraph_multiagent.py
```

---

## 🎓 Learning Resources

- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/)
- [AutoGen Documentation](https://microsoft.github.io/autogen/)
- [Google ADK Documentation](https://google.github.io/adk-docs/)
- [LangChain Agents](https://python.langchain.com/docs/modules/agents/)

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-agent-pattern`
3. Commit your changes: `git commit -m 'feat: add new agent pattern'`
4. Push to the branch: `git push origin feature/your-agent-pattern`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

Made with ❤️ by [Manideep Sitaram Kanna](https://github.com/Manideep-Kanna)

</div>
