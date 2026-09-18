# Pacman Game
## Overview
A classic Pacman game built in Java using Swing.This project started as a way to understand 2D game development fundamentals 
in Java — game loops, collision detection, sprite rendering, and keyboard input handling.

## Features
- Classic Pacman movement using arrow keys
- Four ghosts (red, pink, blue, orange) with random/AI-driven movement
- Wall collision detection using a tile-based map system
- Food collection and scoring
- Lives system with game over screen.
- **High Score Tracking** — The game remembers the highest score achieved during the current session and displays it alongside the live score,
  updating automatically whenever a new high score is reached.
  

## Tech Stack
- **Language:** Java
- **Library:** Java Swing (JFrame, JPanel, Graphics) for rendering and windowing

  ## How to Run
1. Clone or download this repository
2. Open the project folder in VS Code (with the Java Extension Pack installed)
3. Make sure all `.png` image assets are present in **both** the `src` and 
   `bin` folders (required for the game to load sprites correctly)
4. Open `App.java` and click Run

   ## Controls
| Key | Action |
|-----|--------|
| ↑ | Move Up |
| ↓ | Move Down |
| ← | Move Left |
| → | Move Right |

## Screenshot
<img width="798" height="907" alt="Screenshot 2026-09-18 225522" src="https://github.com/user-attachments/assets/d59f723d-23af-473e-bcba-b6359ec86e45" />



## What I Learned
- How game loops work using timers and repaint cycles
- Implementing collision detection between moving and static objects
- Managing game state (lives, score, power-up timers) cleanly across frames
- Reading and parsing a tile-based map from a character array
  ## Instructions for Testing

There is no automated test runner, so the game is verified by running it and working through the scenarios below. Each one maps to a feature listed above.

## Instructions for Testing

There is no automated test runner, so the game is verified by running it and working through the scenarios below. Each one maps to a feature listed above.

| # | Test | Steps | Expected result |
|---|---|---|---|
| 1 | Launch | Run `java -cp bin App` | Window opens with the maze, Pacman, four ghosts, full food, score 0 and three lives |
| 2 | Movement | Press each arrow key on an open path | Pacman moves in that direction and the sprite rotates to match |
| 3 | Wall collision | Drive Pacman straight into a wall | Movement stops flush against the wall — no overlap or tunnelling |
| 4 | Blocked turn | Press a direction key while facing a wall | The direction change is rejected and the previous direction is kept |
| 5 | Food collection | Eat a single pellet | The pellet disappears and the score increases exactly once |
| 6 | Power food | Eat a power food | All ghosts switch to the scared sprite for the power duration |
| 7 | Eat a ghost | Touch a ghost while it is scared | Bonus points awarded, no life lost |
| 8 | Lose a life | Touch a ghost while it is **not** scared | Lives drop by one and all entities reset to their spawn positions |
| 9 | Game over | Lose all three lives | "Game Over" is displayed with the final score and the loop stops |
| 10 | Restart | Press any key after game over | Score, lives and map reset, and a new game begins |
| 11 | Level reset | Clear every pellet on the board | The maze repopulates with food and the score carries over |
| 12 | High score | Beat your previous best in the same session | The high score field updates immediately and stays for the session |
| 13 | Ghost behaviour | Watch the ghosts for about a minute | Ghosts change direction on wall contact; none gets permanently stuck |
| 14 | Stability | Play continuously for several minutes | No exceptions in the console, no frame-rate drop |

If a test fails, check the console output — asset-loading and map-parsing problems surface there first


## Future Improvements
- Smarter ghost AI (pathfinding toward Pacman instead of random movement)
- Multiple levels with increasing difficulty
- Sound effects for eating food, power pellets, and ghost collisions
- Persistent high score (saved to a file instead of resetting on restart)

  Screenshot

  

  
