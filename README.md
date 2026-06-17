# Reversi Game – Java OOP Project

## Overview

This project is an extended implementation of the strategic board game **Reversi**, developed in Java using Object-Oriented Programming principles.

The game is played on an 8x8 board and includes the standard Reversi mechanics, along with additional special disc types and AI-controlled players. The implementation focuses on clean game logic, legal move validation, turn management, disc flipping behavior, undo functionality, and integration with a graphical user interface.

This project was developed as part of an Object-Oriented Programming course and demonstrates practical use of inheritance, interfaces, encapsulation, polymorphism, and structured software design.

## Main Features

* Full Reversi game logic on an 8x8 board
* Legal move validation
* Turn management between two players
* Disc placement and opponent disc flipping
* Special disc types with custom behavior
* AI players with different move-selection strategies
* Undo functionality for human-player games
* Game reset support
* Compatibility with a provided graphical user interface

## Special Disc Types

The game supports several types of discs, each with different behavior:

### SimpleDisc

A regular disc that follows the standard Reversi rules.

### UnflippableDisc

A special disc that cannot be flipped once it is placed on the board.

### BombDisc

A special disc that, when flipped, can trigger additional flips of surrounding discs. This behavior may also activate nearby bomb discs, creating chain reactions.

## AI Players

The project includes AI-controlled players with different strategies:

### RandomAI

Selects a legal move randomly from the available options.

### GreedyAI

Chooses the move that flips the maximum number of opponent discs.

These AI players demonstrate how different decision-making strategies can be implemented using object-oriented design.

## Key Classes

### GameLogic

Implements the main game rules and manages the current game state, including the board, player turns, legal moves, disc placement, flipping logic, undo functionality, and reset behavior.

### PlayableLogic

An interface that defines the expected behavior of the game logic.

### Player

Represents a game player and stores player-related information.

### AIPlayer

An abstract base class for AI-controlled players.

### Disc

Represents a disc on the board and serves as the base abstraction for the different disc types.

### Position

Represents a position on the game board.

### Move

Represents a move in the game and supports tracking information needed for undo operations.

### Main

The entry point used to run the game.

## Game Rules

* The game starts with four discs placed in the center of the board.
* Players take turns placing discs on legal positions.
* A legal move must capture at least one opponent disc.
* Captured opponent discs are flipped according to the rules of the placed disc and the affected disc types.
* The game ends when no legal moves are available.
* The winner is the player with the highest number of discs on the board.

## Technologies Used

* Java
* Object-Oriented Programming
* Inheritance and Interfaces
* Game Logic
* AI Strategy Implementation
* GUI Integration

## What I Learned

This project strengthened my understanding of object-oriented design and helped me practice building a structured Java application with multiple interacting classes.

Through this project, I gained experience with:

* Designing class hierarchies
* Using interfaces and abstract classes
* Implementing complex game rules
* Handling edge cases in board-game logic
* Managing game state and undo operations
* Implementing simple AI strategies
* Writing clean and maintainable Java code

## How to Run

Open the project in a Java IDE such as IntelliJ IDEA or Eclipse, then run the `Main` class.

Make sure all required project files, including the GUI files, are included in the project structure.

## Future Improvements

Possible future improvements include:

* Adding a more advanced AI player
* Improving the graphical interface
* Adding score history and game statistics
* Supporting different board sizes
* Adding automated tests for the main game logic
