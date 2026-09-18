**Overview**
#Pacman Game
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


## Future Improvements
- Smarter ghost AI (pathfinding toward Pacman instead of random movement)
- Multiple levels with increasing difficulty
- Sound effects for eating food, power pellets, and ghost collisions
- Persistent high score (saved to a file instead of resetting on restart)

  Screenshot

  

  
