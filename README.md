# 🐟 Koi Pond

A Snake-style browser game where you guide a koi fish to eat lily pads. Each pad makes you longer and faster. Hit a wall or your own tail and it's game over.

**Play it:** `https://velmurugankrct.github.io/koi-pond/` (after enabling GitHub Pages, see below)

## Features

- Smooth game loop with speed that increases as your score grows
- Keyboard controls (arrow keys / WASD), swipe gestures and on-screen buttons for mobile
- Pause and resume (Space or button)
- High score saved in the browser (localStorage)
- Responsive layout with automatic light and dark mode

## Tech stack

- HTML5, CSS3
- JavaScript (vanilla, no frameworks)
- Canvas API for rendering

## Run locally

1. Download or clone this repository
2. Open `index.html` in any modern browser

```bash
git clone https://github.com/Velmurugankrct/koi-pond.git
cd koi-pond
# then double-click index.html
```

## How it works

| Part | Responsibility |
|------|----------------|
| `reset()` | Creates the starting snake, score and first lily pad |
| `loop()` / `step()` | Moves the snake each tick, checks collisions, handles eating |
| `placeFood()` | Picks a random free cell for the next lily pad |
| `turn()` | Queues direction changes and blocks 180° reversals |
| `draw()` | Renders the pond, lily pad and koi on the canvas |

## Controls

| Action | Desktop | Mobile |
|--------|---------|--------|
| Steer | Arrow keys / WASD | Swipe or on-screen arrows |
| Pause | Space | Pause button |

## Ideas for future improvements

- Difficulty levels
- Sound effects
- Online leaderboard
- Obstacles and power-ups

## License

MIT, see [LICENSE](LICENSE).
