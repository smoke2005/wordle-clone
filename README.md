# Wordle Clone

## Project Overview

This Wordle clone is a word-based guessing game developed using the Pygame library, featuring five interactive windows: rules, menu, options, game board, and result. The game lets users select difficulty levels, enter guesses, and receive feedback on their guesses through colored indicators. The game includes easy, medium, and hard difficulty levels with word sets for each.

## Table of Contents
- [Aim](#aim)
- [Features Offered](#features-offered)
- [Libraries Used](#libraries-used)
- [Integration/Execution Sequence](#integrationexecution-sequence)
- [Files Used](#files-used)
- [Compilers Used](#compilers-used)

## Aim

The aim of this project is to create a Wordle clone using the Pygame library that consists of five windows:
1. **Rules** – Displays the game instructions.
2. **Menu** – Allows the user to play a new game or select the difficulty level.
3. **Options** – Lets the user choose a difficulty level.
4. **Game Board** – Where users can enter guesses.
5. **Result** – Displays the game result (win or lose).

This game uses Pygame's modules like display, mouse, draw, font, image, and event, along with the sleep function from the time module.

## Features Offered
- **Five Interactive Windows**:
  1. **Rules**: Shows the game instructions loaded from a text file.
  2. **Menu**: Offers options to start a new game, choose difficulty, or exit.
  3. **Options**: Allows the selection of difficulty level (easy, medium, hard).
  4. **Game Board**: Displays tiles for guessing and allows input through a virtual keyboard.
  5. **Result**: Displays the outcome of the game (win/loss).
  
- **Dynamic Word Selection**: Words are randomly selected from predefined text files based on the chosen difficulty level.
- **Feedback on Guesses**: Color-coded tiles (green, yellow, gray) to indicate correct, misplaced, or incorrect letters.

## Libraries Used
- **Pygame**: Used for the graphical interface, including handling display, mouse clicks, drawing, fonts, images, and events.
- **Time Module**: Used for the sleep function to control the game's flow and timing.

## Integration/Execution Sequence
1. **Rules Window**: Displays the rules by importing `Rules.txt`.
2. **Menu Window**: Allows the user to start a new game, choose options, or exit.
3. **Options Window**: Lets the user select the difficulty level by clicking on the easy, medium, or hard options.
4. **Game Board**: Displays the word tiles where the user enters guesses and shows feedback on the guesses.
5. **Result Window**: Displays whether the user has won or lost and offers options to play again or exit the game.

## Files Used
- **Text Files**:
  - `Easy.txt`: Contains words for the easy difficulty level.
  - `Medium.txt`: Contains words for the medium difficulty level.
  - `Hard.txt`: Contains words for the hard difficulty level.
  - `Rules.txt`: Contains the rules for the game, displayed in the rules window.

## User-Defined Functions
- **rules()**: Initializes the rules window, loads the rules from `Rules.txt`, and displays the continue button.
- **click_rules()**: Handles mouse hover and click events for the continue button in the rules window.
- **menu()**: Displays the menu window with options to start a new game, choose difficulty, or exit.
- **click_newgame()**: Handles mouse events for the new game, options, and exit buttons in the menu.
- **words()**: Displays difficulty options (easy, medium, hard).
- **word_click()**: Randomly selects a word from the respective difficulty file when a difficulty is chosen.
- **game_board()**: Displays the game board with word tiles.
- **add_letter()**: Renders and displays the entered letter in the corresponding tile.
- **colour()**: Provides feedback by coloring tiles based on the guessed letters.
- **indicator()**: Draws indicators (similar to a virtual keyboard) at the bottom of the screen.
- **indicator_color()**: Colors the indicators based on guessed letters' accuracy.
- **result()**: Displays the result of the game (win/lose) and provides options to play again or exit.
- **reset_button()**: Handles reset or exit after the result is displayed.
- **delete()**: Clears letters from the screen when necessary.
- **quit()**: Exits the Pygame window.

## Compilers Used
- Python 3.x with the Pygame library installed.
- IDEs like PyCharm, VS Code, or Jupyter Notebook for development.
