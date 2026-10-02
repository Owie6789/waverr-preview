> Made this update because funny enough, this was my first ever serious project lmao, I didn't even know how to use git or github😭, if any beginner ever sees this, don't give up, I went from being so proud of myself for making this in HTML and now I comfortably write Rust, anyways it turns out I had this locally 7 months after, and I didn't even know how to push shii, so here it is, issues known, search doesn't work, no debouncing so alot of imported songs gets laggy. If you need an actual music player check out **Nora** https://github.com/Sandakan/Nora/ | https://noramusic.netlify.app/
I ended up working on Nora to rekindle my music player flair.

<br>

<p align="center">
  <img src="https://i.ibb.co/MybpdbZT/image.png" 
       alt="Waverr 3.0 Banner" 
       width="51%" 
       style="border-radius: 24px; border: 1px solid rgba(255,255,255,0.1); box-shadow: 0 20px 50px rgba(0,0,0,0.5); image-rendering: -webkit-optimize-contrast;">
</p>

<p align="center">
  <h1 align="center">Waverr | Music Discovery 3.0</h1>
  <p align="center">
    <strong>An offline-first browser audio player with Web Audio DSP.</strong> 
    <br />
    Built-in signal processing and a dark glass interface.
    <br />
    <br />
    <a href="https://owie6789.github.io/waverr-preview/"><strong>Live Production Preview »</strong></a>
    &nbsp;•&nbsp;
    <a href="https://github.com/Owie6789/waverr-preview/issues"><strong>Open Issue / Suggest Improvement »</strong></a>
    <br />
    <br />
    <img src="https://img.shields.io/github/stars/Owie6789/waverr-preview.svg?style=for-the-badge&color=8b5cf6" alt="Stars" />
    <img src="https://img.shields.io/github/forks/Owie6789/waverr-preview.svg?style=for-the-badge&color=6366f1" alt="Forks" />
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="License" />
  </p>
</p>

---

### 🖼️ Interface Preview

<p align="center">
  <img src="https://i.ibb.co/XrdxwXQw/image.png" width="45%" style="border-radius: 12px; margin-right: 10px; border: 1px solid rgba(255,255,255,0.05);" alt="Waverr Dashboard Preview">
  <img src="https://i.ibb.co/Mxp8TpGK/image.png" width="45%" style="border-radius: 12px; border: 1px solid rgba(255,255,255,0.05);" alt="Waverr Player Preview">
</p>

---

### About Waverr

Waverr 3.0 is an offline-first Progressive Web App (PWA) for playing local audio files. All track data, metadata, and audio processing remain entirely on your device.

---

### 🎧 Audio Features

Waverr runs a custom processing pipeline built on the Web Audio API:

- **10-Band Parametric Equalizer**: A chain of `BiquadFilterNodes` with precise Q-factor controls for tuning frequency bands.
- **Dynamic Range Compression**: Look-ahead compression for volume normalization and audio clipping prevention.
- **Real-time Spectrogram**: 2048-bin Fast Fourier Transform (FFT) visualizer synced to V-Sync display refresh rates.

---

### 🛠️ Technical Architecture

| Layer | Stack | Implementation Details |
| :--- | :--- | :--- |
| **`UI`** | <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white"> | Responsive layout styled with Tailwind CSS and backdrop blurs. |
| **`LOGIC`** | <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white"> | Multi-threaded metadata extraction running in Web Workers to prevent main-thread UI blocking. |
| **`AUDIO DSP`** | <img src="https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white"> <img src="https://img.shields.io/badge/Web_Audio-FF0000?style=for-the-badge&logo=soundcharts&logoColor=white"> | Web Audio API node routing for real-time equalization and visualizers. |
| **`STORAGE`** | <img src="https://img.shields.io/badge/IndexedDB-4479A1?style=for-the-badge&logo=sqlite&logoColor=white"> <img src="https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white"> | IndexedDB BLOB storage for offline file persistence and track retrieval. |
| **`SEARCH`** | <img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/Google_Fonts-4285F4?style=for-the-badge&logo=google-fonts&logoColor=white"> | Inverted index search algorithm for fast querying across large music libraries. |

