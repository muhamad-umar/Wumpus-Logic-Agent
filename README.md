# Wumpus-Logic-Agent
A web-based simulation of the classic Wumpus World where a knowledge-based agent uses propositional logic and resolution to infer safe moves.

## 🚀 Live Demo

Experience the working AI agent here:

🔗 **Deployed on Vercel:**  
https://wumpus-logic-agent-rho.vercel.app

## Project Contents

* `index.html` — user interface with configuration controls, a board view, legend, and status dashboard.
* `style.css` — dark UI styling for the game board, controls, and dashboard panels.
* `app.js` — logic engine that builds the world, constructs the Knowledge Base (KB), and performs resolution-based inference.

## Application Overview

The application creates a grid world with pits, Wumpus, and gold. The agent starts in the bottom-left corner and updates its beliefs using percepts from the current cell.

### Core behavior

* The world generator places pits and Wumpus outside the starting zone and ensures the gold is not isolated behind pits.
* The agent records visited cells, proven safe cells, and danger cells.
* Percepts (`breeze`, `stench`, `glitter`) are converted into CNF clauses and added to the KB.
* The agent uses resolution refutation to prove whether a cell is safe or contains hazards before moving.
* The agent can plan safe paths using BFS over known-safe nodes.

## Features

* Grid size controls from 3x3 up to 8x8.
* Configurable pit count and Wumpus count.
* Step-by-step and auto-run controls for the agent.
* Live dashboard showing clause counts, inference steps, current position, percepts, and entailment results.
* Safety-first decision making with speculative shooting only when necessary.

## Usage

1. Open `index.html` in a browser.
2. Adjust grid rows, columns, pit count, and Wumpus count.
3. Click `New Game` to generate a new world.
4. Use `Step Agent` or `Auto Run` to simulate the agent.
   
## 👨‍💻 Author

**Muhammad Umar**  
🎓 BS Computer Science Student  
🏫 FAST-NUCES (CFD Campus)  
📌 Roll No: 24F-0605  

---

## 🔗 Connect

- LinkedIn: www.linkedin.com/in/muhamad-umar  
- GitHub: https://github.com/muhamad-umar  
