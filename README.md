# Sudoku Solver

A comprehensive Sudoku puzzle solver with both command-line and graphical user interfaces. This application can solve Sudoku puzzles of varying difficulty levels, generate new puzzles, and provide hints.

## Features

- **Solve Sudoku Puzzles**: Efficiently solves puzzles using a backtracking algorithm
- **Generate Puzzles**: Creates new puzzles with different difficulty levels (Easy, Medium, Hard)
- **Interactive GUI**: User-friendly interface with cell selection and keyboard input
- **Puzzle Validation**: Checks if a puzzle is valid and has a unique solution
- **Hint System**: Provides hints by filling in a random cell
- **Performance Metrics**: Shows solving time and number of steps
- **Sample Puzzles**: Includes pre-defined sample puzzles

## Screenshots

(Screenshots will appear when you run the application)

## Requirements

- Python 3.6 or higher
- Tkinter (included with most Python installations)

## Installation

No installation is required. Simply clone or download the repository and run the main script.

```bash
# Clone the repository (if you have git)
git clone https://github.com/yourusername/sudoku-solver.git
cd sudoku-solver

# Or just download and extract the files
```

## Usage

### Graphical User Interface (GUI)

To run the application with the graphical interface:

```bash
python main.py
```

### Command-Line Interface (CLI)

To run the application in command-line mode:

```bash
python main.py --cli
```

You can also specify the difficulty level:

```bash
python main.py --cli --difficulty easy
python main.py --cli --difficulty medium
python main.py --cli --difficulty hard
```

## How to Use the GUI

1. **Solving a Puzzle**:
   - Enter numbers in the cells by clicking on a cell and typing a number (1-9)
   - Click "Solve Puzzle" to solve the current puzzle

2. **Generating a Puzzle**:
   - Select a difficulty level from the dropdown menu
   - Click "Generate Puzzle" to create a new puzzle

3. **Other Functions**:
   - "Clear Board": Clears all cells
   - "Check Puzzle": Validates the current puzzle
   - "Load Sample": Loads a sample puzzle of the selected difficulty
   - "Get Hint": Fills in one cell as a hint

## How It Works

The Sudoku solver uses a backtracking algorithm to efficiently solve puzzles:

1. Find an empty cell
2. Try placing digits 1-9 in the cell
3. Check if the digit is valid in the current position
4. If valid, recursively try to fill the rest of the puzzle
5. If the recursive call returns false, backtrack and try a different digit

The puzzle generator works by:

1. Creating a fully solved Sudoku board
2. Removing numbers while ensuring the puzzle still has a unique solution
3. The number of cells removed depends on the difficulty level

## Project Structure

- `main.py`: Main entry point for the application
- `sudoku_solver.py`: Core solving and generation algorithms
- `sudoku_gui.py`: Graphical user interface implementation

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to all contributors and the Sudoku community
- Inspired by various Sudoku solving algorithms and techniques
