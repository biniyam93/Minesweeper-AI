# Minesweeper AI

## Description:

Welcome to the Minesweeper AI project, where you'll find an implementation of an AI player to play Minesweeper optimally. This project contains logic to handle gameplay, infer moves based on knowledge, and provide an interface to play the game with or without the AI.

## Project Overview:

* `runner.py`: This Python script contains the code to run the graphical interface for the Minesweeper game. It allows users to interact with the game board visually.
* `minesweeper.py`: This file contains the core logic for the Minesweeper game and the implementation of the MinesweeperAI class. It includes the Minesweeper class, Sentence class, and MinesweeperAI class, each handling different aspects of the game and AI behavior.

## Features:

### 1. Minesweeper Class
   * Handles the gameplay, including board initialization, cell revealing, and game state management.

### 2. Sentence Class
   * Represents logical sentences containing a set of cells and a count of mines within those cells.
   * Provides functions for identifying known mines and known safe cells within the sentence.
   * Includes methods to update the sentence when a cell is marked as a mine or safe.

### 3. MinesweeperAI Class
   * Implements an AI player to make optimal moves in the Minesweeper game.
   * Keeps track of cells already clicked, known mines, known safe cells, and logical sentences inferred from gameplay.
   * Includes functions to add knowledge, make safe moves, and make random moves.

## How to Use:

1. **Run the Script**: Execute the `runner.py` script in a Python environment to launch the graphical interface for the Minesweeper game.

2. **Interact with the Game**: Use the graphical interface to play Minesweeper either manually or let the AI play for you.

3. **AI Gameplay**:
    * The AI will analyze the game state and make optimal moves based on the information available.
    * It will update its knowledge base and make deductions to uncover safe cells and mark mines accurately.

## Design Choices:

**Modular Structure**: The project is organized into separate classes for different components of the Minesweeper game and AI player. This modular design enhances readability, maintainability, and extensibility of the codebase.

**Knowledge Representation**: The AI maintains a knowledge base consisting of logical sentences inferred from the game board. These sentences help the AI make informed decisions about where to click next and where mines are likely to be located.

**Optimal Decision Making**: The AI employs strategies to uncover safe cells and mark mines efficiently, ensuring optimal gameplay and maximizing the chances of winning the game.

