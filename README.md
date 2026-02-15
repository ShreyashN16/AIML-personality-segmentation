# 🧠 AI-Based Personality Segmentation & Behavioral Classification System

An end-to-end Machine Learning project that predicts behavioral personality archetypes using structured psychometric-style features and multi-class classification models.

This project demonstrates how supervised learning techniques can be applied to behavioral analytics and personality-driven segmentation using synthetic yet statistically structured datasets.

---

## 🚀 Project Overview

The system takes numerical behavioral indicators (1–10 scale) such as:

- Emotional Availability  
- Career Prioritization  
- Trust Sensitivity  
- Communication Responsiveness  
- Social Energy  
- Romantic Inclination  
- Self-Growth Focus  
- Pickiness Level  
- Jealousy Index  
- Texting Frequency  

It predicts a personality archetype using probabilistic multi-class classification.

### Example Output Categories:

- Emotionally_Unavailable  
- Career_Obsessed  
- Overthinker  
- Too_Picky  
- Hopeless_Romantic  
- Main_Character_Energy  
- Situationship_Survivor  

The model returns:
- ✅ Predicted Class  
- 📊 Confidence Probability  
- 📈 Feature Importance  
- 🧩 Behavioral Radar Visualization  

---

## 🏗 Technical Architecture

### 🔹 Data Layer
- Synthetic dataset generation (2,000+ structured samples)
- Controlled feature distributions
- Balanced class representation
- Reproducible random seed

### 🔹 Machine Learning
- Logistic Regression
- Random Forest Classifier
- XGBoost
- Cross-validation
- Model comparison
- Confusion matrix analysis
- Probability-based inference
- SHAP explainability

### 🔹 Backend
- Python 3.10+
- FastAPI (REST API)
- Model serialization with Joblib

### 🔹 Frontend
- React + Vite
- Tailwind CSS
- Radar Charts (Recharts / Chart.js)
- Optional 3D UI elements (Three.js)

---

## 📊 Model Evaluation

- Multi-class classification metrics
- Accuracy comparison across models
- Cross-validation performance
- Feature importance ranking
- SHAP-based explainability

---

## 📁 Project Structure

```
singles_ai/
│
├── backend/
│   ├── train.py
│   ├── main.py
│   ├── utils.py
│   ├── model.pkl
│   └── data/
│
├── frontend/
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── App.jsx
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/ai-personality-segmentation.git
cd ai-personality-segmentation
```

### 2️⃣ Backend Setup

```bash
cd backend
pip install -r requirements.txt
python train.py
uvicorn main:app --reload
```

### 3️⃣ Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🧪 Applications & Relevance

This project demonstrates concepts used in:

- Behavioral Analytics  
- Consumer Segmentation  
- Marketing Intelligence Systems  
- HR Screening Tools  
- User Engagement Modeling  
- Personality-Based Recommendation Systems  

---

## 🎯 Key Learning Outcomes

- Designing structured synthetic datasets  
- Translating behavioral theory into ML features  
- Multi-class classification implementation  
- Model comparison & evaluation  
- Explainable AI integration (SHAP)  
- Full-stack ML deployment  

---

## 🔮 Future Improvements

- Real survey-based dataset integration  
- Hyperparameter tuning (GridSearch / Bayesian Optimization)  
- Advanced explainability dashboard  
- CI/CD pipeline  
- Cloud deployment (Render / Vercel / AWS)

---

## 📌 Disclaimer

This project is built for educational and experimental purposes.  
It demonstrates probabilistic behavioral classification and is not a psychological diagnostic tool.

---

## 🛠 Tech Stack

Python • Scikit-learn • XGBoost • SHAP • Pandas • NumPy • FastAPI • React • Tailwind CSS • Machine Learning • Explainable AI

---

## 💼 Resume Description (Optional)

Developed an end-to-end ML-based personality segmentation system using multi-class classification and explainable AI techniques, deployed with FastAPI and integrated with a modern React frontend.

---
<img>
