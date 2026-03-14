# 🏃 Zürich Marató Barcelona 2026

> Pace calculator with official GPX map — installable PWA for Android & iOS

**Live app → [plopesc.github.io/marathon-bcn-tracker](https://plopesc.github.io/marathon-bcn-tracker/)**

[![PWA](https://img.shields.io/badge/PWA-ready-6366f1?style=flat-square)](https://plopesc.github.io/marathon-bcn-tracker/)
[![GPX](https://img.shields.io/badge/GPX-official-34d399?style=flat-square)](https://www.zurichmaratobarcelona.es)
[![License](https://img.shields.io/badge/license-MIT-fbbf24?style=flat-square)](LICENSE)

---

## What is this?

A Progressive Web App (PWA) to plan your race strategy for the **Zürich Marató Barcelona 2026** (March 15, 2026). It combines a real-time pace calculator with the official GPX course overlaid on an interactive map — all in a single HTML file, no backend needed.

---

## Features

- 🎚️ **Pace sliders** — configure your target pace for each segment (km 0–20, 21–30, 31–42) and see results update instantly
- 🗺️ **Live map** — official GPX route with split markers repositioned dynamically as you adjust paces
- ⏱️ **Split times** — every 5 km plus the half marathon mark, recalculated in real time
- 🍬 **Gel plan** — configurable interval (15–60 min), with markers placed on the exact km of the route
- 🌍 **Spanish / English** — language switcher in the top bar
- 📴 **Works offline** — Service Worker caches all assets on first load
- 📱 **Installable** — add to home screen on Android (Chrome) and iOS (Safari)

---

## Screenshots

| Calculator | Map |
|---|---|
| Pace sliders, split table and gel plan on the left panel | Official GPX route with dynamic markers on the right |

---

## 📱 Install as an app

### Android (Chrome)
1. Open [plopesc.github.io/marathon-bcn-tracker](https://plopesc.github.io/marathon-bcn-tracker/) in Chrome
2. Tap the **Install** banner at the bottom, or go to menu ⋮ → *Add to home screen*
3. The app installs with its own icon and runs without a browser bar

### iOS (Safari)
1. Open [plopesc.github.io/marathon-bcn-tracker](https://plopesc.github.io/marathon-bcn-tracker/) in Safari
2. Tap the share button **⎙**
3. Select **Add to Home Screen** → **Add**

---

## 📁 Repository structure

```
/
├── index.html        # Full application — single self-contained file
├── manifest.json     # PWA manifest (name, icons, theme colour)
├── sw.js             # Service Worker (offline cache)
├── icon-192.svg      # App icon 192 × 192
├── icon-512.svg      # App icon 512 × 512
└── README.md         # This file
```

---

## 🗺️ Course data

The GPX file is the **official Zürich Marató Barcelona 2026** track, published by RPM Sports on Strava. Split times and gel waypoints are computed dynamically against the real accumulated distance using the [Haversine formula](https://en.wikipedia.org/wiki/Haversine_formula).

---

## 🚀 Deploy your own copy to GitHub Pages

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set Source → Branch: `main`, Folder: `/ (root)` → **Save**
4. Your app will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/`

> GitHub Pages provides HTTPS automatically, which is required for the Service Worker to activate.

---

## 🤖 Built with Claude

This app was built with the help of [Claude](https://claude.ai) by Anthropic — from the pace calculator logic and GPX parsing, to the interactive map, PWA setup, multilingual support and these very icons.

---

## 📄 License

[MIT](LICENSE) — free to use, modify and distribute.
