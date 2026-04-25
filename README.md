# ⏱️ Minimalist Pomodoro Timer with Spotify Integration

A clean, distraction-free Pomodoro timer built using pure HTML, CSS, and JavaScript — designed for deep work sessions with optional ambient music via Spotify.

---

## 🚀 Overview

This project delivers a **zero-dependency productivity tool** with a strong focus on:

- Minimal UI
- Smooth UX transitions
- Persistent session tracking
- Integrated music workflow

It operates entirely in the browser — no backend, no frameworks, no build tools.

---

## ✨ Key Features

### ⏳ Pomodoro Timer
- Default **25 min focus / 5 min break**
- Fully customizable durations
- Auto-switch between focus and break modes
- Auto-restart after session completion

### 🎯 Session Tracking
- Visual progress using session dots
- Tracks completed focus cycles
- Scales dynamically beyond default sessions

### 🎧 Spotify Integration
- Embed any Spotify playlist
- Toggle between player and settings
- Playlist stored via `localStorage`
- Seamless UX with inline player

### 🎛️ Controls
- Start / Pause toggle
- Reset functionality
- Real-time time editing (when paused)

### 🧠 UX Design
- Monospace aesthetic (developer-focused)
- Minimal contrast UI (low distraction)
- Subtle animations and transitions

---

## ⚙️ How It Works

### Timer Engine
- Uses `setInterval()` for countdown
- State-driven:
  - `isRunning`
  - `isFocusMode`
  - `timeLeft`

### Mode Switching Logic
- On timer completion:
  - Switch focus ↔ break
  - Update UI indicator
  - Auto-start next session after delay

### Spotify Embed
- Extracts playlist ID via regex
- Injects into iframe:
- `https://open.spotify.com/embed/playlist/{id}`
- - Stores user playlist in `localStorage`

---

## 📦 Setup

### Direct Run
```bash
# Just open in browser
index.html
