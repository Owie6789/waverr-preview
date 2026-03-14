<p align="center">
  <img src="https://i.ibb.co/MybpdbZT/image.png" 
       alt="Waverr 2.0 Banner" 
       width="51%" 
       style="border-radius: 24px; border: 1px solid rgba(255,255,255,0.1); box-shadow: 0 20px 50px rgba(0,0,0,0.5); image-rendering: -webkit-optimize-contrast;">
</p>

<p align="center">
  <h1 align="center">Waverr | Music Discovery 2.0</h1>
  <p align="center">
    <strong>Offline music made better.</strong> Studio-quality audio meets a "Midnight Glass" aesthetic.
    <br />
    <a href="https://github.com/Owie6789/waverr-preview"><strong>Explore the Docs »</strong></a>
    <br />
    <br />
    <img src="https://img.shields.io/github/stars/Owie6789/waverr-preview.svg?style=for-the-badge&color=8b5cf6" alt="Stars" />
    <img src="https://img.shields.io/github/forks/Owie6789/waverr-preview.svg?style=for-the-badge&color=6366f1" alt="Forks" />
  </p>
</p>

---

### 🖼️ Interface Preview

<p align="center">
  <img src="https://i.ibb.co/XrdxwXQw/image.png" width="45%" style="border-radius: 12px; margin-right: 10px;" alt="Waverr Dashboard Preview">
  <img src="https://i.ibb.co/Mxp8TpGK/image.png" width="45%" style="border-radius: 12px;" alt="Waverr Player Preview">
</p>

---

### ✨ The Waverr Experience

Waverr 2.0 is a high-performance, **offline-first** Progressive Web App (PWA) designed for audiophiles. By bridging the gap between local storage and high-end audio engineering, Waverr transforms your browser into a professional-grade workstation.

> **Why Waverr?**
> 10-band parametric EQ, sub-millisecond search, and 0% cloud tracking. Your music, your privacy.

---

### 🎧 Core Features: The DSP Engine

At the heart of Waverr is a sophisticated **Digital Signal Processing (DSP)** pipeline built on the Web Audio API. 

* **10-Band Parametric Equalizer**: Unlike standard 3-band shelf filters, Waverr utilizes a chain of `BiquadFilterNodes` (Low-shelf, Peaking, and High-shelf) allowing for precise frequency sculpting from 32Hz to 16kHz with a ±12dB gain range.
* **Dynamic Range Compression**: A built-in compressor prevents digital clipping during high-gain EQ adjustments, maintaining a steady RMS level without losing transient punch.
* **Real-time Spectrogram**: High-FPS visualizers rendered via the **Canvas API**, capturing 2048 frequency bins for surgical visual feedback.

---

### 🛠️ Technical Architecture

Waverr utilizes a modern, distributed architecture to handle high-fidelity audio processing and massive local databases without blocking the main UI thread.

