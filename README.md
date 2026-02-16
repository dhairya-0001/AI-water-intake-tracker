# Water-Intake-Tracker

Enterprise-grade AI hydration monitoring platform.

## Prerequisites

- Docker & Docker Compose
- Node.js & npm
- Python 3.9+

## Running the System

### 1. Start Infrastructure (Database & Redis)

```bash
docker-compose up -d
```

### 2. Start Backend

```bash
cd backend
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### 3. Start Frontend

```bash
cd frontend
npm run dev
```

## Access

- **Backend API**: http://localhost:8000/docs
- **Frontend Dashboard**: http://localhost:3000

## AI Features

- **Hydration Prediction**: `/ai/predict/optimal/{user_id}`
- **Behavior Analysis**: `/ai/analyze/{user_id}`
- **Chat Assistant**: `/ai/chat/ask`
