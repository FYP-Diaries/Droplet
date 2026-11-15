# 💧 Droplet — Visual AI Agentic Workflow Builder

&gt; **A No-Code Visual Automation Platform Powered by AI Agents, RAG, and Server-Side Execution.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: In Development](https://img.shields.io/badge/Status-In%20Development-yellow.svg)]()
[![Stack: React + FastAPI + Supabase](https://img.shields.io/badge/Stack-React%20%2B%20FastAPI%20%2B%20Supabase-green.svg)]()

---

## 📌 Project Overview

**Droplet** is an intuitive, web-based, no-code visual workflow builder designed to democratize AI automation for non-technical users. Existing platforms like Zapier, n8n, and Flowise often demand technical setup, JSON configuration, or code writing. 

Droplet bridges this gap by providing:
1. **Interactive Visual Canvas**: Drag-and-drop workflow design using custom nodes and edges.
2. **Form-Based Node Configuration**: Zero raw code—configure node actions, triggers, and parameters exclusively through dynamic side drawers.
3. **Server-Side Execution Engine**: Independent, graph-parsed sequential and conditional execution running asynchronously on the server.
4. **Native RAG Integration**: Attach PDF/DOCX documents to AI nodes using `Supabase pgvector` embeddings for grounded document querying.
5. **System Onboarding SLM Copilot**: Built-in Small Language Model assistant to guide setup and diagnose workflow execution errors in plain English.

---

## 🏗️ Architecture &amp; Core Modules

The platform is divided into **10 core functional modules**:

```

[ Visual Canvas ] ──► [ Form Config Drawer ] ──► [ Workflow Engine ] ──► [ Integrations (Slack/Notion) ] │ │ ▼ ▼ [ SLM Copilot Assistant ] [ Supabase Postgres + pgvector ]

```

| Module ID | Module Name | Primary Responsibility |
| :--- | :--- | :--- |
| **Module I** | Visual Canvas &amp; Graph Editor | **Ifra Ahmed** |
| **Module II** | Form-Based Node Drawer UX | **Fayzan Mahmood** |
| **Module III** | Server-Side Execution Engine | **Ifra Ahmed** |
| **Module IV** | OAuth Integration Layer (Slack, Notion, Google) | **Fayzan Mahmood** |
| **Module V** | AI Agent &amp; RAG Vector Pipeline | **Fayzan &amp; Ifra** |
| **Module VI** | User Auth &amp; Access Control | **Fayzan &amp; Ifra** |
| **Module VII** | Data Persistence &amp; Supabase Schema | **Ifra Ahmed** |
| **Module VIII**| Fine-Tuned SLM Copilot Serving | **Fayzan &amp; Ifra** |
| **Module IX** | Execution Monitoring &amp; Activity Logs | **Fayzan Mahmood** |
| **Module X** | Cloud Infrastructure &amp; CI/CD Deployment | **Fayzan &amp; Ifra** |

---

## 🛠️ Tech Stack

* **Frontend**: React.js, React Flow, Tailwind CSS, Lucide Icons
* **Backend Engine**: Python (FastAPI) / Node.js
* **Database &amp; Auth**: PostgreSQL via Supabase (JSONB payloads + `pgvector` for RAG)
* **AI &amp; Embeddings**: Fine-Tuned SLM, LangChain / LlamaIndex, OpenAI / HuggingFace Embeddings
* **OAuth Integrations**: Slack API, Notion API, Google Workspace API, Trello API

---

## 🚀 Getting Started (Local Development)

### 1. Repository Setup
```bash
# Clone the repository
git clone [suspicious link removed]
cd droplet

```

### 2\. Frontend Setup

```
cd frontend
npm install
npm start

```

The client app will be running at `http://localhost:3000`.

### 3\. Backend Setup

```
cd ../backend
# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Start backend server
uvicorn app.main:app --reload

```

The API engine will be running at `http://localhost:8000`.

---

## 👥 Project Team &amp; Supervision

* **Student Team**:
  * **Fayzan Mahmood** (Registration No: CIIT/FA23-BCS-046)
  * **Ifra Ahmed** (Registration No: CIIT/FA23-BCS-173)
* **Supervised By**: **Ms. Maha Rasheed**
* **Department**: Department of Computer Science, COMSATS University Islamabad (CUI)

---

## 📄 License

This project is developed as a Bachelor's Final Year Project (FYP) under COMSATS University Islamabad guidelines.

---
