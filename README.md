# 🤖 CryptoSentinel

[![n8n](https://img.shields.io/badge/Workflow-n8n-FF6D5A?style=for-the-badge&logo=n8n)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/Model-GPT--4o-412991?style=for-the-badge&logo=openai)](https://openai.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
![Status](https://img.shields.io/badge/Status-Production%20Ready-success?style=for-the-badge)

> **24/7 Autonomous Crypto Market Sentinel & Sentiment Intelligence Assistant.**  
> Condenses hours of cross-market news research into a high-conviction 30-second briefing using GPT-4o and n8n.

---

## 🎯 What Does It Do?

Instead of spending hours monitoring fragmented Twitter threads and news feeds, **CryptoSentinel** automates the entire surveillance cycle in **under 30 seconds**:

*   **Multi-Source Scraper:** Scrapes 9 premier crypto news publications simultaneously.
*   **Noise Filtering:** Eliminates redundant clickbait and extracts asset-specific developments.
*   **Sentiment Extraction:** Leverages GPT-4o to calculate sentiment polarity (Bullish / Neutral / Bearish).
*   **Telegram Delivery:** Dispatches formatted, executive briefings directly to Telegram.
*   **Continuous Surveillance:** Operates 24/7/365 with zero human intervention.

> **Single Command:** Send `"BTC"` or `"SOL"` to your bot → **30 seconds later:** Complete verified sentiment and breaking news dossier.

---

## ✨ Key Features

```
┌─────────────────────────────────┐
│  9 Major Crypto News Sources    │
│  (CoinDesk, Cointelegraph, etc.)│
└─────────────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐       ┌─────────────────────────────────┐
│  Keyword & Token Filter         │ ────> │  GPT-4o Sentiment Analysis      │
│  (GPT-4o-mini Extraction)       │       │  Bullish / Neutral / Bearish    │
└─────────────────────────────────┘       └─────────────────────────────────┘
                                                           │
                                                           ▼
                                          ┌─────────────────────────────────┐
                                          │  Telegram Instant Intelligence  │
                                          │  (30-Second Formatted Briefing) │
                                          └─────────────────────────────────┘
```

### 1. 📰 Multi-Source Real-Time Aggregator
Scrapes and parses breaking headlines across 9 leading outlets:
*   **Cointelegraph** - Top volume breaking market updates
*   **CoinDesk** - Institutional and regulatory analysis
*   **Bitcoin Magazine** - Bitcoin core ecosystem and macro news
*   **NewsBTC** - Real-time market flow and technical summaries
*   **Bitcoinist** - In-depth market developments
*   **CryptoPotato** - Trending token developments
*   **99Bitcoins** - Fundamental and educational coverage
*   **CryptoBriefing** - Research-driven project reports
*   **Crypto.news** - Global industry reporting

### 2. 🧠 Two-Tier AI Intelligence
*   **Tier 1 (GPT-4o-mini):** High-speed keyword matching and entity resolution.
*   **Tier 2 (GPT-4o):** Deep sentiment analysis, narrative context, and executive summary formulation.

### 3. ⚡ Ultra-Fast Turnaround
*   Average response latency: **30–60 seconds**.
*   Cross-source fact confirmation.
*   Webhook and Telegram command-triggered executions.

---

## 🛠️ Prerequisites & Setup

### Requirements
*   Self-hosted n8n instance or n8n Cloud account.
*   OpenAI API Key (GPT-4o & GPT-4o-mini access).
*   Telegram Bot Token (via [@BotFather](https://t.me/BotFather)).

### Step 1: Import the Workflow
1.  Download `cryptosentinel_workflow.json` from this repository.
2.  Open your n8n web dashboard and select **"Import from File"**.

### Step 2: Configure Credentials
Input your credentials in the corresponding nodes:
*   `OpenAI API Key` -> For the AI extraction and sentiment nodes.
*   `Telegram Bot API` -> For incoming message listener and response dispatch.

### Step 3: Activate & Test
*   Toggle the workflow to **Active**.
*   Open Telegram and message your bot:
    ```text
    ETH
    ```
*   Receive a comprehensive sentiment breakdown with key news citations within seconds.

---

**Developed & Maintained by:** [xCodeWraith DEV.](https://github.com/xCodeWraith)  
**License:** [MIT](LICENSE)
