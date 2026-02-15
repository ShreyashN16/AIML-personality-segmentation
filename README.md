# Why Are You Still Single? - 3D AI Personality Experience 💔

A modern, interactive 3D web application that uses Machine Learning to brutally roast your dating life. 

![Project Banner](https://via.placeholder.com/1200x500.png?text=Why+Are+You+Still+Single%3F+AI+App)

## 🚀 Concept
This is **not** a basic form. It's an immersive experience.
- **Frontend**: React + Vite + Three.js + Framer Motion (Neon Glassmorphism UI)
- **Backend**: FastAPI + Python
- **AI Engine**: XGBoost / Random Forest trained on synthetic personality data
- **Explainability**: SHAP (SHapley Additive exPlanations) to tell you *exactly* why you're alone.

---

## 🛠 Tech Stack
- **ML/Backend:** Python, FastAPI, Scikit-Learn, Pandas, XGBoost, SHAP
- **Frontend:** React, TailwindCSS, Framer Motion, React-Three-Fiber
- **Deployment:** Render (Backend), Vercel (Frontend)

---

## 📦 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/singles-ai-3d.git
cd singles-ai-3d
```

### 2. Backend Setup (Python)
Navigate to the backend folder and install dependencies:
```bash
cd backend
python -m venv venv
# Windows
.\venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

pip install -r ../requirements.txt
```

**Important:** Generate data and train the model before running the server.
```bash
# Generate synthetic dataset (2000 samples)
python generate_data.py

# Train the ML models and save the best one
python train.py
```

Start the FastAPI server:
```bash
python main.py
# Server running at http://localhost:8000
```

### 3. Frontend Setup (React)
Open a new terminal, navigate to the frontend folder:
```bash
cd frontend
npm install
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) to view the app.

---

## 🌐 Deployment Guide

### Backend (Render.com)
1. Push code to GitHub.
2. Create a new **Web Service** on Render.
3. Connect your repo.
4. Settings:
   - **Root Directory**: `backend`
   - **Build Command**: `pip install -r ../requirements.txt && python train.py` (Run training on build)
   - **Start Command**: `uvicorn main:app --host 0.0.0.0 --port 10000`
   - **Environment Variables**: `PYTHON_VERSION` = 3.9

### Frontend (Vercel)
1. Import your repo to Vercel.
2. Settings:
   - **Root Directory**: `frontend`
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - **Framework Preset**: Vite
3. **Environment Variable**: `VITE_API_URL` = (Your Render Backend URL)

---

## 🧠 ML Model Details
We trained 3 models (`LogisticRegression`, `RandomForest`, `XGBoost`) on 10 behavioral features including:
- `reply_speed`
- `emotional_availability`
- `trust_issues`

The best performing model (typically RandomForest ~92% acc) is selected automatically.

---

## 🎨 Creative Direction
- **Vibe**: Gen-Z, Neon, Dark Mode, Brutal Honesty.
- **Visuals**: Floating 3D orbs, glass cards, smooth page transitions.

## 📄 License
MIT
