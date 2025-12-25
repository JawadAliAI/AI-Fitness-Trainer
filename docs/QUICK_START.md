# 🚀 Quick Start Guide

Get FitBot running in 5 minutes!

## Prerequisites

- Node.js 18+ installed
- Python 3.8+ installed
- Git installed

## Step 1: Clone & Install (2 minutes)

```bash
# Clone repository
git clone https://github.com/yourusername/fitbot-ai-fitness.git
cd fitbot-ai-fitness

# Install frontend dependencies
npm install

# Install backend dependencies
pip install -r requirements.txt
```

## Step 2: Setup Environment (1 minute)

### Get API Keys (Free!)

1. **Groq API Key**: https://console.groq.com (Sign up → Create API Key)
2. **Supabase**: https://supabase.com (Create Project → Get URL & Key)

### Create .env Files

**Frontend `.env`:**
```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_key
```

**Backend `.env` (create in root):**
```env
GROQ_API_KEY=your_groq_api_key
```

## Step 3: Setup Database (1 minute)

1. Go to Supabase Dashboard → SQL Editor
2. Copy content from `supabase_setup.sql`
3. Paste and Run
4. ✅ Done!

## Step 4: Run Application (1 minute)

**Terminal 1 - Backend:**
```bash
uvicorn AIchat:app --reload --port 8000
```

**Terminal 2 - Frontend:**
```bash
npm run dev
```

**Open**: http://localhost:8080

## Step 5: Test It Out!

1. Sign up with any email
2. Click "AI Chat"
3. Try: "I want to lose weight and build muscle"
4. 🎉 Enjoy your AI fitness coach!

---

## Troubleshooting

**Backend won't start?**
- Check GROQ_API_KEY in .env
- Make sure Python 3.8+ is installed

**Frontend errors?**
- Run `npm install` again
- Check Supabase credentials

**Database errors?**
- Run the SQL setup script in Supabase
- Check Supabase project is active

---

## Next Steps

- Explore Exercise Tutorials page
- Try voice features (mic button)
- Check out the Dashboard
- Read full documentation in README.md

**Need help?** Open an issue on GitHub!
