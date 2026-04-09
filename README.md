# 📊 FinAgent Pro — AI-Powered Financial Intelligence

**FinAgent Pro** is a next-generation AI-driven financial analysis platform built with **Streamlit + CrewAI + Gemini**.  
It enables users to analyze stocks in real-time, combining **market data, news insights, and AI-driven strategy** into a concise institutional-grade report.

---

## 🚀 Features

- 🤖 **Multi-Agent AI System (CrewAI)**
  - Research Agent → Fetches stock data & news  
  - Analysis Agent → Generates sentiment & strategy  
  - Orchestrator → Produces final report  

- 📈 **Real-Time Stock Data**
  - Price, volatility, trend
  - Revenue, EPS, P/E ratio, Market Cap  
  - Powered by `yfinance`

- 📰 **Latest Market News**
  - Scrapes top 3 Yahoo Finance headlines

- 🧠 **AI-Powered Insights (Gemini)**
  - Sentiment classification (Positive / Neutral / Negative)
  - Actionable one-line strategy

- 🎨 **Beautiful UI**
  - Modern gradient-based design
  - Interactive dashboards
  - Institutional-style reporting interface

---

## 🏗️ Tech Stack

- **Frontend:** Streamlit  
- **AI Orchestration:** CrewAI  
- **LLM:** Google Gemini (`gemini-2.5-flash-lite`)  
- **Data Sources:**  
  - Yahoo Finance (`yfinance`)  
  - Web scraping (`BeautifulSoup`)  
- **Backend Tools:**  
  - LangChain  
  - Pydantic  

---

## ⚙️ How It Works

1. User enters a query, e.g., `Analyze Tesla last month`.
2. System pipeline:
   - Extracts **ticker + time period**
   - Normalizes period (e.g., "last month" → `1mo`)
   - Fetches:
     - Stock data via `yfinance`
     - News via Yahoo Finance scraping
   - AI agents:
     - Analyze trends + volatility + news
     - Generate sentiment + strategy
     - Produce final report

---

## 🧠 Agent Architecture

### 🔹 Research Agent
- Fetches structured stock + news data
- Uses:
  - `YahooFinanceTool`
  - `NewsScraperTool`
  - `normalize_period`

### 🔹 Analysis Agent
- Interprets:
  - Price movement
  - Volatility
  - Market sentiment
- Outputs:
  - Sentiment
  - Strategy

### 🔹 Orchestrator Agent
- Combines all outputs
- Produces final report

---

## 💻 How to Run 

Use the following link on Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1twY86MkbxHFwf-2IaTjUs4_Vx4L_s-iW)
