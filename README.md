
# Snake Game 🐍

Welcome to **Snake Game**, a classic arcade game brought to life in C++! This project showcases modular programming and efficient game mechanics to deliver a fun and engaging gameplay experience.

---

## Table of Contents
- [About the Project](#about-the-project)
- [Features](#features)
- [How to Play](#how-to-play)
- [Installation](#installation)
- [Code Architecture](#code-architecture)
- [File Structure](#file-structure)
- [Future Enhancements](#future-enhancements)
- [Acknowledgments](#acknowledgments)
- [Known Issues](#known-issues)
- [Resources and References](#resources-and-References)

---

## About the Project

This project is a console-based **Snake Game** where players control a snake, aiming to collect food while avoiding collisions with the walls and the snake's own body. The game implements object-oriented principles and focuses on efficient handling of player movement, collision detection, and dynamic food generation.

---

## Features
- Dynamic snake growth with every food consumed
- Randomized food generation, avoiding collisions 
- Win and lose conditions for a satisfying gameplay loop 
- Modular and clean C++ codebase for extensibility 
- Lightweight graphics using custom utility functions 

---

## How to Play
1. Use the following keys to control the snake:
   - **W**: Move Up
   - **A**: Move Left
   - **S**: Move Down
   - **D**: Move Right
2. Collect food (`=`) to grow the snake and increase your score.
3. Avoid colliding with the walls (`#`) or the snake’s body.
4. Press `/` to exit the game.

---

## Installation

### Prerequisites
- C++ compiler (GCC, Clang, MSVC)
- Make sure `MacUILib.h` and its implementation are included or replaced with compatible drawing libraries.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/snake-game.git
   ```
2. Navigate to the project directory:
   ```bash
   cd snake-game
   ```
3. Compile the project:
   ```bash
   g++ -o SnakeGame Project.cpp Player.cpp MacUILib.cpp GameMechs.cpp objPos.cpp objPosArrayList.cpp -std=c++17
   ```
4. Run the game:
   ```bash
   ./SnakeGame
   ```

---

## Code Architecture

### Core Components
- **GameMechs**: Handles game logic, score tracking, and food generation.
- **Player**: Manages the snake's movement and collision detection.
- **objPos & objPosArrayList**: Represents positions on the board and manages dynamic lists.
- **Project.cpp**: Main entry point, orchestrates game flow and rendering.

### File Structure
```
.
├── GameMechs.h/cpp      # Core game mechanics
├── objPos.h/cpp         # Position management
├── objPosArrayList.h/cpp # Dynamic array-based position lists
├── Player.h/cpp         # Player (snake) logic
├── Project.cpp          # Main entry point
```

---

## Future Enhancements
- Add difficulty levels (e.g., increasing speed over time).
- Implement a graphical interface using SDL or SFML.
- Introduce obstacles and power-ups.
- Add a high-score leaderboard.

---

## Acknowledgments
- Inspired by the classic arcade game Snake.

---

### Known Issues

- **Performance on Larger Boards:** The game may experience slowdowns on boards larger than 50x50 due to increased collision checks.
- **Input Responsiveness:** On certain systems, input detection might lag depending on the terminal environment.

---

### Resources and References

- [C++ Documentation](https://en.cppreference.com/)
- [Game Programming Patterns](http://gameprogrammingpatterns.com/)
- [MacUILib Library](https://github.com/username/MacUILib)
