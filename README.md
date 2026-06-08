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

## Environment Variables

The API key must stay server-side. The browser calls `/api/analyze`, which proxies to Anthropic using `ANTHROPIC_API_KEY`.

### Vercel (production)
1. Open your project in the [Vercel dashboard](https://vercel.com/dashboard)
2. Go to **Settings → Environment Variables**
3. Add:

| Name | Value |
|---|---|
| `ANTHROPIC_API_KEY` | Your key from [console.anthropic.com](https://console.anthropic.com/) |

4. Enable it for **Production** (and Preview if you want)
5. **Redeploy** after saving — env vars only apply on the next deploy

### Local development
```bash
cp .env.example .env.local
# Edit .env.local with your key, then:
npx vercel dev
```

Do not put the API key in `index.html` or commit it to git.

## Tech Stack
- Vanilla HTML/CSS/JS (no framework needed)
- Claude API (claude-sonnet-4-20250514) via Vercel serverless proxy
- Hosted on Vercel
