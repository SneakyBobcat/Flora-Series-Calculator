# GH Nutrient Calculator — PWA

Mobile-optimized hydroponic feeding calculator for General Hydroponics product lines:
- **Flora Series** — Classic 3-Part, 6-Part Advanced, 10-Part Professional
- **FloraPro** — Standard & High EC powder programs
- **BioThrive** — Basic 2-Part & Custom 7-Part organic systems
- **MaxiSeries** — Indoor 2-Part & Outdoor 1-Part dry concentrate
- **FloraNova** — 1-Part, 4-Part & 8-Part liquid concentrate

---

## Deploy to Netlify (free, ~5 minutes)

### Step 1 — Push to GitHub
1. Create a free account at **github.com**
2. Click **+** → **New repository** → name it `gh-nutrient-calculator`
3. Upload all files from this folder into the repo (drag and drop works)

### Step 2 — Deploy on Netlify
1. Create a free account at **netlify.com** (sign in with GitHub)
2. Click **Add new site** → **Import an existing project** → **GitHub**
3. Select your `gh-nutrient-calculator` repo
4. Build settings are auto-read from `netlify.toml` — just click **Deploy site**
5. You'll get a free URL like `https://gh-nutrient-calc-abc123.netlify.app`

### Step 3 — Optional custom domain (~$12/year)
In Netlify → **Domain settings** → **Add custom domain**

---

## Install on iPhone as an app

1. Open the URL in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (box with arrow pointing up)
3. Tap **Add to Home Screen**
4. Tap **Add** — the GH green icon appears on your home screen
5. Open it — runs full-screen like a native app, works offline

---

## Local development

```bash
npm install
npm run dev        # starts at http://localhost:5173
npm run build      # production build to /dist
npm run preview    # preview the production build locally
```

---

## Project structure

```
gh-nutrient-calculator/
├── index.html              # App shell with PWA + iOS meta tags
├── vite.config.js          # Vite + PWA plugin config
├── package.json            # Dependencies
├── netlify.toml            # Netlify build config
├── public/
│   ├── favicon.svg
│   ├── apple-touch-icon.png
│   └── icons/
│       ├── icon-192.png
│       └── icon-512.png
└── src/
    ├── main.jsx            # React entry point
    └── App.jsx             # Full calculator app
```

---

## Updating the app

Any time you push changes to GitHub, Netlify automatically rebuilds and redeploys. Users with the app installed will get the update automatically on next open (PWA auto-update is enabled).
