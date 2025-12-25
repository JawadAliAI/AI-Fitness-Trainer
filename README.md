# 🏋️ FitBot - AI Fitness Assistant

<div align="center">

![FitBot Logo](https://img.shields.io/badge/FitBot-AI%20Fitness%20Coach-blue?style=for-the-badge&logo=dumbbell)

**"Your Personal AI-Powered Fitness Coach with Voice Interaction & AI Vision"**

[![React](https://img.shields.io/badge/React-18.3-61DAFB?style=flat-square&logo=react&logoColor=white)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Supabase](https://img.shields.io/badge/Supabase-Database-3ECF8E?style=flat-square&logo=supabase&logoColor=white)](https://supabase.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

[Features](#-features) • [Demo](#-demo) • [Installation](#-installation) • [API](#-api-documentation) • [Contributors](#-contributors)

</div>

---

## 📖 Overview

**FitBot** is a state-of-the-art AI fitness ecosystem designed to revolutionize your workout experience. Combining **Generative AI (LLMs)**, **Computer Vision (Pose Estimation)**, and **Interactive 3D Avatars**, FitBot provides a truly personalized coaching experience. Whether you're at home or the gym, FitBot tracks your form, answers your nutrition questions, and generates custom workout plans optimized for your goals.

### 🌟 Why FitBot?
- **Real-time AI Vision:** Tracks your form during exercises like pushups and lunges.
- **Natural Voice Conversations:** Talk to your trainer just like a real person.
- **Interactive 3D Coach:** A digital human that guides you through your fitness journey.
- **Smart Analytics:** Track your BMI, exercise history, and progress over time.

---

## ✨ Features

### 🤖 AI Digital Human Assistant
- **3D Avatar Integration:** An interactive digital human that responds to your queries.
- **Context-Aware Coaching:** Remembers your fitness history and goals for personalized advice.
- **Nuanced Responses:** Powered by Groq's LLaMA 3.3 70B for high-speed, intelligent chat.

### 👁️ AI Vision & Tracking
- **Pose Estimation:** Real-time exercise tracking using MediaPipe.
- **Rep Counter:** Automatically counts your reps for various exercises.
- **Form Correction:** Provides instant feedback to ensure safety and efficiency.

### 🎤 Intelligent Voice Interface
- **Speech-to-Text (STT):** Advanced voice recognition for hands-free interactions.
- **Text-to-Speech (TTS):** Natural-sounding AI voice for coaching and guidance.
- **Auto-Play:** Optional automatic playback of AI responses.

### 📚 Exercise & Nutrition
- **Video Library:** 50+ curated YouTube tutorials for perfect form.
- **Smart BMI:** Calculate your metrics and get instant health recommendations.
- **Custom Plans:** Fully tailored 3-day, 5-day, or 7-day workout routines.

---

## 📸 Demo

<div align="center">

| **Dashboard & Analytics** | **AI Fitness Chatbot** |
|:---:|:---:|
| ![Dashboard](docs/screenshots/dashboard.png) | ![AI Chat](docs/screenshots/ai-chat.png) |

| **3D AI Avatar** | **Exercise Library** |
|:---:|:---:|
| ![AI Avatar](docs/screenshots/ai-avatar.png) | ![Tutorials](docs/screenshots/tutorials.png) |

| **BMI Calculator** | **Pose Estimation** |
|:---:|:---:|
| ![BMI Calculator](docs/screenshots/bmi-calculator.png) | ![Perform Exercise](docs/screenshots/perform-exercise.png) |

</div>

### 🔗 Public Links
- **Backend API Docs:** [https://fitbot-api-cks6.onrender.com/docs](https://fitbot-api-cks6.onrender.com/docs)
- **Frontend Live Demo:** *[Coming Soon]*

---

## 🛠️ Tech Stack

| Component | Technologies |
| :--- | :--- |
| **Frontend** | React 18, TypeScript, Vite, TailwindCSS, Shadcn/UI, Lucide Icons |
| **Backend** | FastAPI (Python), uvicorn, Groq AI API (LLaMA 3.3 70B) |
| **Database/Auth** | Supabase (PostgreSQL), Edge Functions |
| **AI/Vision** | MediaPipe (Pose), gTTS (Voice), SpeechRecognition |
| **Deployment** | Render (Docker Support), Vercel |

---

## 📦 Installation & Setup

### 1. Prerequisites
- **Node.js** 18.x or higher
- **Python** 3.8 or higher
- **Supabase** Project
- **Groq API Key**

### 2. Frontend Setup
```bash
git clone https://github.com/JawadAliAI/AI-Fitness-Trainer.git
cd AI-Fitness-Trainer
npm install
cp .env.example .env # Add your Supabase credentials
npm run dev
```

### 3. Backend Setup
```bash
# In a new terminal
cd AI-Fitness-Trainer
python -m venv venv
# Windows: venv\Scripts\activate | Mac: source venv/bin/activate
pip install -r requirements.txt
# Set GROQ_API_KEY in your .env
uvicorn AIchat:app --reload --port 8000
```

---

## 📝 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/chat` | Send a message to FitBot AI |
| `POST` | `/tts` | Convert text to speech (WAV) |
| `POST` | `/stt` | Convert audio file to text |
| `GET` | `/tutorials` | Fetch exercise tutorial metadata |

---

## 🤝 Contributors

A huge thanks to the developers who made FitBot possible:

| Contributor | Role | Socials |
| :--- | :--- | :--- |
| **Jawad Ali** | Lead Developer / AI Architect | [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github)](https://github.com/JawadAliAI) |
| **Rana Idrees** | AI Architect / Key Contributor / Full Stack Developer | [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github)](https://github.com/ranaidrees184) |

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.

---

<div align="center">

**Built with ❤️ for a healthier future.**  
[⬆ Back to Top](#%EF%B8%8F-fitbot---ai-fitness-assistant)

</div>
