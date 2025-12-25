# 🏋️‍♂️ FitBot - AI-Powered Fitness Coach

<div align="center">

![FitBot Banner](https://via.placeholder.com/1200x300/1a1a2e/16c79a?text=FitBot+-+Your+Personal+AI+Fitness+Coach)

### Transform Your Fitness Journey with AI-Powered Guidance

[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=flat-square&logo=react&logoColor=white)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Supabase](https://img.shields.io/badge/Supabase-Powered-3ECF8E?style=flat-square&logo=supabase&logoColor=white)](https://supabase.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

[✨ Features](#-core-features) • [🚀 Quick Start](#-quick-start) • [📖 Documentation](#-documentation) • [🤝 Contributing](#-contributing) • [📬 Support](#-support)

</div>

---

## 🌟 Overview

**FitBot** is a next-generation fitness assistant that combines artificial intelligence, voice interaction, and personalized coaching to help you achieve your fitness goals. Whether you're a beginner taking your first steps or an athlete optimizing performance, FitBot adapts to your needs.

### Why FitBot?

| Feature | Description |
|---------|-------------|
| 🧠 **Smart AI Coach** | Powered by Groq's LLaMA 3.3 70B for intelligent, context-aware conversations |
| 🎤 **Voice First** | Hands-free interaction with speech-to-text and text-to-speech capabilities |
| 📹 **Visual Learning** | 50+ curated exercise tutorials from YouTube with proper form demonstrations |
| 📊 **Data-Driven** | Track progress, analyze performance, and visualize your fitness journey |
| 🎯 **Personalized** | Custom workout plans based on your goals, equipment, and schedule |
| 🌙 **Modern UX** | Beautiful dark-mode interface that's responsive across all devices |

---

## ✨ Core Features

### 💬 Intelligent Conversational AI
- **Natural Language Understanding** - Chat naturally about your fitness goals
- **Contextual Memory** - FitBot remembers your preferences and progress throughout conversations
- **Smart Recommendations** - Get personalized workout plans, nutrition advice, and form corrections
- **Goal-Oriented Coaching** - Whether building muscle, losing weight, or improving endurance, FitBot guides you

### 🎙️ Advanced Voice Integration
- **Speech-to-Text Input** - Speak your questions during workouts (5-second recording)
- **Text-to-Speech Output** - Listen to AI responses with natural voice synthesis
- **Auto-Play Mode** - Hands-free experience with automatic voice playback
- **Multi-Language Support** - Communicate in your preferred language

### 🎬 Comprehensive Exercise Library
- **50+ Professional Tutorials** - Covering all major muscle groups and movements
- **Smart Search** - Find exercises instantly by name or muscle group
- **Category Filters** - Chest, Back, Legs, Shoulders, Arms, Core, Cardio, Full Body
- **Difficulty Levels** - Beginner-friendly to advanced techniques
- **Direct Integration** - Watch tutorials without leaving the app

### 🎨 Premium User Experience
- **Interactive Onboarding** - Welcome popup with guided examples
- **Quick-Action Templates** - One-click message suggestions for common queries
- **Real-Time Chat** - Smooth animations and instant AI responses
- **In-Context Recommendations** - Exercise tutorials embedded directly in chat responses
- **Persistent History** - All conversations saved for future reference
- **Responsive Design** - Seamless experience on desktop, tablet, and mobile

### 📈 Progress Tracking & Analytics
- **Exercise History** - Log and review all your workouts
- **Performance Metrics** - Track sets, reps, and personal records
- **BMI Calculator** - Monitor your body composition
- **Visual Dashboards** - Graphs and charts showing your progress over time
- **AI Pose Estimation** - Real-time form checking during exercises

### 👤 Complete Profile Management
- **User Authentication** - Secure login and signup with Supabase
- **Personalized Profiles** - Store your fitness goals, preferences, and stats
- **Customizable Settings** - Adjust AI behavior, voice settings, and notifications
- **Data Privacy** - Your information is encrypted and secure

---

## 🎯 Use Cases

<table>
<tr>
<td width="50%">

### 💪 Muscle Building
- Progressive overload programs
- Hypertrophy-focused routines
- Compound movement guidance
- Recovery optimization

</td>
<td width="50%">

### 🔥 Weight Loss
- Caloric deficit strategies
- HIIT and cardio plans
- Nutrition guidance
- Sustainable habit formation

</td>
</tr>
<tr>
<td width="50%">

### 🏃 Endurance Training
- Cardio conditioning
- Stamina building programs
- Heart rate zone training
- Race preparation

</td>
<td width="50%">

### 🧘 Wellness & Mobility
- Flexibility routines
- Injury prevention
- Stress relief exercises
- Mindful movement

</td>
</tr>
</table>

---

## 🚀 Quick Start

### ⚡ Prerequisites

Before you begin, ensure you have:
- **Node.js** 18.0 or higher ([Download](https://nodejs.org/))
- **Python** 3.8 or higher ([Download](https://www.python.org/))
- **Git** ([Download](https://git-scm.com/))
- **Supabase Account** ([Sign up free](https://supabase.com/))
- **Groq API Key** ([Get free key](https://console.groq.com/))

### 📥 Installation

#### Step 1: Clone the Repository
```bash
git clone https://github.com/JawadAliAI/AI-Fitness-Trainer.git
cd AI-Fitness-Trainer
```

#### Step 2: Frontend Setup
```bash
# Install dependencies
npm install

# Configure environment
cp .env.example .env
```

Edit `.env` and add your Supabase credentials:
```env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_PUBLISHABLE_KEY=your-anon-key
```

#### Step 3: Backend Setup
```bash
# Create and activate virtual environment
python -m venv venv

# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate

# Install Python dependencies
pip install -r requirements.txt
```

Create backend `.env` file:
```env
GROQ_API_KEY=your-groq-api-key-here
```

#### Step 4: Database Setup
1. Navigate to [Supabase Dashboard](https://app.supabase.com/)
2. Create a new project (or use existing)
3. Go to **SQL Editor** in the left sidebar
4. Copy and run the schema from `supabase_setup.sql`

#### Step 5: Launch Application

**Terminal 1 - Start Backend:**
```bash
uvicorn AIchat:app --reload --port 8000
```

**Terminal 2 - Start Frontend:**
```bash
npm run dev
```

**🎉 Open your browser:** http://localhost:8080

---

## 🛠️ Technology Stack

### Frontend Architecture
```
React 18 + TypeScript
├── Vite (Build Tool)
├── TailwindCSS (Styling)
├── Shadcn/ui (Components)
├── Supabase Client (Auth & DB)
└── React Router (Navigation)
```

### Backend Architecture
```
FastAPI (Python)
├── Groq AI (LLaMA 3.3 70B)
├── gTTS (Text-to-Speech)
├── SpeechRecognition (Speech-to-Text)
├── Pydantic (Validation)
└── CORS Middleware
```

### Database & Infrastructure
```
Supabase (PostgreSQL)
├── User Authentication
├── Profile Management
├── Exercise History
└── Real-time Updates
```

---

## 📖 Documentation

### 🔌 API Reference

**Base URLs:**
- Production: `https://fitbot-api-cks6.onrender.com`
- Development: `http://localhost:8000`
- Docs: `https://fitbot-api-cks6.onrender.com/docs`

#### Chat Endpoint
```http
POST /chat
Content-Type: application/json

Request Body:
{
  "message": "Create a 4-day workout plan",
  "user_id": "user_123",
  "chat_history": []
}

Response:
{
  "reply": "I'd be happy to create a 4-day plan! Do you have access to a gym or will you be working out at home?",
  "tutorials": [
    {
      "exercise": "Bench Press",
      "links": ["https://youtube.com/watch?v=..."]
    }
  ],
  "chat_history": [...],
  "message_count": 2
}
```

#### Text-to-Speech Endpoint
```http
POST /tts
Content-Type: application/json

Request Body:
{
  "text": "Great job completing your workout!",
  "language_code": "en"
}

Response: audio/wav (binary)
```

#### Speech-to-Text Endpoint
```http
POST /stt
Content-Type: multipart/form-data

Form Data:
- file: audio.wav (audio file)

Response:
{
  "transcript": "I want to build muscle"
}
```

#### Get Tutorials
```http
GET /tutorials

Response:
{
  "total_exercises": 50,
  "exercises": [
    {
      "id": 1,
      "name": "Squats",
      "category": "Legs",
      "difficulty": "Beginner",
      "video_url": "https://youtube.com/..."
    }
  ]
}
```

### 📱 Usage Examples

#### Example 1: Weight Loss Journey
```
User: "I need to lose 20 pounds in 3 months"

FitBot: "That's a great goal! Let's create a sustainable plan. 
First, where will you be working out - gym or home?"

User: "Gym"

FitBot: "Perfect! How many days per week can you commit to training?"

User: "5 days"

FitBot: [Creates detailed 5-day workout plan with:
- 3 days strength training
- 2 days cardio
- Specific exercises with sets/reps
- YouTube tutorial links
- Nutrition guidelines]
```

#### Example 2: Home Workout
```
User: "I only have dumbbells at home"

FitBot: "No problem! I can design an effective program with just dumbbells. 
What are your main goals?"

User: "Build upper body strength"

FitBot: [Provides dumbbell-only upper body routine with:
- Push day exercises
- Pull day exercises
- Shoulder workouts
- Progressive overload tips
- Video demonstrations]
```

---

## 📂 Project Structure

```
fitbot-ai-fitness/
│
├── 📁 src/                          # Frontend source code
│   ├── 📁 components/              # Reusable React components
│   │   ├── Navbar.tsx
│   │   ├── Footer.tsx
│   │   └── ui/                    # Shadcn UI components
│   │
│   ├── 📁 pages/                   # Application pages
│   │   ├── AIChatbot.tsx          # AI chat interface
│   │   ├── ExerciseTutorials.tsx  # Tutorial library
│   │   ├── Dashboard.tsx          # User dashboard
│   │   ├── Profile.tsx            # Profile management
│   │   ├── BMICalculator.tsx      # BMI tool
│   │   └── Auth.tsx               # Login/Signup
│   │
│   ├── 📁 integrations/           # Third-party services
│   │   └── supabase/
│   │       ├── client.ts
│   │       └── types.ts
│   │
│   ├── 📁 hooks/                   # Custom React hooks
│   ├── 📁 utils/                   # Helper functions
│   ├── App.tsx                     # Main app component
│   └── main.tsx                    # Entry point
│
├── 📁 backend/
│   ├── AIchat.py                   # FastAPI application
│   ├── requirements.txt            # Python dependencies
│   └── .env                        # Environment variables
│
├── 📁 docs/                         # Documentation
│   ├── SETUP.md                    # Setup guide
│   ├── API.md                      # API documentation
│   ├── CONTRIBUTING.md             # Contribution guide
│   └── 📁 screenshots/
│
├── 📁 database/
│   └── supabase_setup.sql         # Database schema
│
├── package.json                    # Node dependencies
├── tsconfig.json                   # TypeScript config
├── tailwind.config.js             # Tailwind config
├── vite.config.ts                 # Vite config
├── .env.example                   # Environment template
├── .gitignore
├── LICENSE
└── README.md                      # This file
```

---

## 🚢 Deployment

### Frontend Deployment (Vercel)

1. **Build the project:**
```bash
npm run build
```

2. **Deploy to Vercel:**
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel deploy --prod
```

3. **Set environment variables in Vercel dashboard:**
- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_PUBLISHABLE_KEY`

### Backend Deployment (Render)

1. Create a new **Web Service** on [Render](https://render.com)
2. Connect your GitHub repository
3. Configure:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `uvicorn AIchat:app --host 0.0.0.0 --port $PORT`
4. Add environment variable:
   - `GROQ_API_KEY=your_key_here`
5. Deploy

### Alternative: Docker Deployment

```dockerfile
# Dockerfile example
FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
EXPOSE 8000
CMD ["uvicorn", "AIchat:app", "--host", "0.0.0.0", "--port", "8000"]
```

```bash
docker build -t fitbot-backend .
docker run -p 8000:8000 -e GROQ_API_KEY=your_key fitbot-backend
```

---

## 🤝 Contributing

We love contributions! Here's how you can help make FitBot even better:

### Development Process

1. **Fork** the repository
2. **Create** a feature branch
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make** your changes
4. **Test** thoroughly
5. **Commit** with clear messages
   ```bash
   git commit -m "Add: Amazing new feature that does X"
   ```
6. **Push** to your fork
   ```bash
   git push origin feature/amazing-feature
   ```
7. **Open** a Pull Request

### Contribution Guidelines

- ✅ Follow existing code style and conventions
- ✅ Write clear, descriptive commit messages
- ✅ Add tests for new features
- ✅ Update documentation as needed
- ✅ Ensure all tests pass before submitting PR
- ✅ Keep PRs focused on a single feature/fix

### Areas We Need Help With

- 🐛 Bug fixes and testing
- 🌍 Internationalization and translations
- 📱 Mobile app development
- 🎨 UI/UX improvements
- 📚 Documentation improvements
- 🧪 Unit and integration tests
- ♿ Accessibility enhancements

---

## 🐛 Bug Reports & Feature Requests

### Reporting Bugs
Found a bug? [Open an issue](https://github.com/JawadAliAI/AI-Fitness-Trainer/issues) with:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Your environment (OS, browser, versions)

### Requesting Features
Have an idea? [Open a feature request](https://github.com/JawadAliAI/AI-Fitness-Trainer/issues) with:
- Clear description of the feature
- Use cases and benefits
- Potential implementation approach

---

## 🔮 Roadmap

### Q1 2025
- [ ] 🍎 Meal planning and nutrition tracking module
- [ ] 📊 Advanced analytics dashboard with charts
- [ ] 🔗 Wearable device integration (Fitbit, Apple Watch)
- [ ] 🌍 Multi-language support (Spanish, French, German)

### Q2 2025
- [ ] 📱 Native mobile apps (iOS & Android)
- [ ] 🎥 In-app video player for tutorials
- [ ] 👥 Social features (friends, challenges, leaderboards)
- [ ] 🤖 AI pose estimation improvements

### Q3 2025
- [ ] 💰 Premium features and subscription model
- [ ] 🏋️ Virtual personal training sessions
- [ ] 📖 Exercise form AI analysis with feedback
- [ ] ☁️ Offline mode with sync

### Future Considerations
- [ ] Integration with gym equipment
- [ ] Community workout challenges
- [ ] Certified trainer marketplace
- [ ] AR-powered exercise guidance

---

## 📊 Project Stats

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/JawadAliAI/AI-Fitness-Trainer?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/JawadAliAI/AI-Fitness-Trainer?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/JawadAliAI/AI-Fitness-Trainer?style=for-the-badge)
![GitHub pull requests](https://img.shields.io/github/issues-pr/JawadAliAI/AI-Fitness-Trainer?style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/JawadAliAI/AI-Fitness-Trainer?style=for-the-badge)

</div>

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for full details.

```
MIT License

Copyright (c) 2024 Jawad Ali

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
...
```

---

## 👨‍💻 Author

<div align="center">

**Jawad Ali**

[![GitHub](https://img.shields.io/badge/GitHub-JawadAliAI-181717?style=for-the-badge&logo=github)](https://github.com/JawadAliAI)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jawadaliyousafzai.ai@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/jawadali)

</div>

---

## 🙏 Acknowledgments

Special thanks to the amazing technologies and teams that made FitBot possible:

- **[Groq](https://groq.com/)** - Lightning-fast LLaMA 3.3 70B inference
- **[Supabase](https://supabase.com/)** - Open-source Firebase alternative for auth and database
- **[FastAPI](https://fastapi.tiangolo.com/)** - Modern Python web framework
- **[Shadcn/ui](https://ui.shadcn.com/)** - Beautiful, accessible component library
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[React](https://react.dev/)** - UI library by Meta
- **YouTube** - Exercise tutorial content creators
- **Open Source Community** - For continuous inspiration and support

---

## 📬 Support

Need help? We're here for you!

- 📧 **Email:** jawadaliyousafzai.ai@gmail.com
- 💬 **Discord:** [Join our community](https://discord.gg/fitbot) _(coming soon)_
- 🐛 **Issues:** [GitHub Issues](https://github.com/JawadAliAI/AI-Fitness-Trainer/issues)
- 📚 **Docs:** [Full Documentation](https://github.com/JawadAliAI/AI-Fitness-Trainer/wiki)

---

## 🌟 Star History

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=JawadAliAI/AI-Fitness-Trainer&type=Date)](https://star-history.com/#JawadAliAI/AI-Fitness-Trainer&Date)

</div>

---

<div align="center">

### Made with ❤️ and 💪 by the FitBot Team

**Transform your fitness journey today!**

[⭐ Star this repo](https://github.com/JawadAliAI/AI-Fitness-Trainer) • [🐛 Report Bug](https://github.com/JawadAliAI/AI-Fitness-Trainer/issues) • [💡 Request Feature](https://github.com/JawadAliAI/AI-Fitness-Trainer/issues)

---

**FitBot** - *Because everyone deserves an intelligent fitness coach*

[⬆ Back to Top](#️-fitbot---ai-powered-fitness-coach)

</div>
