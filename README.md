# Sudoku-Solver

This Python project implements a Sudoku solver capable of solving classic 9-by-9 Sudoku puzzles. The objective is to fill empty cells with digits 1 through 9 in such a way that each row, column, and 3-by-3 box contains all of the digits from 1 to 9 without repetition.

## Features
Backtracking Search: The solver uses backtracking search algorithm to systematically explore all possible solutions, backtracking when it encounters an invalid state.

Minimum Remaining Values (MRV): It employs the MRV heuristic to choose the variable (cell) that is most constrained (i.e., has the fewest legal values remaining) to assign a value.

Degree Heuristic: Among variables with the same MRV, the solver selects the one with the maximum number of constraints on remaining variables. This helps in making informed decisions during the search.

Least Constraining Value: When selecting a value for a variable, the solver prefers the value that rules out the fewest choices for the neighboring variables. This heuristic helps in selecting values that are likely to lead to successful solutions.

AC3 Algorithm for Domain Reduction: Before starting the search, the solver uses the AC3 algorithm to reduce the domain of variables by removing values that are inconsistent with the constraints.

## Usage
To use the Sudoku solver, follow these steps:

Clone the Repository: git clone https://github.com/usmannazeer72/Sudoku-Solver
Run this code on Google Colab.

## Contributing
Contributions to improve the solver or add new features are welcome. If you want to contribute, feel free to fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. You can find more details in the LICENSE file.
