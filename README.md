# Lovie3D — Romantic 3D Memory Universe ♡

<div align="center">

![Lovie3D Banner](background.jpg)

**An interactive, highly personalized 3D WebGL environment designed as a romantic digital experience for Lovie.**

[![Live Demo](https://img.shields.io/badge/Netlify-Live_Demo-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://a-3d-memory.netlify.app/)
[![Three.js](https://img.shields.io/badge/Three.js-v0.160.0-ff69b4.svg)](https://threejs.org/)
[![WebGL](https://img.shields.io/badge/WebGL-2.0-blueviolet.svg)](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API)
[![Web Audio API](https://img.shields.io/badge/Web_Audio_API-Enabled-brightgreen.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

### 🌐 [Click Here to View Live Experience](https://a-3d-memory.netlify.app/)

</div>

---

## 🌟 Overview

**Lovie3D** is a romantic 3D web application that creates a magical candlelit dinner scene surrounded by a rotating gallery of floating memory frames, a pulsing red heart cloud, and 3D cartoon characters. Built entirely with WebGL and Three.js, it features procedural 3D modeling, interactive photo lightbox inspection, an ambient music synthesizer, and smooth camera controls.

---

## 🚀 Live Demo

Experience the live 3D romantic universe online:
👉 **[https://a-3d-memory.netlify.app/](https://a-3d-memory.netlify.app/)**

---

## ✨ Key Features

### 🖥️ 1. Terminal Typewriter Intro (`lovie3d_init.sh`)
- Styled with a modern macOS-inspired terminal window (red/yellow/green control dots, glass backdrop).
- Types out a personalized, glowing English greeting before fading to reveal the 3D scene:
  > *"Hey Lovie... This is a little special world I created just for you... access_granted: I LOVE YOU FOREVER <3"*

### 👫 2. 3D Boy & Girl Characters
- Custom 3D cartoon models of the boy and girl sitting together in wooden dining chairs with plush pink cushions.
- Positioned leaning forward with heads tilted down and holding wooden chopsticks over their sushi bowls like they are enjoying dinner.

### 🍣 3. Dual-Mode 3D Dining Objects & Fallbacks
- Uses a **dual-loading architecture** (`loadModelWithFallback`): attempts loading external `.gltf` 3D models with an automatic 3.5s timeout procedural fallback.
- **Table Setup**:
  - Ceramic Sushi Bowls with salmon blocks, avocado, and chopsticks.
  - Dark Slate Sushi Platter with nigiri and maki rolls.
  - Refractive Glass Wine Bottle featuring a custom *"Château Lovie — Cuvée d'Amour 2026"* label.
  - Refractive Wine Glasses filled with red wine liquid.
  - Crystal Flower Vase with a bouquet of 7 multi-layered blooming roses.
  - Animated Flickering Candles emitting warm dynamic point light shadows.

### 🖼️ 4. Memory Ring & Interactive Photo Lightbox
- Rotating gallery of 12 sleek **Black Picture Bar Frames** floating around the dining area.
- Displays AI-generated cartoon romantic couple illustrations (`1.jpeg` through `12.jpeg`, `tavolo2.jpeg`).
- **Interactive Lightbox Modal**: Click or tap any photo frame in the 3D scene to open a full-screen blurred glass modal with the enlarged photo, romantic title, and memory description.

### ❤️ 5. Red Heart Cloud & Magical Sparkle Dust
- **Background Heart Cloud**: 280 glowing **red text sprites** ("i love you") orbiting along a 3D parametric heart equation.
- **Sparkle Dust**: 140 floating magical pink and gold dust particles using `AdditiveBlending`.
- **Mandala Floor & Checkered Tablecloth**: Procedural canvas-generated textures for an Indian-style mandala tile floor and red-white checkered tablecloth.

### 🎵 6. Web Audio API Ambient Synthesizer
- Interactive top-right **"🎵 Music On/Off"** toggle button.
- Generates romantic C Major 7 chord arpeggios in real-time using sine oscillators and gain envelopes without external audio file dependencies.

---

## 🛠️ Tech Stack

- **Frontend Core**: HTML5, Vanilla CSS3 (Glassmorphic Design)
- **3D Graphics & WebGL Engine**: [Three.js (v0.160.0)](https://threejs.org/) via ES6 modules
- **Controls & Lighting**: `OrbitControls`, ACES Filmic Tone Mapping, Soft Shadow Maps (`PCFSoftShadowMap`)
- **Audio Engine**: Web Audio API (real-time chord synthesis)
- **Design & Typography**: Google Fonts (`Outfit`, `Playfair Display`, `Fira Code`)
- **Hosting & Deployment**: Netlify

---

## 📁 Directory & Asset Structure

```
Nancy3D-main/
├── index.html              # Main application entry point (HTML, CSS, Three.js logic)
├── background.jpg          # Fantasy romantic night sky background
├── 1.jpeg - 12.jpeg        # Cartoon couple memory gallery photos
├── tavolo2.jpeg            # Special surprise memory photo
├── README.md               # Project documentation
├── LICENSE                 # Project license
├── bowl/                   # 3D sushi bowl GLTF model directory
├── sushi/                  # 3D sushi platter GLTF model directory
├── glass/                  # 3D glass cup GLTF model directory
├── wine bottle/            # 3D wine bottle GLTF model directory
└── flowers/                # 3D flower vase GLTF model directory
```

---

## 🚀 Quick Start / Local Setup

Because Three.js loads local textures and 3D models via ES modules, it is recommended to run the project using a local HTTP server:

### Option 1: Python (Built-in)
```bash
python -m http.server 5500
```
Then open `http://localhost:5500` in your web browser.

### Option 2: Node.js / `http-server`
```bash
npx http-server -p 8080
```
Then open `http://localhost:8080` in your web browser.

### Option 3: Direct File Opening
You can also open `index.html` directly in modern browsers. The project includes automatic canvas texture fallbacks if local `file://` CORS restrictions apply.

---

## 🎮 Controls & Interactions

| Action | Control |
|---|---|
| **Rotate Camera** | Left-click & drag (or 1-finger touch drag) |
| **Zoom In / Out** | Mouse wheel scroll (or pinch-to-zoom) |
| **Inspect Photo Memory** | Left-click / tap any black photo frame |
| **Close Photo Lightbox** | Click **✕** button, click backdrop, or press **Esc** |
| **Toggle Music** | Click top-right **🎵 Music** button |
| **Reset View** | Click top-right **📷 Reset View** button |

---

## 🙌 Credits & Acknowledgments

Created with love by **[hxni](https://github.com/hxni)** for **Lovie**.

Special thanks to open-source contributors and 3D model creators for Three.js assets and shaders.

---

<div align="center">

Made with ❤️ by **hxni** for **Lovie**

</div>
