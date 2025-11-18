MediBot – AI Symptom Checker

MediBot is an AI-powered health assistant built with React + TypeScript + Vite (Frontend) and FastAPI + Machine Learning (Backend).
Users can enter symptoms, and the system predicts the most likely diseases with confidence scores.

 Live Demo

Frontend: (Add your Vercel URL here)
Backend API: (Add your Render API URL here)

 Features

✔ AI-based disease prediction

✔ Clean UI built with shadcn-ui

✔ TailwindCSS for styling

✔ Fully responsive

✔ FastAPI backend with ML model

✔ Top-3 disease predictions with confidence

✔ Input validation & safety checks

 Tech Stack
Frontend

React + TypeScript

Vite

Tailwind CSS

shadcn-ui

Axios

Backend

FastAPI

Python

Scikit-learn

Joblib

Pandas / NumPy

 Project Setup (Frontend)
# Clone the repo
git clone https://github.com/Kartikey1405/Medibot_Frontend.git

cd Medibot_Frontend

# Install dependencies
npm install

# Start development server
npm run dev

 Project Setup (Backend)
# Navigate to backend
cd MediBot_Backend   # if in a separate folder

# Install dependencies
pip install -r requirements.txt

# Run FastAPI
uvicorn app.main:app --reload


API will run at:

http://127.0.0.1:8000

 API Endpoints
POST /predict

Send symptoms and receive top 3 predictions.

{
  "symptoms": ["itching", "fatigue"]
}


Response:

{
  "predictions": [
    { "disease": "Arthritis", "confidence": 0.12 },
    { "disease": "Diabetes", "confidence": 0.08 },
    { "disease": "Migraine", "confidence": 0.07 }
  ]
}

 Folder Structure (Frontend)
src/
 ├─ components/
 ├─ pages/
 ├─ hooks/
 ├─ App.tsx
public/
 ├─ favicon.ico
 ├─ robots.txt
package.json
vite.config.ts
tailwind.config.ts

 Deployment
Frontend Deployment

Use Vercel:

Push your repo to GitHub

Import to Vercel

Build & deploy automatically

Backend Deployment

Use Render or Railway:

Choose “Deploy Web Service”

Select your repo

Add requirements.txt

Set Start Command:

uvicorn app.main:app --host 0.0.0.0 --port 10000

 License

This project is open-source and free to use.

 Author

Kartikey Kushagra
AI/ML Enthusiast • Full-Stack Developer
