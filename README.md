# 🕯️ RUN, CHASE, RUN!

*A 16-bit horror side-scroller developed by **Chase Jennings**. The Grave King has stolen Leah — run the haunted graveyard, with your black German Shepherd at your side, and bring your bride home.*

One HTML file. No dependencies, no build step. Runs in any browser and is built for phones.

![genre](https://img.shields.io/badge/genre-16--bit%20horror-purple) ![deps](https://img.shields.io/badge/dependencies-none-green)

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
| **Drag your thumb** left/right on the left half of the screen — move | Arrow keys / A & D |
| JUMP button, or tap the right half of the screen | Space / W / Up |
| FIRE button — fireball | X / F / J |

## 💀 How to survive

- **Rescue Leah** — she's held at the crypt door at the far end of the graveyard.
- **Stomp zombies and flying eyeballs** — jump on their heads, classic style — or **burn them with fireballs**.
- **Watch the ceilings.** Spiders drop down on silk threads when you walk under them.
- **Never turn your back on a ghost.** It only drifts toward you while you're facing away. Stare it down and it fades back into the dark.
- **Trust your dog.** He runs at your side, and he **barks (!)** when a ghost is hunting you from behind.
- **🌙 Moon totem** — transform into a **tall werewolf**: faster, higher jumps, and everything you touch is shredded — *even ghosts*.
- **✝ Crucifix** — ghosts flee from you and can't harm you while the holy timer runs.
- **♥ Hearts** — restore health (or +500 if you're full).
- **Candles are souls.** Collect 10 and a heart comes back.
- **Skull blocks** hide souls — bump them from below. Bricks smash.
- Spikes and pits send you back to the last **lantern checkpoint**.
- Out of hearts? **Tap to continue** from your lantern — your score and souls are kept.

You have 3 hearts. The graveyard is patient.

## 🔧 Tech

- Single-file HTML5 canvas game at a 320×192 internal resolution, integer-scaled with `image-rendering: pixelated` for crisp pixels
- All sprites drawn in code (pixel-map strings) in a 16-bit style — Chase (with his leather pack strap and jeans), Leah (lace gown, bouquet, tattoo sleeve), werewolf Chase, the dog, and the Grave King — plus a tiny 3×5 bitmap font, procedural cobblestone tiles, and a distant castle with lit windows
- Opening cutscene: the Grave King snatches Leah away before the level begins (tap to skip)
- Adaptive viewport: the view expands to fill any phone edge-to-edge at a fixed pixel zoom
- **Three-track chiptune soundtrack**, sequenced live through WebAudio (zero audio files): a D-minor graveyard waltz, a fast action riff while you're the werewolf, and a bright D-major victory tune when Leah is rescued
- Companion-dog AI (follows, hops gaps, warns of ghosts), multi-touch on-screen controls, jump buffering + coyote time, parallax night sky with towering peaks and a distant lit castle, drifting fog, and lightning
