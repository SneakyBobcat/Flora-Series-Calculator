# Reservoir

Mobile-first PWA for multi-brand hydroponic nutrient calculation, styled with native iOS design language. Live at **reservoir.farm**.

## Manufacturers & Lines

**17 manufacturers, 38 base systems.** Each line carries its own products, mixing order, EC ranges, and gap-based supplement logic.

### Mineral & Synthetic
General Hydroponics (Classic 3/6/10-Part, FloraPro, BioThrive, MaxiSeries, FloraNova), Advanced Nutrients (pH Perfect Trio, Sensi, Connoisseur, Jungle Juice, Iguana Juice), Botanicare (Pure Blend Pro, CNS17, KIND), Fox Farm (Liquid Trio), CANNA (Coco, Terra), Athena (Pro, Blended), Humboldts Secret (Starter Kit), Emerald Harvest (Cali Pro), House & Garden (Aqua Flakes, Cocos, Soil), Dyna-Gro (Grow & Bloom, Foliage Pro), Technaflora (B.C. Grow & Bloom), Remo Nutrients (Grow/Micro/Bloom), Heavy 16 (Veg & Bud A+B), Mills Nutrients (Basis A+B).

### Dry & Powder
Jack's Nutrients (321).

### Organic
Roots Organics (Buddha Grow & Bloom), Nectar for the Gods (Greek Goddess).

## Crops
26 crops grouped into Fruiting Vegetables, Leafy Greens, Root & Tuber Crops, Herbs, Berries & Fruit, Flowers & Ornamentals, Houseplants & Succulents, and Cannabis.

## Features
- 9-step wizard, manufacturer-aware (auto-skips Brand/System when there's only one option)
- Searchable, category-grouped home page that scales to all brands
- 7 growth stages including Peak Flower, gated to fruiting crops
- Substrate-aware dosing (Hydro / Inert / Potting / Soil) with separate cal-mag scaling
- Feed-strength tiers (Light / Medium / Aggressive) with DLI-based light guidance
- Optional plant-specific dosing, per crop and per stage, controlled by a single master switch
- Gap-based supplement engine: a supplement is flagged Recommended only when the selected base leaves that gap (cal-mag and fulvic are base-aware)
- EC budget with per-plant ceiling alerts, and a per-medium/per-crop pH target
- Always-visible mixing order, plus a link to each brand's official feeding chart
- My Tent: save multiple plants and compare side by side
- Offline-capable PWA, installable to the iPhone home screen

## Deploy to Netlify
1. Create a GitHub repo and upload all files from this folder
2. netlify.com to Add new site to Import from GitHub to select the repo
3. netlify.toml handles build settings, click Deploy
4. Point reservoir.farm at the Netlify site (Domain settings)

## Before going live
- Contact address for security reports and support is reservoirfarmcalc@gmail.com (set in both security.txt files and in the app's Support button).
- If you change the domain, update the canonical/sitemap references in index.html, public/robots.txt, public/sitemap.xml, and both security.txt files.

## Local dev
```bash
npm install
npm run dev
npm run build
```
