# 🧭 Driftaway Trip Planner – Full Stack MVP

Driftaway is an intelligent trip planning assistant that blends conversational AI with deterministic modules. This MVP showcases a modular backend (FastAPI), a reactive frontend (React/Vite/TailwindCSS), and cloud-native deployment via Docker and Render.

## 🚀 Features

- 🧠 Conversational trip planning via /chat endpoint
- 🗺️ Modular MCPs for food, activities, and routing
- ⚡ FastAPI backend with mock and real toggles
- 🎨 Stateless frontend with backend-driven session history
- 🐳 Dockerized for local development and CI/CD
- 🛠️ Makefile for fast resets and clean orchestration

## 📦 Tech Stack

Frontend - React + Vite + TailwindCSS
Backend - FastAPI + Uvicorn

🧰 Installation

1. Clone the repo
   git clone https://github.com/your-username/driftaway.git
   cd driftaway

2. Set up environment variables
   Create a .env file in backend/ and frontend/ if needed. Example:
   FIREBASE_SERVICE_ACCOUNT=<path of your firebase service account>
   GEMINI_API_KEY=<your api key>
   SNIP_SMART_URL=http://snipsmart:5000/snip-json

3. Build and run with Docker
   make reset

This will:

- Tear down any existing containers
- Rebuild backend and frontend images
- Start fresh containers for both services

4. Access the app

- Frontend: http://localhost:5173
- Backend: http://localhost:4000

# 🛠️ Dev Commands

make reset # Rebuild and restart everything
make backend # Run backend only
make frontend # Run frontend only
make logs # Tail logs from all containers

# 🌐 Frontend

```
cd frontend
npm install
npm run build
npm run dev

```

Access at http://localhost:5173

🧠 Philosophy
This project is built for scale, clarity, and maintainability. It embraces:

- Modular orchestration
- Stateless frontend flows
- Backend-driven session state
- Clean separation of concerns
- Developer happiness via automation
