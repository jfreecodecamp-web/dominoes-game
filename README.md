# Jamrock Dominoes

**JavaScript · HTML5 Canvas · CSS · Browser game prototype**

A Jamaican-themed browser game built with vanilla JavaScript and HTML5 Canvas. Play against three computer opponents, match domino ends, and keep score across successive hands.

[Play live demo](https://jfreecodecamp-web.github.io/dominoes-game/) · [Browse source](https://github.com/jfreecodecamp-web/dominoes-game/blob/main/index.html) · [Developer profile](https://github.com/jfreecodecamp-web)

## Preview

![Jamrock Dominoes — game interface](https://github.com/user-attachments/assets/84a69c22-768b-4610-b17c-cc71abf68c39)

![Jamrock Dominoes — setup and gameplay](https://github.com/user-attachments/assets/6f427e8f-874d-4a1b-8e43-0265afc59e2f)

![Jamrock Dominoes — board view](https://github.com/user-attachments/assets/a2818973-6d04-4e95-9355-5030bf5fc2c5)

## Features

- Four-player table with one human player and three computer opponents.
- Cut Throat and Partner mode selection.
- Easy, Hard, and Very Hard computer move selection; the strongest setting uses passing history when evaluating moves.
- Double-six opening, winner-led subsequent hands, and locked-hand scoring.
- Animated tile washing, drag-and-drop play, sound effects, and round-end feedback.

## Run locally

No package installation or build step is required.

```bash
git clone https://github.com/jfreecodecamp-web/dominoes-game.git
cd dominoes-game
```

Open `index.html` in a current desktop browser. For a local HTTP server, run `python -m http.server 8000` from the project directory and visit **http://localhost:8000**. Python is only needed for the optional local server.

## How to play

1. Select **Enter Game**, choose an AI skill level, then choose a game mode.
2. When it is your turn, drag a matching tile from your hand to the left or right side of the table.
3. Use **Pass** when you have no legal move. The first hand starts with double-six.
4. Finish your hand to score; if play is blocked, the lowest remaining pip count determines the hand winner.

## Implementation highlights

| Area | Implementation |
| --- | --- |
| Rendering | Canvas drawing, pip layouts, tile orientation, and animation loops. |
| Rules and state | Hands, turn order, chain ends, previous-hand winner, and score tracking. |
| Computer opponents | Legal-move generation and heuristic scoring with passing-history input. |
| Interaction | Mouse drag-and-drop and browser audio initialized from a user gesture. |

## Repository guide

| File | Purpose |
| --- | --- |
| `index.html` | Active interface, styles, game rules, Canvas renderer, and computer player logic. |
| `jamrock.mp3` | Audio asset used by the game. |

## Project status

The current prototype uses mouse controls and keeps match state in memory. Partner mode includes partner-aware move selection, while scoring is currently tracked per player.

## Planned improvements

- Add touch and keyboard controls.
- Add explicit team totals for Partner mode and a clearer match-end screen.
- Separate game rules from rendering and add focused rule tests.

## Author

**Javel Swaby** · [GitHub](https://github.com/jfreecodecamp-web)

Part of a portfolio exploring interactive interfaces, state management, and rule-based JavaScript applications.
