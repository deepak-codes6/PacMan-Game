# Project Statement

## Project Title
**Pacman Game **

## Problem Statement
The objective of this project is to design and implement a fully functional,2D arcade-style Pacman game using core Java and the Swing GUI library, 
demonstrating the practical application of object-oriented programming concepts, event-driven programming, and real-time graphics rendering.

## Objectives
1. To implement a tile-based game map that defines walls, pathways, ghost spawn points, and collectible items.
2. To implement smooth player-controlled movement using keyboard input (arrow keys) with collision detection against walls.  
3. To implement autonomous ghost movement with random direction changes upon collision.
4. To implement a scoring system based on food collection.
5. To implement a lives system with game-over detection.

## Scope of the Project
- The game is a single-player, single-level implementation.
- The game runs locally as a desktop application (no networking or  multiplayer functionality).
- The map layout, ghost count, and starting positions are fixed and   defined within the source code.
- The project does not include persistent storage (high scores reset when the application is closed) -
   this is listed as a future enhancement.

  ## Methodology
1. **Research & Learning** 
    Studied the fundamentals of 2D game development in Java, including the game loop pattern, Swing's `JPanel`/`JFrame` rendering pipeline,
    and `KeyListener`-based input handling,  using an existing open-source tutorial as a structural reference.
  
  2. **Base Implementation** 
  Understood and set up the core game  architecture — map parsing, sprite loading, movement logic, and collision detection.

## Target Users

- **Casual players** who want a quick, familiar arcade game that runs locally with no installation beyond a Java runtime.
- **Students learning Java** who want a readable, dependency-free reference for how a game loop, collision detection and Swing rendering fit together in a real program.
- **Evaluators and reviewers** assessing the practical application of object-oriented design, event-driven programming and real-time rendering in core Java.
- **Anyone extending the project** — the tile map is plain text and the entity model is a single reusable class, so new mazes, ghosts or collectibles can be added without touching the rendering logic.
  

## High-Level Features

| # | Feature | Description |
|---|---|---|
| 1 | Tile-based maze | The map is stored as a character grid and parsed once at start-up into walls, food, power food, ghosts and Pacman. |
| 2 | Player movement | Arrow-key control with the sprite rotating to face the direction of travel; turns into walls are rejected rather than clipped. |
| 3 | Wall collision | Axis-aligned bounding-box detection; a blocked move is reverted so entities rest flush against walls. |
| 4 | Ghost movement | Four ghosts move autonomously and pick a new random direction whenever a move is blocked. |
| 5 | Food and scoring | Pellets are removed on contact and the score increases; the live score is drawn on screen. |
   
   ## Expected Outcome
A playable, bug-free Pacman game that demonstrates:
- Correct application of object-oriented design (Block, PacMan classes)
- Real-time rendering and animation
- Functional game mechanics (movement, collision, scoring, power-ups)
- Clean, readable, and well-documented source code

