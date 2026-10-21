# 🚀 Autonomous Open-Source AI Operations Hub

> An end-to-end automated system that crawls tech trends, analyzes them using local open-source AI insights, and orchestrates workflows with n8n and Telegram. Built for the **HF26 DEV Challenge**.

---

## 🏗️ System Architecture

This project is structured as a clean monorepo combining data scraping, AI-powered analysis, and workflow automation:

```text
ai-operations-hub/
│
├── scraper-agent/          # Module 1: Python Scraper & Ingestion (Python, BeautifulSoup, Requests)
│   ├── scraper.py
│   └── requirements.txt
│
├── ai-engine/              # Module 2: AI Analysis & RAG Pipeline (Data processing & local insights)
│   └── rag_engine.py
│
└── n8n-workflows/          # Module 3: Automation & Telegram Approval
    └── automation_hub_flow.json

```

---

## ⚙️ Core Modules

1. **Agentic Web Scraper (`scraper-agent/`)**:
* Autonomously collects trending articles and tech discussions.
* Cleans and formats raw data into structured JSON (`scraped_trends.json`).


2. **AI & RAG Engine (`ai-engine/`)**:
* Processes ingested data to generate smart technical summaries and relevance insights (`ai_insights.json`).


3. **n8n Workflow Automation (`n8n-workflows/`)**:
* Orchestrates daily scheduled runs, executes scripts via CLI, and sends interactive review prompts straight to Telegram (`Human-in-the-Loop`).



---

## 🛠️ Getting Started & Installation

### Prerequisites

* Python 3.8+
* n8n (Self-hosted or Cloud instance)
* Telegram Bot Token & Chat ID

### 1. Clone the Repository

```bash
git clone [https://github.com/YOUR_USERNAME/ai-operations-hub.git](https://github.com/YOUR_USERNAME/ai-operations-hub.git)
cd ai-operations-hub

```

### 2. Setup Module 1 (Scraper)

```bash
cd scraper-agent
pip install -r requirements.txt
python scraper.py

```

### 3. Setup Module 2 (AI Engine)

```bash
cd ../ai-engine
python rag_engine.py

```

### 4. Setup n8n Automation

* Import the workflow JSON file located in `n8n-workflows/automation_hub_flow.json` into your n8n instance.
* Update the file paths and Telegram credentials nodes according to your local environment.

---

## 💡 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [suspicious link removed].

## 📄 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).
