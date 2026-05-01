# Puzzle Path Finder

[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
![Made with HTML/CSS/JS](https://img.shields.io/badge/frontend-HTML%20%2F%20CSS%20%2F%20JS-blue)
[![Open in browser](https://img.shields.io/badge/Open-in%20Browser-brightgreen)](puzzle-path-finder.html)

## 🚀 About

Puzzle Path Finder is a lightweight, single-file HTML/JS puzzle game. Players place directional arrows in a grid to guide a ball from a start point (`🟢`) to the goal (`🔴`) while avoiding walls (`▪`). The game includes keyboard navigation, fail-mode feedback, animated runners, and a built-in auto-solver.

## 🎮 Demo Screenshot

(windows screenshot shown in issue: start cell, walls, solution path, status)

- Level: 1
- Arrows: 0/active
- Steps/solved stats in UI

## 🕹️ Controls

- `← → ↑ ↓`: select arrow direction
- `W A S D`: move cursor in grid
- `Space`: place selected arrow at cursor
- `Backspace` / `Delete`: erase arrow
- `Enter`: run the path simulation
- `R`: reset level
- `🧠 Solve`: auto-solve current level

## 🧩 Gameplay

1. Select direction arrow.
2. Place arrows in open cells to form a path.
3. Start from `🟢` and end at `🔴`.
4. Avoid walls and out-of-bounds movement.
5. Run and win! On success, shows step count and arrow count.

## 🧠 Auto-solver

The `Solve` button performs BFS to find a valid path from start to end for the current level and populates arrows automatically. It helps validate level design and gives a baseline solution for players.

## 🔧 Project structure

- `puzzle-path-finder.html`: full game implementation (self-contained)
- `README.md`: project description and usage details

## 🎯 How to run

1. Clone or download repo.
2. Open `puzzle-path-finder.html` in any modern browser (Chrome/Edge/Firefox).
3. Play using the on-screen controls or keyboard shortcuts.

## 🛠️ Development notes

- Levels are defined in `LEVELS` array inside `puzzle-path-finder.html`.
- Each level has: `name`, `size`, `walls`, `start`, `end`.
- Add a level by appending object to `LEVELS`.
- A solver function updates `arrows` map and visual arrow elements.
- Grid/responsive sizing is handled by CSS and `getCellSize()`.

## ✨ Improvement ideas

- Add points + best score per level.
- Add level editor and save to localStorage.
- Add sound fx and visual particle effects.
- Add mobile gestures (drag to place path).

## 📜 License

MIT
