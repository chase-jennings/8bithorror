# 🕯️ GRAVE CHASE

*A spooky 8-bit side-scroller starring **Chase Jennings** — and his faithful black German Shepherd.*

One HTML file. No dependencies, no build step. Runs in any browser and is built for phones.

![genre](https://img.shields.io/badge/genre-8--bit%20horror-purple) ![deps](https://img.shields.io/badge/dependencies-none-green)

## ▶️ Play it

**On your phone (easiest):** enable GitHub Pages for this repo
(**Settings → Pages → Deploy from a branch**, pick the branch, `/ (root)` folder), then open:

```
https://chase-jennings.github.io/8bithorror/
```

Turn your phone **sideways** (landscape) for the best experience, tap once, and run.

**On a computer:** just open `index.html` in a browser, or serve it locally:

```
python3 -m http.server 8000
# → http://localhost:8000
```

## 🎮 Controls

| Phone | Keyboard |
|---|---|
| ◀ ▶ buttons — move | Arrow keys / A & D |
| JUMP button | Space / W / Up |

## 💀 How to survive

- **Stomp zombies and bats** — jump on their heads, classic style.
- **Never turn your back on a ghost.** It only drifts toward you while you're facing away. Stare it down and it fades back into the dark.
- **Trust your dog.** He runs at your side, and he **barks (!)** when a ghost is hunting you from behind.
- **🌙 Moon totem** — transform into a **tall werewolf**: faster, higher jumps, and everything you touch is shredded — *even ghosts*.
- **✝ Crucifix** — ghosts flee from you and can't harm you while the holy timer runs.
- **♥ Hearts** — restore health (or +500 if you're full).
- **Candles are souls.** Collect 10 and a heart comes back.
- **Skull blocks** hide souls — bump them from below. Bricks smash.
- Spikes and pits send you back to the last **lantern checkpoint**.
- Reach the **glowing crypt door** at the far end of the graveyard to escape.

You have 3 hearts. The graveyard is patient.

## 🔧 Tech

- Single-file HTML5 canvas game at a true 320×192 internal resolution, integer-scaled with `image-rendering: pixelated` for chunky pixels
- All sprites drawn in code (pixel-map strings) — including 8-bit Chase, werewolf Chase, and the dog — tiny 3×5 bitmap font, procedural tiles
- **Looping 8-bit horror soundtrack**: a D-minor chiptune sequenced live through WebAudio (square lead, triangle bass, noise hats) plus an ambient drone — zero audio files
- Companion-dog AI (follows, hops gaps, warns of ghosts), multi-touch on-screen controls, jump buffering + coyote time, parallax night sky, drifting fog, lightning, and a lantern-glow darkness vignette
