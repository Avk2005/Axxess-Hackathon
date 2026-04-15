# MedVisor 🚀 AI-Powered Immersive Agent Platform

![Platform Preview](dashboard/frontend/public/prelude.png)

**An immersive AI platform that combines multi-agent systems, real-time 3D visualization, and cloud-native infrastructure to simulate intelligent coordination in dynamic environments.**

This project demonstrates how modern AI agents can collaborate, reason, and orchestrate decisions in a mission-based simulation environment. It integrates multimodal AI, distributed agent communication, real-time data processing, and scalable cloud deployment into a unified system.

DevPost Link: https://devpost.com/software/medvisor-5dclk8

---

## 🎯 Project Overview

This platform simulates a high-stakes coordination scenario where intelligent agents must:

- Generate contextual identities and assets using multimodal AI  
- Analyze geospatial and environmental data  
- Communicate across agent networks  
- Process incoming signals and system events  
- Coordinate group-level decisions in real time  

The system highlights:

- Multi-agent orchestration  
- Event-driven AI pipelines  
- Real-time participant tracking  
- Scalable cloud-native backend design  
- 3D interactive frontend visualization  

---

## 🧠 Core Capabilities

### 🔹 Multimodal AI Generation
- Multi-turn image generation  
- Context-aware prompt refinement  
- Identity and asset creation using large multimodal models  

### 🔹 Multi-Agent Systems
- Parallel agent execution  
- MCP (Model Context Protocol) integration  
- Agent-to-agent communication patterns  
- Distributed reasoning workflows  

### 🔹 Event-Driven Architecture
- Real-time event ingestion  
- Signal processing and state updates  
- Backend-triggered AI workflows  

### 🔹 3D Interactive Visualization
- Real-time map rendering  
- Live state updates  
- WebGL-based immersive interface  

---

## Run Web Server

bash`
cd ~/Axxess-Hackathon/level_1
source set_env.sh
uv run adk web
`

---


## 🛠️ Technology Stack

| Layer | Technologies |
|-------|-------------|
| **Frontend** | Next.js 14, Three.js, React Three Fiber, Tailwind CSS |
| **Backend** | FastAPI, Firestore, Firebase Storage |
| **AI / ML** | Vertex AI, Gemini 2.5 Flash, Veo 3.1 |
| **Agents** | Google ADK (Agent Development Kit), MCP (Model Context Protocol), OneMCP BigQuery |
| **Infrastructure** | Google Cloud Run, Cloud Build, Artifact Registry |
| **Database** | Firestore (events, users, state tracking) |

---

## 🏗️ System Architecture
Frontend (Next.js + 3D Visualization)
↓
Backend API (FastAPI on Cloud Run)
↓
Agent Layer (ADK + MCP + LLM Orchestration)
↓
Vertex AI (Multimodal Models)
↓
Firestore + Firebase Storage


The architecture supports:

- Stateless backend scaling  
- Event-driven AI execution  
- Agent parallelization  
- Real-time state synchronization  

---

## 🚀 Local Development

### Backend

```bash
cd dashboard/backend
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8080
Frontend
cd dashboard/frontend
npm install
npm run dev
☁️ Deployment

Designed for cloud-native deployment on Google Cloud:

gcloud builds submit --config cloudbuild.yaml

Key components:

Cloud Run (API hosting)

Firestore (state persistence)

Firebase Storage (media handling)

Vertex AI (model inference)

The backend scales to zero when idle and auto-scales under load.

💡 Design Highlights

Modular multi-level architecture

Clean separation between visualization and AI orchestration

Lightweight API-based agent invocation

Structured JSON outputs for state tracking

Cost-efficient, serverless infrastructure

📄 License

Apache 2.0 — See LICENSE for details.
