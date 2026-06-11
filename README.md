# Tunnel Trouble

A single-file web tribute to the classic 1983 tunnel-digging arcade game, styled
after its MS-DOS/CGA port — magenta-and-cyan four-color palette, chunky pixels,
PC-speaker-style bleeps, and faint CRT scanlines. All code, pixel art, and sounds
are original.

## Play

Open `index.html` in any modern browser — no build, no dependencies, no server
needed (a local server like `python -m http.server` works too).

## Controls

| Key | Action |
|---|---|
| Arrows / WASD | Move + dig tunnels |
| Space (or Ctrl) | Fire the air pump; tap/hold to inflate a snagged monster |
| Enter | Start |
| P | Pause |
| M | Mute |
| C | Toggle CGA / VGA palette |

## How it works

- Dig through four dirt bands; deeper kills score more (200–500 per pop).
- Harpoon a monster, then pump it four times to pop it. Walking away lets it
  deflate and resume the chase.
- **Puffers** roam the tunnels; when frustrated they turn into ghost-eyes and
  drift straight through dirt at you.
- **Dragons** breathe fire down open tunnels — popping one sideways pays double.
- Dig under a **rock** to drop it: 1000 points per flattened monster, and after
  two dropped rocks a bonus veggie appears at the center shaft.
- The last survivor flees to the surface and runs off the screen.
- Extra life at 20,000. Hi-score persists in localStorage.
