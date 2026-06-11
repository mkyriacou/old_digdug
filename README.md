# Web Digger

A single-file web tribute to **Digger** (Windmill Software, 1983) — the CGA PC
classic where you drive a little digging machine through the dirt, hoovering up
emeralds while gold bags teeter overhead and Nobbins pour out of the door in the
top-right corner. Authentic CGA magenta-and-cyan look (with a VGA-ish alternate
palette), chunky 320×200 pixels, PC-speaker-style synth, and faint CRT scanlines.

All code, pixel art, and the background tune are original. (The 1983 game played
"Popcorn", which is still under copyright — this version has its own chip loop —
but the public-domain Rossini gallop in bonus mode and the Chopin funeral march
on death survive.)

## Play

Open `index.html` in any modern browser — no build, no dependencies, no server
needed.

## Controls

| Key | Action |
|---|---|
| Arrows / WASD | Drive + dig |
| Space (or Ctrl) | Fire bolt (slow recharge — watch the FIRE light) |
| Enter | Start |
| P | Pause |
| M | Mute |
| C | Toggle CGA / VGA palette |

## The rules, like you remember them

- **Emeralds** are 25 points; grab 8 in quick succession for a 250 bonus
  (the pickup blip rises in pitch as the streak builds).
- **Gold bags** wobble when undermined, then fall. Two rows or more and they
  burst into gold worth 500. One row and they land intact — push them along
  tunnels to set up another drop. Anything underneath gets flattened.
- **Nobbins** chase you through the tunnels (250 if you shoot or crush one).
  Leave them stewing too long and they morph into **Hobbins**, which dig their
  own tunnels and devour emeralds, gold, and even bags on the way to you.
- When the level's last monster has entered, a **cherry** appears at the door:
  1000 points and a bonus spell — the screen inverts and you eat the fleeing
  monsters for 200, 400, 800, 1600…
- A level ends when every emerald is gone or every monster is dealt with.
- Extra life every 20,000. Hi-score persists in localStorage.
- 8 hand-made level layouts that cycle with rising speed, monster counts, and
  meaner spawn odds.
