[🇹🇷 Click here for Turkish](README.tr.md)

# futoshiki

A cyberpunk-themed, browser-based Futoshiki puzzle game. Built as a single-page HTML application with neon visuals, animated backgrounds, and full responsive support.

---

## Features

### 1. Game Board
- **4×4 and 5×5** grid modes
- Inequality symbols: `<` / `>` (horizontal), `∧` / `∨` (vertical) — the tip always points to the smaller value

### 2. Difficulty Levels
- **EASY / MEDIUM / HARD** — adjusts the number of pre-filled cells and countdown duration
  - 4×4: Easy = 2 min, Medium = 3 min, Hard = 4.5 min
  - 5×5: Easy = 4 min, Medium = 6 min, Hard = 8 min

### 3. Countdown Timer
- Counts down from the difficulty-based limit
- Flashes red with a pulse animation during the last 10 seconds

### 4. Controls
- **Numpad:** digit buttons (1–N) + ✕ (erase) button
- **RESET** — restart the current puzzle
- **SOLUTION** — reveal the full solution
- **CHECK** — validate your current progress

### 5. Success Modal
- Displays **"ACCESS GRANTED"** when the puzzle is solved correctly

### 6. Background Music
- Plays `mp3/music.mp3` on load
- Toggle with the ♪ / × button

### 7. Help Button (?)
- Opens the rules modal without resetting the game

### 8. Cyberpunk Visual Theme
- Scanlines overlay, neon grid pulse, floating particle animations
- Glassmorphism panels, Orbitron & Rajdhani Google Fonts

### 9. Responsive Design
- Optimised for mobile (portrait), tablet, and desktop
- Landscape mode on mobile shows a rotate-device warning

### 10. Puzzle Solver
- `minimizeInequalities` function guarantees a unique solution for every generated puzzle

---

## Project Structure

```
futoshiki/
├── index.html    — full application (HTML/CSS/JS in a single file)
└── mp3/
    └── music.mp3 — background music
```

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/miyigun/futoshiki.git
   ```
2. Enter the project folder:
   ```bash
   cd futoshiki
   ```
3. Open `index.html` in your browser — no build step or server required.

---

## How to Play

1. Choose a grid size (**4×4** or **5×5**) and a difficulty level (**EASY**, **MEDIUM**, or **HARD**).
2. Fill each cell with a number so that every row and column contains each digit exactly once.
3. Respect all inequality signs — the tip of each symbol (`<`, `>`, `∧`, `∨`) always points to the smaller number.
4. Use the **CHECK** button to verify your answers at any time.
5. Stuck? Press **SOLUTION** to see the correct answer, or **RESET** to start over.
6. Solve the puzzle before the countdown timer runs out!

---

## 🛠️ Technologies Used

- HTML5 / CSS3 / Vanilla JavaScript
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- [jQuery](https://jquery.com/) 3.7.1
- [Google Fonts](https://fonts.google.com/) — Orbitron & Rajdhani

---

## 📌 Notes

- No installation or build tools are needed — just open `index.html`.
- The puzzle generator always produces a board with a unique, valid solution.
- Background music requires browser autoplay permission; use the ♪ / × toggle if it does not start automatically.
- The game is fully self-contained in a single `index.html` file.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.