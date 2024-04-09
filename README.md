# SudokuSolver.py - A Simple Sudoku Solver

## Overview

`SudokuSolver.py` is a Python script that solves a Sudoku puzzle using a backtracking algorithm. The script takes a 9x9 grid as input, with 0s representing empty cells.

## Detailed Description

The script contains two main functions:

- `solve_sudoku(grid)`: This function iterates over each cell in the grid. If it finds an empty cell (represented by 0), it attempts to place a number (1-9) in that cell. It checks if the number is valid for that cell using the `is_valid_move(grid, i, j, num)` function (not shown in the provided excerpt). If the number is valid, it places the number in the cell and recursively calls `solve_sudoku(grid)`. If the recursive call returns `True`, the function returns `True`. If not, it undoes the current cell (sets it back to 0) and continues with the next number. If no number can be placed in the current cell, the function returns `False` to trigger backtracking in the previous stack frame.

- `find_empty_cell(grid)`: This function finds the first empty cell in the grid. The implementation of this function is not shown in the provided excerpt.

## Installation

Python 3 is required to run this script. If you don't have Python installed, you can download it from [here](https://www.python.org/downloads/).

## Usage

To run the script, navigate to the directory containing `SudokuSolver.py` and run the following command in your terminal:

```bash
python SudokuSolver.py