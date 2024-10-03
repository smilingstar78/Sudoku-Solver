# Sudoku Solver

This project implements a Sudoku puzzle solver using a backtracking algorithm. The program takes a partially completed Sudoku board as input and attempts to solve it by filling in the missing numbers while adhering to the rules of Sudoku.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Example](#example)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Sudoku is a logic-based number-placement puzzle. The goal is to fill a 9x9 grid with digits so that each column, each row, and each of the nine 3x3 subgrids contain all of the digits from 1 to 9.

This solver uses a **backtracking algorithm** to try and solve the puzzle by filling in missing digits step by step, validating each guess as it progresses. If a guess leads to a dead-end, it backtracks to try a different number.

## Features

- **Efficient Backtracking Algorithm**: Quickly solves even complex Sudoku puzzles.
- **Visual Board Representation**: Displays the puzzle in an easy-to-read format.
- **Validation of Puzzle**: Ensures that the board is solvable before displaying the solution.
- **Customizable Input**: Input any valid Sudoku board.

## Project Structure


## How It Works

### Board Class:
- **`find_empty_cell()`**: Finds the first empty cell (represented by 0) in the puzzle.
- **`valid_in_row()`, `valid_in_col()`, `valid_in_square()`**: Validates whether a number can be placed in a particular row, column, or 3x3 square.
- **`is_valid()`**: Ensures that the current number can be legally placed in the given cell by checking row, column, and square.
- **`solver()`**: The main backtracking function that attempts to solve the puzzle by trying numbers 1-9 in empty cells.
- **`__str__()`**: Converts the board into a readable string format, replacing zeros with `*` to represent empty spaces.

## Usage

### To use the solver:
1. Clone or download the repository.
2. Run the `solver.py` file in your terminal or Python environment.
3. You can input any valid 9x9 Sudoku puzzle in the form of a nested list (like in the `puzzle` variable).
4. The program will attempt to solve the puzzle and print the result.

```bash
python solver.py

Puzzle to solve:
* * 2 * * 8 * * *
* * * * * 3 7 6 2
4 3 * * * * 8 * *
* 5 * * 3 * * 9 *
* 4 * * * * * 2 6
* * * 4 6 7 * * *
* 8 6 7 * 4 * * *
* * * 5 1 9 * * 8
1 7 * * * 6 * * 5

Solved puzzle:
5 6 2 1 7 8 4 3 9
8 1 9 4 5 3 7 6 2
4 3 7 6 9 2 8 5 1
7 5 4 2 3 6 1 9 8
9 4 8 7 2 1 5 2 6
6 2 3 4 6 7 9 8 1
3 8 6 7 9 4 2 1 5
2 9 5 5 1 9 6 7 8
1 7 3 8 4 6 3 9 5
```
## Requirements
- Python 3.x
- No external libraries are required for this project.

## Contributing
- If you would like to contribute to the project, feel free to submit a pull request or create an issue. All contributions are welcome!

## 📫 How to Reach Me
- **Instagram**: [ai_enthusiast86](https://www.instagram.com/ai_enthusiast86)
- **LinkedIn**: [Muskan Tariq](https://www.linkedin.com/in/muskan-tariq-095a50282)
