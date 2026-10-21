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