| Layer | Stack | Technical implementation |
| :--- | :--- | :--- |
| **Frontend UI** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square) ![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square) | Declarative UI with hardware-accelerated CSS filters and JIT-compiled styling. |
| **Logic Layer** | ![ES2024](https://img.shields.io/badge/JavaScript_ES2024-F7DF1E?style=flat-square&logo=javascript&logoColor=black) | Async state management and non-blocking event loops for metadata extraction. |
| **Audio DSP** | ![Web Audio](https://img.shields.io/badge/Web_Audio_API-9cf?style=flat-square) ![Canvas](https://img.shields.io/badge/Canvas_API-orange?style=flat-square) | Real-time 10-band `BiquadFilterNode` chain and high-FPS spectrogram rendering. |
| **Storage Engine** | ![IndexedDB](https://img.shields.io/badge/IndexedDB-blue?style=flat-square) ![PWA](https://img.shields.io/badge/PWA_Service_Worker-6366f1?style=flat-square) | Transactional binary storage for audio blobs and offline asset caching. |
| **Performance** | ![Web Workers](https://img.shields.io/badge/Web_Workers-green?style=flat-square) | Multi-threaded search indexing using FlexSearch to prevent UI jank. |

---

### ⚡ Performance Benchmarks

Waverr is engineered for scale. By offloading heavy tasks to **Web Workers** and utilizing **IndexedDB** for persistent binary storage, it maintains 60FPS even with massive libraries.

* **Library Capacity**: Tested up to **10,000+ tracks** (approx. 80GB of local data).
* **Search Latency**: `< 5ms` query time via **FlexSearch** contextual indexing.
* **Indexing Speed**: ~1,200 tracks metadata extracted and indexed per minute.
* **Memory Footprint**: Efficient heap management keeping baseline usage under **65MB** during active playback.

---

### 🚀 Getting Started

#### 1️⃣ Installation
**Option A: Git (Developers)**
///bash
git clone https://github.com/Owie6789/waverr-preview.git
///

**Option B: ZIP (Manual Download)**
1. Click the green **"Code"** button at the top of the page.
2. Select **"Download ZIP"** and extract.

#### 2️⃣ Launch
* **🌐 Browser**: Open `index.html` in Chrome, Edge, or Brave.
* **📂 Import**: Drag and drop your music folder to begin the automated indexing process.

---

<p align="center">
  Built with ❤️ by <strong>Owie Emmanuel</strong><br />
  <a href="https://github.com/Owie6789">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=flat&logo=github" alt="GitHub" />
  </a>
</p>

<br>

<div align="center">
  <p style="opacity: 0.8;">
    💡 <strong>Tip:</strong> To populate your Waverr library with high-quality audio without watermarks for free, use these third-party tools:
  </p>
  <p>
    <img src="https://www.google.com/s2/favicons?domain=spotify-downloader.com&sz=16" width="12"> <a href="https://spotify-downloader.com" style="color: inherit; text-decoration: none;">Spotify-Downloader</a> | 
    <img src="https://www.google.com/s2/favicons?domain=cobalt.tools&sz=16" width="12"> <a href="https://cobalt.tools" style="color: inherit; text-decoration: none;">Cobalt (YT/Tidal)</a> | 
    <img src="https://www.google.com/s2/favicons?domain=apple-music-downloader.com&sz=16" width="12"> <a href="https://apple-music-downloader.com" style="color: inherit; text-decoration: none;">Apple Music</a> |
    <img src="https://www.google.com/s2/favicons?domain=soundcloud.com&sz=16" width="12"> <a href="https://scdownloader.io" style="color: inherit; text-decoration: none;">SoundCloud</a> |
    <img src="https://www.google.com/s2/favicons?domain=deezer.com&sz=16" width="12"> <a href="https://deezer-downloader.com" style="color: inherit; text-decoration: none;">Deezer</a> |
    <img src="https://www.google.com/s2/favicons?domain=boomplay.com&sz=16" width="12"> <a href="https://boomplaydownloader.com" style="color: inherit; text-decoration: none;">Boomplay</a> |
    <img src="https://www.google.com/s2/favicons?domain=lucida.to&sz=16" width="12"> <a href="https://lucida.to" style="color: inherit; text-decoration: none;">Lucida (Hi-Res)</a>
  </p>
  <br>
  <p style="max-width: 900px; text-align: justify; text-align-last: center; line-height: 1.4; opacity: 0.5; font-size: 11px; color: #666;">
    <strong>LEGAL DISCLAIMER:</strong> Waverr is an offline audio player designed for educational and private use only. The developer does not host, provide, or condone the download of copyrighted material. Waverr is a standalone interface and is not affiliated with Spotify, YouTube Music, Boomplay, or any other streaming platform. Users are solely responsible for ensuring their use of this software and any external links complies with local jurisdiction laws. This software is provided "as is" without warranty of any kind. The author assumes no liability for damages, account bans, or legal issues arising from the use of this tool.
  </p>
</div>
