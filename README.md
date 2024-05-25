# Guessing Game Project

## Overview

This project is a simple console-based guessing game implemented in Java. The game involves a `Guesser`, three `Players`, and an `Umpire` who manages the game. The objective is for the players to guess a number chosen by the guesser. The game determines the winner(s) based on the accuracy of the guesses.

## Classes and Functionality

### 1. Guesser
- **Attributes:**
  - `guessNum`: Stores the number guessed by the Guesser.
- **Methods:**
  - `guessNumber()`: Prompts the guesser to enter a number and returns it.

### 2. Player
- **Attributes:**
  - `pguessNum`: Stores the number guessed by the Player.
- **Methods:**
  - `guessNumber()`: Prompts the player to enter a number and returns it.

### 3. Umpire
- **Attributes:**
  - `numFromGuesser`: The number provided by the Guesser.
  - `numFromPlayer1`: The number guessed by Player 1.
  - `numFromPlayer2`: The number guessed by Player 2.
  - `numFromPlayer3`: The number guessed by Player 3.
- **Methods:**
  - `collectNumFromGuesser()`: Collects the number from the Guesser.
  - `collectNumFromPlayer()`: Collects the numbers from all three players.
  - `compare()`: Compares the numbers and declares the winner(s).

### Main Class: `Launchgame`
- This is the entry point of the application.
- **Workflow:**
  - Creates an instance of `Umpire`.
  - Collects the number from the Guesser.
  - Collects the numbers from all three players.
  - Compares the numbers and announces the result.

## How to Play

1. The `Guesser` chooses a number and enters it into the system.
2. Each of the three `Players` takes turns to guess the number.
3. The `Umpire` collects the numbers from both the `Guesser` and the `Players`.
4. The `Umpire` compares the guesses with the Guesser's number and announces the result:
   - If all players guess the number correctly, the game is tied.
   - If two players guess correctly, they win.
   - If one player guesses correctly, they win.
   - If none of the players guess correctly, the game is lost.

