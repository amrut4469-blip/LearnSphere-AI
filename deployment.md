# ☁ Deployment Guide

## Deploy on Vercel
1. Push the repository to GitHub.
2. Go to https://vercel.com/new and import the repository.
3. Under **Environment Variables**, add `GEMINI_API_KEY`.
4. Click **Deploy**.

Live app: https://learnsphere-ai-seven.vercel.app

## Run locally
```bash
npm install
cp .env.example .env.local
npm run dev
```

## Production build
```bash
npm run build
npm start
```

## Checklist
- [ ] `GEMINI_API_KEY` set in Vercel
- [ ] `.env.local` not committed
- [ ] Build passes
