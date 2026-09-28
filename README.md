# Shape Drop

A neon falling-and-merging puzzle game, inspired by "Shapes" on the Triumph app and the Suika (watermelon) game.

Drop shapes into a tight, tall box. Two matching shapes merge into the next shape in an 11-stage chain:

**Sliver → Chevron → Cross → Crescent → Rhombus → Gear → T-Block → Bolt → Trapezoid → Crown → Labyrinth**

Two Labyrinths make a **Supernova** and vanish for a big bonus. Don't let the pile stay over the red line!

Every shape has **real corners**: the game uses true polygon physics, so shapes wedge, jam, hook onto each other and refuse to roll. Turn your shape before you drop it to find the gaps.

## How to play

Open `index.html` in a web browser. The physics engine ([Matter.js](https://brm.io/matter-js/)) loads from the internet, so you need a connection.

| Action | Mouse / keyboard | Phone |
|---|---|---|
| Aim | Move the mouse, or ← → (A / D) | Drag your finger |
| Rotate | ↑ / W / R, scroll wheel, or right-click (Q turns the other way) | Rotate button |
| Drop | Click, or Space | Lift your finger |
| Pause | P | Tap while paused to resume |
| Mute | M | Sound button |
| Show collision pieces | G | – |

## Features

- **True polygon collisions** (Matter.js), including dented shapes built from convex pieces
- **Landing preview** that shows exactly where your shape will land, at its current angle
- **Classic Mode** (shapes merge by shape) and **Color Mode** (shape *and* color must match)
- **Sticky shapes** covered in goo that glue to whatever they touch until the goo dries
- **Power-ups:** Bigger Box, Wildcard, Bomb, Shake Up
- **Combos** for quick merges in a row (up to x3 points)
- Shatter, bubble-pop and glitch merge effects, faces on every shape, screen shake and slow motion on huge merges
- Separate high scores for each mode, saved in your browser

## Changing the game

All the easy-to-tweak numbers are in the **A. SETTINGS** section near the top of the `<script>` in `index.html`: gravity, box size, how many shapes drop, shape sizes and grip, colors, power-up and sticky-shape chances, combo rules, and effect levels. Save the file and refresh the browser to see your changes.

### Making your own shapes

Section **A2. SHAPE BLUEPRINTS** holds the corner points of every shape, on a small grid from about -1 to 1. Each blueprint has:

- `outline`: the points around the whole shape (used for drawing)
- `parts`: convex pieces that exactly fill the outline (used for physics; the engine can only collide shapes with no dents)
- `face`: where the face goes

Copy a blueprint, change the points, and use its name in `SHAPE_CHAIN`. Press **G** in the game to see the collision pieces drawn in white.

## Version history

Each change is saved as a git commit, and stable versions get a release tag (like `V1.0`). To see or restore an older version, look under **Releases / Tags** or the commit history on GitHub.
