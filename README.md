# 2048 Game

## Introduction

Welcome to the **2048 Game** project, a vanilla JavaScript implementation of the classic 2048 puzzle game. Players slide numbered tiles on a 4×4 grid, merging matching tiles to reach the **2048** tile. The game is built with modern web technologies and delivers a smooth, responsive experience across all devices.

## Live Demo

[Play the game](https://eg598.github.io/2048-game/)

## Key Features

- **Tile Movement and Merging**: Accurate logic for sliding and combining tiles in all four directions using arrow keys.
- **Random Tile Spawning**: After every valid move, a new tile (2 with 90% chance, 4 with 10% chance) appears in a random empty cell.
- **Score Tracking**: Real-time score updates as tiles are merged throughout the game.
- **Win and Lose Conditions**: The game detects when the player reaches 2048 (win) or has no valid moves remaining (lose) and displays the appropriate message.
- **Restart Functionality**: A Start/Restart button lets the player reset the board at any time.
- **Responsive Design**: The layout adapts to desktops, tablets, and mobile screens.

## Challenges

Building this project presented several non-trivial problems that required careful design decisions.

**Key Challenges:**

- **Tile Movement Logic**: Correctly shifting and merging tiles along each axis while preventing double-merges in a single move required precise array manipulation.
- **Game State Management**: Tracking the board configuration, score, and game status (idle / playing / won / lost) without external libraries demanded disciplined state handling.
- **Win/Lose Detection**: Efficiently checking for available moves when the board is full — without false positives — needed thorough edge-case coverage.
- **Responsive Layout**: Keeping the grid visually consistent and playable across a wide range of screen sizes involved careful SCSS structuring.

## Technical Requirements

To run this project locally, you will need:

- A modern web browser (latest versions of Chrome, Firefox, Safari, or Edge)
- Node.js (version 16.x or newer)
- npm (version 8.x or newer)

## Installation and Setup

1. Clone the repository:

```bash
git clone https://github.com/eg598/2048-game.git
```

2. Navigate to the project directory:

```bash
cd 2048-game
```

3. Install dependencies:

```bash
npm install
```

4. Start the local development server:

```bash
npm start
```

## Usage

After starting the project, it will be available at `http://localhost:1234`.

1. Click **Start** to initialize the board
2. Use **Arrow Keys** (↑ ↓ ← →) to slide all tiles in a direction
3. Tiles with the **same number** merge when they collide — their values are added together
4. Reach the **2048** tile to win
5. Click **Restart** at any time to reset the board and score

## Technologies Used

- **HTML5** — Semantic table-based game grid
- **CSS3 / SCSS** — Styling with nested rules and BEM-like class naming
- **JavaScript (ES6+)** — Game logic and DOM manipulation
- **Parcel** — Module bundler and development server
- **ESLint / Stylelint / LintHTML** — Code quality enforcement
- **Git / GitHub** — Version control and repository hosting

## Design Specifications

- **Desktop**: 1280px
- **Tablet**: 640px
- **Mobile**: 320px+
