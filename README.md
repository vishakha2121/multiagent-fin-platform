# 🤖 FinAgent AI — Multi-Agent Financial Intelligence Platform

> **An AI-powered financial analysis platform where 5 autonomous agents collaborate to deliver budgeting, forecasting, risk detection, compliance checks, and investment insights — all orchestrated intelligently.**

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-green.svg)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-18-61DAFB.svg)](https://reactjs.org)
[![Gemini](https://img.shields.io/badge/Gemini-API-orange.svg)](https://ai.google.dev)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎬 What is FinAgent AI?

**FinAgent AI** is a next-generation **Multi-Agent Financial Intelligence Platform** that simulates an entire finance team using AI. Instead of one monolithic model, it uses **5 specialized autonomous agents** that work together — just like a real finance department.

Each agent has a **distinct role, domain expertise, and reasoning capability**, powered by **Google Gemini** and **Machine Learning models**. An **Orchestrator** coordinates them all to produce a unified financial intelligence report.

---

## 🧠 The 5 Autonomous Agents

| # | Agent | Role | Tech Used |
|---|-------|------|-----------|
| 1️⃣ | **Budget Agent** | Allocates company budget across departments | Gemini + Rule Engine |
| 2️⃣ | **Forecast Agent** | Predicts future revenue/expenses (3-6 months) | Prophet + Gemini |
| 3️⃣ | **Risk Agent** | Detects anomalies & fraud in transactions | Isolation Forest + Gemini |
| 4️⃣ | **Compliance Agent** | Checks GST/TDS/Tax rule violations | Rules Engine + Gemini |
| 5️⃣ | **Investment Agent** | Suggests smart investment portfolios | Gemini + Portfolio Logic |

### 🎼 Plus: The Orchestrator
A master coordinator that **runs all 5 agents in parallel**, aggregates their outputs, and generates a **unified financial intelligence report**.

---

## ✨ Key Features

- 🎯 **Multi-Agent Coordination** — 5 independent AI agents working in sync
- 🧠 **Gemini-Powered Reasoning** — LLM for financial insights & explanations
- 📊 **ML-Driven Anomaly Detection** — Isolation Forest for fraud detection
- 📈 **Time-Series Forecasting** — Prophet model for revenue prediction
- ⚖️ **Automated Compliance Checks** — GST, TDS, Income Tax validation
- 💰 **Smart Investment Suggestions** — Risk-profiled portfolio recommendations
- 🎨 **Beautiful React Dashboard** — Dark-themed, animated, responsive UI
- 🗄️ **SQLite Database** — Zero-setup, CPU-friendly, persistent storage
- 🔄 **Agent Orchestration** — Parallel execution with result aggregation
- 📄 **Exportable Reports** — PDF/CSV download support
- 🖥️ **CPU-Friendly** — Runs perfectly without GPU
- 🔐 **JWT Auth** — Secure API access

---

## 🏗️ Architecture



---

## 🛠️ Tech Stack

### Backend
- **Python 3.10+**
- **FastAPI** — Modern async web framework
- **Uvicorn** — ASGI server
- **SQLAlchemy** — ORM
- **SQLite** — Lightweight database
- **Google Gemini API** — LLM reasoning
- **Pandas + NumPy** — Data processing
- **Scikit-learn** — ML models
- **Prophet** — Time-series forecasting
- **Pydantic** — Data validation
- **Python-JOSE** — JWT auth

### Frontend
- **React 18** — UI library
- **Vite** — Build tool
- **TailwindCSS** — Styling
- **Framer Motion** — Animations
- **Recharts** — Charts
- **Axios** — HTTP client
- **React Router** — Navigation
- **Lucide React** — Icons

### Database
- **SQLite** — Zero-setup, CPU-friendly

---

## 📁 Project Structure



---

## 🚀 Quick Start

### Prerequisites

- **Python 3.10+** → [Download](https://www.python.org/downloads/)
- **Node.js 18+** → [Download](https://nodejs.org/)
- **Git** → [Download](https://git-scm.com/)
- **Gemini API Key** → [Get free key](https://aistudio.google.com/app/apikey)

---

### 🔧 Backend Setup

```bash
# 1. Navigate to backend
cd backend

# 2. Create virtual environment
python -m venv venv

# 3. Activate venv
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Setup environment variables
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY

# 6. Initialize database
python database/init_db.py

# 7. Seed sample data
python database/seed_data.py

# 8. Run backend server
uvicorn main:app --reload --port 8000


# 1. Open a NEW terminal and navigate to frontend
cd frontend

# 2. Install dependencies
npm install

# 3. Setup environment variables
cp .env.example .env
# Edit .env if needed (default API URL: http://localhost:8000)

# 4. Run frontend
npm run dev