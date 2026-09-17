# Movingpoint# MovingPoint 🕹️⚡
> **Redirect momentum. Outsmart hazards. Find the true path.**
**MovingPoint** is a sleek, hyper-satisfying casual logic puzzle game inspired by *AmazeGo*. Players navigate a grid by following directional arrows to reach a hidden exit portal while dodging dynamic hazards, timed laser barriers, and moving patrols.
---
## 📸 Overview & Visuals
* **Style:** Cyberpunk Minimalist / Dark Vector
* **Palette:** Obsidian Black (`#0A0A10`), Glowing Cyan (`#00F0FF`), Neon Magenta (`#FF0055`), Electric Gold (`#FFD700`)
* **Platform:** Web / HTML5 (Phaser.js) — Playable on Desktop & Mobile
---
## 🎮 Gameplay & Mechanics
* **Directional Movement:** Swiping or launching moves your point continuously along arrow paths until hitting a wall or tile modifier.
* **Rotatable Arrows:** Tap designated arrow tiles to rotate their orientation 90° clockwise.
* **Hazards & Obstacles:**
  * **Static Hazards:** Spikes (Instant Reset) & Solid Walls.
  * **Timed Hazards:** Laser Gates (Toggle active state every $N$ turns).
  * **Dynamic Hazards:** Patrol Drones moving along fixed tile routes.
  * **Path Modifiers:** One-Way Gates, Teleporters, Step-Activated Shifters, and Decoy Exits.
---
## 📈 Level Progression Matrix

| Level Range | Grid Size | Key Mechanics | Hazard Density | Avg. Moves |
| :--- | :--- | :--- | :--- | :--- |
| **1–15** | $5 \times 5$ | Static Arrows, Basic Walls | 10% | 3–6 |
| **16–40** | $7 \times 7$ | Tap-to-Rotate Arrows, Timed Lasers, Patrols | 25% | 7–12 |
| **41–75** | $9 \times 9$ | Color Keys, Step Shifters, Strict Move Counters | 40% | 12–18 |
| **76–100+** | $12 \times 12$ | Fog-of-War, Dynamic Exit Portals, Decoy Exits | 60% | 20+ |

---
## 🛠️ Project Architecture
```text
MovingPoint/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Pages auto-deployment
├── assets/
│   ├── images/                # Sprites, tiles, UI icons
│   └── audio/                 # Sound FX & haptics
├── src/
│   ├── scenes/                # Boot, MainMenu, GameScene, LevelSelect
│   ├── objects/               # Player, ArrowTile, Hazard, ExitPortal
│   ├── logic/                 # GridManager, PathSolver, DirectionUtils
│   └── data/
│       └── levels.json        # Level configuration & grid matrices
├── index.html                 # Main entry point
├── package.json               # Dependencies & scripts
└── README.md                  # Project documentation
game that clears the mind
