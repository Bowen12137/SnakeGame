
# Snake Game

A classic Snake game implemented in Java using Swing for the graphical user interface (GUI). The game follows the traditional Snake mechanics where the player controls the snake to consume apples and grow in length, while avoiding collisions with the borders or itself.

![Badge](https://img.shields.io/badge/version-1.0.0-blue) ![Badge](https://img.shields.io/badge/Java-8%2B-green)

## Table of Contents
- [Snake Game](#snake-game)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Features](#features)
  - [Game Mechanics](#game-mechanics)
  - [Project Structure](#project-structure)
    - [File Descriptions:](#file-descriptions)
  - [How to Play](#how-to-play)
  - [Installation](#installation)
    - [Step 1: Clone the Repository](#step-1-clone-the-repository)
    - [Step 2: Compile the Java Code](#step-2-compile-the-java-code)
  - [Running the Game](#running-the-game)
  - [Future Improvements](#future-improvements)
  - [Requirements](#requirements)
  - [License](#license)
  - [Contact \& Feedback](#contact--feedback)

## Overview

The **Snake Game** is a simple yet enjoyable arcade-style game where the player controls a snake that grows longer each time it consumes an apple. The snake can move in four directions (up, down, left, right), and the objective is to eat as many apples as possible without colliding with the game boundaries or its own body. The game ends when the snake collides with itself or a wall.

This game is built using Java Swing for GUI and has been structured with proper OOP principles, encapsulating the game mechanics in a clean and maintainable way.

## Features

- **Classic Snake Mechanics**: Control the snake using arrow keys and grow by consuming apples.
- **Randomized Apples**: Apples appear at random locations on the grid, encouraging movement and strategy.
- **Growing Snake**: The snake grows in length as it consumes apples.
- **Colorful Snake**: The snake’s body is colorful, with each part having a random color.
- **Game Over Detection**: The game ends when the snake hits the screen boundaries or itself.
- **Customizable Settings**: The game can easily be modified to change the grid size, game speed, or snake appearance.

## Game Mechanics

1. **Snake Movement**: The snake is controlled using the arrow keys (`UP`, `DOWN`, `LEFT`, `RIGHT`). The snake will move continuously in the last given direction until changed by the player.
   
2. **Apple Consumption**: When the snake's head overlaps with an apple, the snake's body grows by one unit and a new apple spawns at a random location.

3. **Collision Detection**: 
   - If the snake's head touches its own body or hits the boundary of the game window, the game ends.
   - A "Game Over" message is displayed when the snake collides with itself or the wall.

4. **Grid and Graphics**: The game is played on a grid, and the snake moves one unit at a time. The snake and apples are drawn using the `Graphics` class from Java's `java.awt` package.

## Project Structure

```
SnakeGame/
│
├── out/                             # Compiled class files (auto-generated)
│   └── production/
│       └── Snake/
│           ├── GameFrame.class
│           ├── GamePanel.class
│           ├── GamePanel$MyKeyAdapter.class
│           └── SnakeGame.class
│
├── src/                             # Source code directory
│   ├── GameFrame.java               # The JFrame that sets up the game window
│   ├── GamePanel.java               # Core game logic, rendering, and mechanics
│   └── SnakeGame.java               # Main class to start the game
│
├── LICENSE                          # Open source license for the project
├── README.md                        # Project documentation (this file)
└── Snake.iml                        # IntelliJ IDEA project configuration file
```

### File Descriptions:

1. **`GameFrame.java`**:
   - This class extends `JFrame` and sets up the window for the game. It contains basic settings like the title, size, close operation, and visibility settings. The `GamePanel` is added to the frame for game rendering.

2. **`GamePanel.java`**:
   - This is the core class that implements the game logic and rendering. It uses the `JPanel` class and overrides the `paintComponent` method to draw the game objects (snake, apple, grid). It also handles user inputs through a `KeyAdapter`, manages the game state (running or game over), and implements the game loop with a `Timer` for continuous movement.

3. **`SnakeGame.java`**:
   - The main class with the `main` method, which initializes the game by creating an instance of `GameFrame`. It acts as the entry point of the application.

## How to Play

1. **Objective**: Control the snake and eat as many apples as possible without colliding with the walls or yourself.
   
2. **Controls**:
   - **Arrow Keys**: Control the direction of the snake.
   - **Game Over**: The game ends when the snake hits the edge of the game screen or its own body.

3. **Winning**: There is no win condition in the classic Snake game — try to eat as many apples as possible and keep growing the snake!

## Installation

### Step 1: Clone the Repository

Clone the repository from GitHub using the following command:
```bash
git clone https://github.com/bowen12137/SnakeGame.git
```

### Step 2: Compile the Java Code

Navigate to the `src/` directory and compile the `.java` files using the following commands:
```bash
cd src
javac SnakeGame.java
```

This will compile the Java source files and output `.class` files in the `out/production/Snake/` directory.

## Running the Game

After compiling the code, run the game using the following command:
```bash
java SnakeGame
```

This will launch the game window where you can start playing.


## Future Improvements

Here are some potential enhancements to improve the game:

1. **Scoring System**: Display the score based on how many apples the snake has eaten.
2. **Levels of Difficulty**: Add multiple levels with increasing difficulty by adjusting the snake's speed.
3. **Obstacles**: Add stationary or moving obstacles that make the game more challenging.
4. **Power-ups**: Introduce power-ups that provide temporary abilities like increased speed or invincibility.
5. **High Score Tracking**: Implement a leaderboard that tracks the highest scores locally or in the cloud.

## Requirements

- **Java 8 or later**: You need to have the Java Development Kit (JDK) installed on your machine to compile and run the game.
- **Java Swing**: The game uses Swing, which is part of the standard Java library, so no additional dependencies are required.

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

## Contact & Feedback

We highly appreciate any feedback or suggestions for improving the game. If you encounter any issues or want to propose features, feel free to reach out.

✉️ **Email**: Arthur12137@gmai.com
