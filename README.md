# 🔮 SPELL DUEL

> A browser-based fantasy dueling game controlled entirely by real-time hand gestures — no installs, no controllers, just your webcam and your hands.

---

## ✨ What It Is

**Spell Duel** is a single-file web game where you cast spells by making hand gestures in front of your camera. Using Google's MediaPipe Hands library for real-time hand tracking, the game reads your finger positions and fires spells at an AI enemy. Fight through escalating waves, manage your HP and mana, chain combos, and survive as long as you can.

Built entirely in vanilla HTML, CSS, and JavaScript — no frameworks, no bundler, no server needed.

---

## 🖐️ How to Play

Open `spell-duel.html` in **Google Chrome**, allow camera access, and use these gestures to cast:

| Gesture | Spell | Effect |
|---|---|---|
| ☝️ Point (index finger up) | **Fireball** | Fast projectile, moderate damage |
| ✌️ Peace (index + middle up) | **Lightning** | Stuns the enemy briefly |
| 🖐️ Open Hand (all fingers up) | **Shield** | Blocks the next enemy attack |
| ✊ Fist (all fingers down) | **Void Blast** | Heavy damage, high mana cost |

Hold a gesture for ~350ms to cast — this prevents accidental triggers from shaky hands or bad cameras.

---

## 🎮 Features

- **Real-time hand gesture recognition** via MediaPipe Hands (works even on low-quality webcams)
- **4 spells** with unique visuals, cooldowns, and mana costs
- **AI enemy** that attacks on a timer — gets faster and tougher each wave
- **Wave system** with scaling difficulty
- **Combo multiplier** for rapid kills
- **HP & mana bars**, score tracking, and live HUD
- **Particle effects** and animated wizard figures on a canvas-rendered arena
- **Procedural sound effects** via the Web Audio API — no audio files needed
- **Animated starfield background**
- **Live camera preview** with mirrored hand tracking feedback
- Dark fantasy aesthetic with the Cinzel & Share Tech Mono fonts

---

## 🚀 Getting Started

### Requirements

- **Google Chrome** (required — MediaPipe camera access works best in Chrome)
- A **webcam**
- No internet connection needed after the page loads (MediaPipe loads from CDN on first visit)

### Run It

1. Download or clone this repo
2. Open `spell-duel.html` directly in Chrome
3. Allow camera access when prompted
4. Wait for the loader to finish, then click **BEGIN**

That's it. No npm, no build step, no server.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands) | Real-time hand landmark detection |
| HTML5 Canvas | Game rendering (arena, projectiles, particles, figures) |
| Web Audio API | Procedurally generated sound effects |
| Vanilla JS | All game logic — no frameworks |
| Google Fonts (Cinzel, Share Tech Mono) | UI typography |

---

## 📁 Project Structure

```
spell-duel/
└── spell-duel.html    # The entire game — HTML, CSS, and JS in one file
```

---

## 🤔 Known Limitations

- **Chrome only** — MediaPipe camera utils have limited support in other browsers
- Gesture detection may struggle in very low light or with fast hand movement
- The AI enemy doesn't learn or adapt strategically — difficulty scales by speed and HP only

---

## 🙌 Credits

Made by **Ak**

---

## 📄 License

Feel free to fork, remix, and build on this. Credit appreciated but not required.
