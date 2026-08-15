# Dawat-e-Tabligh 📿

A trilingual (Urdu / Roman Urdu / English) Progressive Web App presenting the history, core teachings, and etiquette of Dawat-e-Tabligh — installable on any phone with no app-store download required.

**🔗 Live demo:** https://p8500775-web.github.io/dawat-e-tabligh/

![Home screen](screenshots/1-home-roman.png)

## Features

- 🌐 **3-language switcher** — Urdu (RTL, Nastaliq script), Roman Urdu, and English, with full content translated across every screen
- 📱 **Installable PWA** — add-to-home-screen support via `manifest.json` and a service worker for offline access
- 🎨 **Custom design system** — geometric star motifs, no figurative imagery, RTL-aware layout, Google Fonts (Reem Kufi, Amiri, Noto Nastaliq Urdu)
- 🧭 **6 content sections** — Home, History timeline, Six Points (with accordion detail), Etiquette checklist, Rules & Regulations, and an FAQ accordion
- ⚡ **Zero dependencies** — a single-file frontend (vanilla HTML/CSS/JS), no build step, no framework

## Screenshots

| Home | Six Points | FAQ (English) | Urdu (RTL) |
|---|---|---|---|
| ![Home](screenshots/1-home-roman.png) | ![Six Points](screenshots/2-six-points.png) | ![FAQ](screenshots/3-faq-english.png) | ![Urdu](screenshots/4-home-urdu.png) |

## Tech Stack

- HTML5 / CSS3 (custom properties, no framework)
- Vanilla JavaScript (i18n dictionary pattern, tab + accordion state management)
- PWA: Web App Manifest + Service Worker (cache-first offline strategy)
- Fonts: Google Fonts (Reem Kufi, Amiri, Noto Nastaliq Urdu, Outfit)

## Run Locally

```bash
git clone https://github.com/your-username/dawat-e-tabligh.git
cd dawat-e-tabligh
# open index.html directly in a browser, or serve it:
python3 -m http.server 8000
```

## Install as an App

1. Open the [live demo link](https://p8500775-web.github.io/dawat-e-tabligh/) on your phone
2. Tap your browser's menu → **Add to Home Screen**
3. Launch it like any other app — full screen, no browser bar

## Project Structure

```
dawat-e-tabligh/
├── index.html       # entire app: markup, styles, i18n content, logic
├── manifest.json     # PWA metadata (name, icons, theme colour)
├── sw.js              # service worker for offline caching
├── icon-192.png
├── icon-512.png
└── screenshots/
```

## What This Project Demonstrates

- Building a multi-language app with a maintainable i18n pattern (no framework)
- RTL layout handling alongside LTR layouts in the same codebase
- Converting a static site into an installable PWA
- Component-style UI patterns (accordions, tab navigation) in vanilla JS
- Attention to content accuracy and source-based accuracy when presenting factual/historical material

## License

MIT — free to use and adapt.
