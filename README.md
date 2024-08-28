# Sudoku Solver

This Java program solves Sudoku puzzles using a backtracking algorithm. Sudoku is a logic-based number placement puzzle where the goal is to fill a 9x9 grid so that each digit from 1 to 9 appears exactly once in each row, column, and 3x3 subgrid.

## Main Components and Functionality

### `display` Method

- Responsible for displaying the current state of the Sudoku board.
- Utilizes ANSI escape codes for terminal text coloration, making the output visually appealing.
- Prints each cell's value in either cyan or yellow, separated by vertical and horizontal lines for clarity.

### `solve` Method

- Implements the main recursive backtracking algorithm to solve the Sudoku puzzle.
- Takes the current board, row (i), and column (j) as parameters.
- Attempts to fill empty cells with valid numbers (1-9) and prints the solution if successful.
- Backtracks by resetting cell values to 0 when necessary and continues exploring other possibilities.

### `isValid` Method

- Checks whether placing a number (val) in a specific cell (x, y) is valid according to Sudoku rules.
- Validates that the number does not already exist in the same row, column, or 3x3 subgrid.

### `main` Method

- Initializes a 9x9 Sudoku board with a sample puzzle configuration.
- Optionally allows for input via the console using a `Scanner` (commented out section).
- Displays the initial board and calls the `solve` method to find a solution.
- Prints the solved board or a message indicating "No solution possible" if unsolvable.

## Usage

1. **Initialization**: Set up the Sudoku board with a starting configuration.
2. **Display**: View the board with color-coded output in the console.
3. **Solve**: Use the recursive algorithm to fill in the board and backtrack as needed.
4. **Validation**: Ensure all placements meet Sudoku rules.
5. **Results**: See the solved board or a message if no solution is found.

This code provides a functional Sudoku solver using recursive backtracking and offers a visually enhanced output through colored text.
