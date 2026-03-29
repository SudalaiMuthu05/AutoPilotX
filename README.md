# 🚀 AutoPilotX – Autonomous Workflow Intelligence System

AutoPilotX is an AI-powered platform that transforms unstructured documents into intelligent, automated workflows with real-time monitoring and execution.

It automates enterprise operations like onboarding, task allocation, and invoice processing using OCR, LLMs, and workflow orchestration.

---

## 🧠 Overview

AutoPilotX enables organizations to process documents and execute workflows automatically:

- 📄 Resume → Candidate onboarding tasks  
- 📞 Meeting transcript → Task extraction & assignment  
- 💰 Invoice → Validation & finance routing  

The system provides real-time visibility through a dynamic dashboard with logs, analytics, and workflow health monitoring.

---

## 🎯 Problem Statement

Organizations face challenges such as:

- Manual processing of unstructured data  
- Inefficient task assignment  
- Lack of real-time workflow visibility  
- Delayed execution and decision-making  
- No centralized automation system  

---

## 🚀 Solution

AutoPilotX introduces a fully autonomous pipeline:

- Extracts data using OCR + AI  
- Converts to structured JSON  
- Validates inputs  
- Generates and assigns tasks  
- Sends notifications automatically  
- Updates dashboard in real-time  

---

## 🔄 System Workflow


User Upload → OCR/PDF Parser → AI Extraction → JSON → Validation → Execution → Database → Email → Dashboard


---

## 🏗️ Architecture


Frontend (React + Tailwind + Framer Motion)
↓
API Layer (Axios)
↓
Backend (FastAPI)
↓
AI Engine (OCR + LLM)
↓
Workflow Engine (LangGraph)
↓
Database (Supabase)
↓
Email Service


---

## 🧩 Core Modules

### 1️⃣ Resume-Based Onboarding
- Extracts candidate details from resume  
- Generates personalized onboarding tasks  
- Sends automated emails  

---

### 2️⃣ Meeting Transcript Automation
- Converts meeting discussions into tasks  
- Assigns tasks to team members  
- Stores and tracks execution  

---

### 3️⃣ Invoice Processing System
- Extracts invoice details using AI  
- Validates fields (amount, invoice number)  
- Routes to finance team  
- Logs all actions  

---

### 4️⃣ Workflow Health Monitoring
- Tracks system performance  
- Computes failure rates  
- Displays status:
  - 🟢 Healthy  
  - 🟡 Warning  
  - 🔴 Critical  

---

## ⚙️ Tech Stack

### 🖥️ Frontend
- React (Vite)
- Tailwind CSS
- Framer Motion
- Axios

### ⚙️ Backend
- FastAPI
- LangGraph
- LangChain

### 🤖 AI & Processing
- Tesseract OCR
- LLM (OpenAI / Groq)

### 🗄️ Database
- Supabase

### 🔄 Background Processing
- Celery
- Redis

---

## 📊 Features

- 🤖 AI-powered automation  
- 📄 OCR + document understanding  
- 🔄 End-to-end workflow execution  
- 📊 Real-time dashboard  
- 📧 Automated email notifications  
- 🧠 Intelligent validation engine  
- 🔍 Full audit logging  
- ⚡ Self-healing workflows  
- 📈 Workflow health monitoring  

---

## 🖼️ UI Highlights

- Modern SaaS dashboard  
- Real-time activity feed  
- Workflow timeline visualization  
- Animated interactions (Framer Motion)  
- System health monitoring  

---

## 🚀 Installation

### 1️⃣ Clone the Repository

bash :
git clone https://github.com/SudalaiMuthu05/AutoPilotX.git
cd autopilotx
2️⃣ Backend Setup
pip install -r requirements.txt

Create .env file:

SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
OPENAI_API_KEY=your_api_key

Run backend:

python -m app.main
3️⃣ Frontend Setup
cd frontend
npm install
npm run dev
4️⃣ Start Background Worker (Celery)
celery -A app.celery_worker.celery_app worker --loglevel=info

Start Redis:

redis-server
🌐 API Endpoints
Endpoint	Description
POST /upload-resume	Resume onboarding
POST /upload-transcript	Meeting analysis
POST /upload-invoice	Invoice processing
GET /tasks	Fetch tasks
GET /invoices	Fetch invoices
GET /logs	Fetch logs

##📊 Dashboard Capabilities
Real-time updates (polling every 2 seconds)
Live activity feed
Workflow health computation
Interactive charts and analytics

##🔐 Authentication
Basic login/logout UI (frontend)
Session handling

##🧪 Testing
Upload a resume / transcript / invoice
Verify:
Data extraction
Task generation
Email notifications
Dashboard updates

##🚀 Future Enhancements
WebSocket real-time updates
AI-based anomaly detection
Role-based access control
Multi-language support
Cloud deployment

## 🏆 Conclusion
AutoPilotX transforms traditional manual workflows into intelligent, automated systems with real-time observability and AI-driven execution.
