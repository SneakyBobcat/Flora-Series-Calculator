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

- 8-step wizard: Brand → System → Plant → Photoperiod → Stage → Settings → Supplements → Results
- 10 supported crops with individual EC ceilings and dose adjustments (Classic systems)
- Water source calibration — Tap, Soft, RO/DI
- Light / Medium / Aggressive feed strength tiers
- EC budget with per-plant ceiling alerts
- Optional supplement recommendations by plant type and stage (8 categories, collapsible)
- Mixing order guide for every product combination
- Direct gram totals for dry concentrate systems — no stock-solution math required
- Save & load runs with persistent storage

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

### 3 — Optional custom domain
Netlify → **Domain settings → Add custom domain**

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

## Auto-updates

Push any change to GitHub → Netlify rebuilds automatically → users get the update silently on next open.

---

## Project structure

```
gh-nutrient-calculator/
├── index.html              # App shell with PWA + iOS meta tags
├── vite.config.js          # Vite + PWA plugin
├── package.json
├── netlify.toml            # Netlify build + redirect config
├── public/
│   ├── favicon.svg
│   ├── apple-touch-icon.png
│   └── icons/
│       ├── icon-192.png
│       └── icon-512.png
└── src/
    ├── main.jsx            # React entry point
    └── App.jsx             # Full calculator — all brands, logic, and UI
```