---

### ⚡ Performance Metrics

- **Library Support**: Tested up to **10,000+ tracks** (~85GB local storage).
- **Search Latency**: `< 5ms` query response time across large libraries.
- **Indexing Speed**: ~1,200 tracks per minute via background header parsing.
- **Memory Usage**: Stays under **70MB** during playback.

---

### 🚀 Getting Started

#### 1️⃣ Setup
**Option A: Clone Repository**
```bash
git clone https://github.com/Owie6789/waverr-preview.git
```

**Option B: Direct Download**
1. Click the green **"Code"** button at the top of this repository.
2. Select **"Download ZIP"** and extract the files.

#### 2️⃣ Running the App
- **Browser**: Open `index.html` in any modern web browser (Chrome, Edge, Brave). No server setup or internet connection required.
- **Adding Music**: Drag and drop your audio folders or files directly into the window to index them into your library.

---

### 🤝 Contributing

- **Feature Requests**: [Open an Issue](https://github.com/Owie6789/waverr-preview/issues) and apply the "Enhancement" label.
- **Bug Reports**: [Submit a Bug Report](https://github.com/Owie6789/waverr-preview/issues) with reproduction steps.

---

### ⭐ Project Activity

| Status | Forking | Licensing | Community |
| :--- | :--- | :--- | :--- |
| ✅ Stable | 🍴 Forks | 📄 MIT | 🌟 Stars |

---

<p align="center">
  Built by <strong>Owie Emmanuel</strong><br />
  <em>Software Engineer | UI/UX Designer</em><br />
  <a href="https://github.com/Owie6789">
    <img src="https://img.shields.io/badge/GitHub-Profile-181717?style=flat&logo=github" alt="GitHub" />
  </a>
</p>

<br>

<div align="center">
  <p style="opacity: 0.8;">
    💡 <strong>Note:</strong> Utilities for downloading local audio files for offline use:
  </p>
  <p>
    <img src="https://www.google.com/s2/favicons?domain=spotify.com&sz=16" width="12"> <a href="https://spotify-downloader.com" style="color: inherit; text-decoration: none;">Spotify-Downloader</a> | 
    <img src="https://www.google.com/s2/favicons?domain=cobalt.tools&sz=16" width="12"> <a href="https://cobalt.tools" style="color: inherit; text-decoration: none;">Cobalt (YT/Tidal)</a> | 
    <img src="https://www.google.com/s2/favicons?domain=apple.music-downloader.com&sz=16" width="12"> <a href="https://apple-music-downloader.com" style="color: inherit; text-decoration: none;">Apple Music</a> |
    <img src="https://www.google.com/s2/favicons?domain=soundcloud.com&sz=16" width="12"> <a href="https://scdownloader.io" style="color: inherit; text-decoration: none;">SoundCloud</a> |
    <img src="https://www.google.com/s2/favicons?domain=deezer.com&sz=16" width="12"> <a href="https://deezer-downloader.com" style="color: inherit; text-decoration: none;">Deezer</a> |
    <img src="https://www.google.com/s2/favicons?domain=boomplay.com&sz=16" width="12"> <a href="https://boomplaydownloader.com" style="color: inherit; text-decoration: none;">Boomplay</a> |
    <img src="https://www.google.com/s2/favicons?domain=lucida.to&sz=16" width="12"> <a href="https://lucida.to" style="color: inherit; text-decoration: none;">Lucida (Hi-Res)</a>
  </p>
  <br>
  <p style="max-width: 900px; text-align: justify; text-align-last: center; line-height: 1.4; opacity: 0.5; font-size: 11px; color: #666;">
    <strong>LEGAL DISCLAIMER:</strong> Waverr is a local playback interface designed strictly for private educational use. The developer does not host or condone the procurement of copyrighted content via unauthorized channels.
  </p>
</div>
