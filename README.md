# TTB COLA AI Validator

AI-powered Certificate of Label Approval compliance platform for the U.S. Alcohol and Tobacco Tax and Trade Bureau (TTB).

## What This Is
A live demo app that validates alcohol beverage labels against TTB regulatory requirements (27 CFR Parts 4, 5, 7) before submission — reducing rejections and cutting review time.

## Features
- 5-screen guided demo flow for TTB stakeholder presentations
- AI-powered label compliance analysis (Claude API)
- Sample label generator with toggleable compliance violations
- CFR citation mapping for every check
- Plain-English fix recommendations

## Deploy to Vercel

### Option 1 — Drag & Drop (Fastest)
1. Go to https://vercel.com/new
2. Drag this folder into the browser
3. Done — live URL in 30 seconds

### Option 2 — CLI
```bash
npm install -g vercel
vercel
```

### Option 3 — GitHub
1. Push this folder to GitHub
2. Connect repo at https://vercel.com/new
3. Auto-deploys on every push

## Files
- `index.html` — Main demo app (all-in-one)
- `vercel.json` — Vercel deployment config
- `README.md` — This file

## Tech Stack
- Vanilla HTML/CSS/JS (no framework needed)
- Claude API (claude-sonnet-4-20250514) for AI analysis
- Hosted on Vercel
