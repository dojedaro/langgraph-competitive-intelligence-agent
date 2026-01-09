# 🧠🕸️ LangGraph AI Agent for Competitive Intelligence (Retail)

An end-to-end **LangGraph-powered competitive intelligence agent** that helps retail businesses analyze nearby clothing-store competitors, estimate **footfall patterns**, and generate **investor-ready reports**.

This project demonstrates agentic workflow design (LangGraph), tool integration (Google Places), and structured report generation—turning what would normally be hours of manual market research into a repeatable pipeline.

---

## 🚀 What This Agent Does

✅ **Discovers nearby clothing store competitors** (real-time) using **Google Places API**  
✅ **Segments competitors** (market leaders, direct competitors, indirect competitors)  
✅ **Estimates footfall patterns & peak hours** using a proxy heuristic (review count / popularity factor)  
✅ **Optimizes operating hours & staffing strategy** based on predicted demand  
✅ Produces:
- 📄 **Full business intelligence report** (Markdown-ready)
- 📋 **Executive summary** for quick stakeholder review

---

## 🧩 Pipeline Overview (7 Tasks)

This notebook is organized as a clear, modular pipeline:

1. 🔐 **Secure API setup** (hidden input using `getpass`)
2. 📍 **Google Places data retrieval** (nearby clothing stores)
3. 🧠 **LangGraph agent creation** (StateGraph + ToolNode + conditional routing)
4. 🏪 **Competitor analysis node** (leaders vs direct vs indirect)
5. 📈 **Footfall prediction node** (weekday/weekend patterns + staffing & revenue ideas)
6. 📝 **Report generation node** (full report + exec summary)
7. ✅ **End-to-end integration test** (complete workflow run)

---

## 📦 Repository Structure

```txt
langgraph-competitive-intelligence-agent/
├── notebook/
│   └── LangGraph_Pipeline.ipynb
└── README.md
