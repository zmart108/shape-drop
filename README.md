# Shape Drop

A neon falling-and-merging puzzle game, inspired by "Shapes" on the Triumph app and the Suika (watermelon) game.

Drop shapes into a tight, tall box. Two matching shapes merge into the next shape in the chain:

**Circle → Triangle → Square → Pentagon → Hexagon → Star → Heart → Sun**

Two Suns make a **Supernova** and vanish for a big bonus. Don't let the pile stay over the red line!

## How to play

Open `index.html` in any web browser. There's nothing to install.

| Action | Mouse / keyboard | Phone |
|---|---|---|
| Aim | Move the mouse, or ← → (A / D) | Drag your finger |
| Drop | Click, or Space | Lift your finger |
| Pause | P | Tap while paused to resume |
| Mute | M | Sound button |

## Features

- **Classic Mode** (shapes merge by shape) and **Color Mode** (shape *and* color must match)
- **Sticky shapes** covered in goo that glue to whatever they touch until the goo dries
- **Power-ups:** Bigger Box, Wildcard, Bomb, Shake Up
- **Combos** for quick merges in a row (up to x3 points)
- Shatter, bubble-pop and glitch merge effects, faces on every shape, screen shake and slow motion on huge merges
- Separate high scores for each mode, saved in your browser

## Changing the game

All the easy-to-tweak numbers are in the **A. SETTINGS** section near the top of the `<script>` in `index.html`: gravity, box size, how many shapes drop, colors, power-up and sticky-shape chances, combo rules, the shape chain, and effect levels. Save the file and refresh the browser to see your changes.

## Version history

Each change is saved as a git commit, and stable versions get a tag (like `v1.0`). To see or restore an older version, look under **Releases / Tags** or the commit history on GitHub.

## Bonus game: Neon Dunk

`neon-dunk/index.html` is a separate one-file neon arcade game in the style of Flappy Dunk. Tap, click or press Space to bounce the ball, and drop it through hoops that alternate between the walls. Two swishes in a row (no rim touch) start **Fever Mode**, which adds a lightning trail and a growing multiplier. The floor is super bouncy but breaks after 3 bounces per hoop. Press M to mute.
