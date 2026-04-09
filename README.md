# ✈ Unsent

> *Messages nobody was brave enough to send.*

A shared sky of paper planes — each one carrying something someone never said. Type your unsent message, watch it fold into a plane, and let it join thousands of others drifting through the night.

---

## What It Is

Unsent is an anonymous, collaborative experience where every visitor contributes one thing they never said — to a person, to the world, to themselves. The message folds into a paper plane and joins a shared sky visible to everyone. Before it flies away, the person it was meant for finally replies.

---

## Features

### The Experience
- **Typewriter input** — mechanical click sounds on every keystroke, blinking cursor, character-by-character reveal
- **Origami fold animation** — your message physically folds into a paper plane before flying into the sky
- **AI reply** (Pollinations.ai) — before your plane joins the sky, the person you wrote to finally replies in one warm, understanding sentence
- **Shared sky** — all visitor planes visible to everyone in real time, drifting with 12 unique flight animations
- **Click any plane** — unfolds to reveal the message, anonymous city shown if geolocation granted
- **Heart / resonate** — heart messages that feel like yours; most loved planes glow warmer

### Navigation
| Filter | Shows |
|--------|-------|
| Recent | All messages, newest first |
| Most Loved | Only messages with at least 1 heart |
| Mysterious | Messages with unusually high consonant ratio — cryptic, sparse, strange |

### Audio
- **Lofi music** — generative 4-layer engine: vinyl crackle + chord progression (Cmaj7 → Am7 → Fmaj7 → G7) + soft bass + sparse piano plinks. Starts on first interaction, fades in over 4 seconds.
- **Typewriter clicks** — Web Audio noise burst on every keypress
- **Paper rustle + whoosh** — on plane fold and launch
- **Chime** — on AI reply reveal and on heart

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML / CSS / JavaScript — single file |
| 3D / Animation | CSS keyframe animations (12 unique drift paths) |
| Audio | Web Audio API — fully generative, no audio files |
| Backend | JSONBin.io REST API (free tier) |
| AI Reply | Pollinations.ai text API (no API key required) |
| Geolocation | Browser Geolocation API + Nominatim reverse geocoding |
| Fonts | Special Elite + Lora (Google Fonts) |

---

## Setup

### 1. Clone / Download
```bash
git clone https://github.com/yourusername/unsent.git
```
Or simply download `unsent.html` — it is a single self-contained file.

### 2. Configure JSONBin
1. Create a free account at [jsonbin.io](https://jsonbin.io)
2. Create a new public bin with content `[]`
3. Copy your **Bin ID** and **X-Master-Key**
4. In `unsent.html`, update these two lines:
```js
const BIN = 'your-bin-id-here';
const MKEY = 'your-master-key-here';
```

### 3. Deploy
Drop the single HTML file onto any static host:
- [Netlify Drop](https://app.netlify.com/drop) — drag and drop, live in seconds
- [Vercel](https://vercel.com)
- GitHub Pages
- Any web server

No build step. No dependencies. No npm install.

## Project Structure


## Credits

- **Pollinations.ai** — free AI text generation, no API key
- **JSONBin.io** — free JSON storage backend
- **Nominatim / OpenStreetMap** — reverse geocoding for anonymous city display
- **Google Fonts** — Special Elite, Lora
- All audio generated procedurally via Web Audio API — no audio files used

---
live demo: https://unsentmessages.netlify.app
