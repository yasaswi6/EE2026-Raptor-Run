# Raptor Run

Raptor Run is a single-player game developed as part of an EE2026 project. The game is built for an FPGA board with an OLED display connected to the JC PMOD port. Players control a dinosaur character that must navigate obstacles by jumping, ducking, and moving forward or backward. The game features four levels of increasing difficulty, each with progressively faster obstacle speeds.

## Table of Contents
- [Getting Started](#getting-started)
- [Game Controls](#game-controls)
- [Gameplay](#gameplay)
- [Features](#features)
- [Contributors](#contributors)

## Getting Started

To start the game:
1. Use the Left (BTNL) and Right (BTNR) buttons to select your desired difficulty level from 1 to 4.
2. Toggle SW[15] to start the game.

The 7-segment display will act as a timer, tracking the duration of your gameplay.

## Game Controls

The game includes the following controls:
- **BTNU (Up)**: Makes the dinosaur jump. Press twice quickly to perform a double jump.
- **BTND (Down)**: Allows the dinosaur to duck under flying bird obstacles.
- **BTNL (Left)**: Moves the dinosaur backward.
- **BTNR (Right)**: Moves the dinosaur forward.

## Gameplay

### Main Menu
When the game loads, you'll see a dinosaur on the menu screen. Choose your level using the Left and Right buttons.

### Obstacles
The obstacles, including different types of cacti and birds, appear randomly and scroll across the screen. Each level speeds up the obstacles, making the game more challenging. Collision with an obstacle triggers the Game Over screen.

### Game Over
When you collide with an obstacle:
- The OLED display shows a Game Over screen with an animated dinosaur breathing fire.
- The 7-segment display shows "OVER."
- You can press any button to return to the main menu and start a new game.

## Features

### Obstacle Generation and Speed Control
- Obstacles include green cacti (single and double), tall cacti, and flying birds.
- The game adjusts obstacle speed based on the selected difficulty level.

### Obstacle Detection and Game Over Screen
- Collision detection ensures the game ends when the dinosaur hits an obstacle.
- The Game Over screen displays an animation and prompts the player to restart.

### Score Counter
- The score increments based on how long the player survives.
- A separate module tracks and displays the score on the 7-segment display.

### In-Game Animation and LED Effects
- The dinosaur’s movements, including jumps and slides, are animated.
- Background cloud animations and LED-based Easter eggs add depth to gameplay.

## Contributors

- **Christopher Tjahyadi** - Obstacle generation and speed control.
- **Jaiswal Yasaswi** - Obstacle detection and Game Over screen.
- **Ong Qi Zhi Ignatius** - Menu design and score counter.
- **Saiful Imran** - In-game dinosaur animation, cloud animations, and LED-based special effects.
