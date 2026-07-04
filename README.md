# 🍥 Naruto Jutsu Hand Tracker

Turn your webcam into a jutsu machine. Open your palm, watch the Rasengan or Chidori appear — no app, no gloves, no sensors. Just your browser.

## 🎥 Demo
Live:  https://powerpunch.pages.dev/

## ⚡ How it works
- **MediaPipe Hands** tracks 21 landmarks per hand in real time via webcam
- When your palm opens, the tool detects it (comparing fingertip distance to knuckle distance from the wrist)
- Left hand → Rasengan overlay (Naruto)
- Right hand → Chidori overlay (Sasuke)
- Overlays fade in/out smoothly based on how "open" your hand is, tracked frame-by-frame
- Background music fades in on load for that extra dramatic entrance

No backend. No build step. Just one HTML file.

## 🛠 Tech Stack
- Vanilla JavaScript
- [MediaPipe Hands](https://github.com/google/mediapipe) for hand landmark detection
- Canvas API for skeleton overlay rendering
- HTML5 video/audio for effects and BGM

## 🚀 Run it locally
1. Clone this repo
2. Add your own `assets/naruto.mp4`, `assets/sasuke.mp4`, and `assets/bgm.mp3` (not included — copyright reasons)
3. Open `index.html` in a browser (needs webcam permission)
4. That's it — no npm install, no build tools, nothing

```bash
git clone <your-repo-url>
cd naruto-hand-tracker
# just open index.html — or serve it locally:
python3 -m http.server 8000
```

## 📋 Requirements
- A webcam
- A browser that supports `getUserMedia` (Chrome/Edge/Firefox — all modern browsers)
- Decent lighting for hand detection to work well

## 🎬 Credits
Built solo as a fun experiment mixing anime nostalgia with computer vision. Naruto/Sasuke assets belong to their respective copyright holders — used here for non-commercial fan content only.

## 📬 Found this from the reel?
Drop a follow, and feel free to fork/remix it. If you build something cool with it, tag me — would love to see it.

---
⭐ If this made you smile, star the repo.
