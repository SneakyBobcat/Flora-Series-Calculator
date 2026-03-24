# GH Nutrient Calculator

Mobile-first Progressive Web App for General Hydroponics nutrient systems.

## Supported Brands & Systems

| Brand | Systems |
|---|---|
| **Classic** | 3-Part Classic · 6-Part Advanced · 10-Part Professional |
| **FloraPro** | Standard · High EC |
| **BioThrive** | Basic 2-Part · Custom 7-Part |
| **MaxiSeries** | Indoor 2-Part · Outdoor 1-Part |
| **FloraNova** | 1-Part · 4-Part · 8-Part |

## Features

- 9-step wizard: Medium → Brand → System → Plant → Photoperiod → Stage → Settings → Supplements → Results
- Substrate-aware dosing — Hydroponics / Inert / Potting Soil / Ground Soil with automatic dose reduction
- 10 supported crops with individual EC ceilings and dose adjustments (Classic systems)
- Plant modifier toggle on Classic brand — enable/disable crop-specific dose adjustments
- Water source calibration — Tap, Soft, RO/DI
- Light / Medium / Aggressive feed strength tiers
- EC budget with per-plant ceiling alerts
- Optional supplement recommendations by plant type and stage (8 categories, collapsible)
- Always-visible mixing order guide with numbered product rows
- Direct gram totals for dry concentrate systems
- Substrate-specific pH targets

---

## Deploy to Netlify (free, ~5 minutes)

### 1 — Push to GitHub
1. Create a repo at **github.com** (e.g. `gh-nutrient-calculator`)
2. Upload all files from this folder into the repo

### 2 — Deploy on Netlify
1. Sign up at **netlify.com** with your GitHub account
2. **Add new site → Import an existing project → GitHub**
3. Select your repo — build settings auto-read from `netlify.toml`
4. Click **Deploy** — live in ~60 seconds

---

## Install on iPhone

1. Open the live URL in **Safari**
2. Tap **Share → Add to Home Screen**
3. Tap **Add** — runs full-screen offline like a native app

---

## Local development

```bash
npm install
npm run dev       # http://localhost:5173
npm run build     # production build → /dist
npm run preview   # preview production build
```

---

## Project structure

```
gh-nutrient-calculator/
├── index.html
├── vite.config.js
├── package.json
├── netlify.toml
├── public/
│   ├── favicon.svg
│   ├── apple-touch-icon.png
│   └── icons/
│       ├── icon-192.png
│       └── icon-512.png
└── src/
    ├── main.jsx
    └── App.jsx
```
