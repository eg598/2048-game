# 2048 Game

A browser-based implementation of the classic **2048 puzzle game**, built with vanilla JavaScript, HTML, and SCSS.

## Live Demo

[Play the game](https://eg598.github.io/2048-game/)

## About the Project

The goal is to slide numbered tiles on a 4×4 grid and merge matching tiles to reach the **2048** tile. Each move spawns a new tile (2 or 4) in a random empty cell. The game ends when no moves are left.

### Game Rules

- Use **arrow keys** to slide all tiles in a direction
- Two tiles with the **same number** merge into one when they collide
- A new tile (**2** with 90% chance, **4** with 10% chance) appears after every valid move
- **Win** by creating a tile with the value `2048`
- **Lose** when the board is full and no merges are possible

## Technologies Used

- **JavaScript (ES6+)** — Game logic and DOM manipulation
- **SCSS** — Styling with nested rules and BEM-like class naming
- **HTML5** — Semantic table-based game grid
- **Parcel** — Bundler and dev server
- **ESLint / Stylelint / LintHTML** — Code quality

```

## Getting Started

### Prerequisites

- Node.js v16+
- npm

### Installation

1. Clone the repository:

```bash
git clone https://github.com/eg598/2048-game.git
cd 2048-game
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm start
```

### Lint

```bash
npm run lint
```

## How to Play

1. Click **Start** to begin
2. Use **Arrow Keys** to move tiles
3. Merge tiles of the same value to double them
4. Reach the **2048** tile to win
5. Click **Restart** at any time to reset the board
