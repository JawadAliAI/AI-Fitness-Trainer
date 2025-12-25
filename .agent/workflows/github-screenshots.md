---
description: Run modules and capture screenshots for GitHub
---

# GitHub Screenshots Workflow

This workflow will help you run each module and capture screenshots for your GitHub repository.

## Prerequisites
- Node.js and npm installed
- Python 3.8+ installed
- All dependencies installed

## Steps

### 1. Create Screenshots Directory
```bash
mkdir -p docs/screenshots
```

### 2. Start Backend (AI Assistant)
```bash
cd "d:\FYP\AI Assistent"
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
uvicorn app:app --reload --port 8000
```

### 3. Start Frontend (Main App)
Open a new terminal:
```bash
cd d:\FYP
npm install
npm run dev
```

### 4. Capture Screenshots for Each Module

Access the application at http://localhost:8080 and capture screenshots of:

**Authentication:**
- Login page
- Signup page

**Dashboard:**
- Main dashboard view
- User stats and overview

**AI Chatbot:**
- Chat interface
- Welcome popup
- Voice features (microphone button)
- AI response with tutorials

**Exercise Tutorials:**
- Tutorial library view
- Search functionality
- Category filters
- Individual tutorial card

**BMI Calculator:**
- Calculator interface
- Results display

**Suggested Workouts:**
- Workout plans view
- Workout details

**Perform Exercise:**
- Exercise tracking interface
- Timer/counter view

**Exercise History:**
- History list view
- Exercise logs

**Profile:**
- User profile page
- Settings view

### 5. Organize Screenshots
Save all screenshots to `docs/screenshots/` with descriptive names:
- `auth-login.png`
- `auth-signup.png`
- `dashboard.png`
- `ai-chat.png`
- `ai-chat-voice.png`
- `tutorials.png`
- `tutorials-search.png`
- `bmi-calculator.png`
- `suggested-workouts.png`
- `perform-exercise.png`
- `exercise-history.png`
- `profile.png`

### 6. Update README
Update the README.md file to reference the actual screenshots.

### 7. Create Demo GIF (Optional)
Use a screen recording tool to create a demo GIF showing the main workflow.
