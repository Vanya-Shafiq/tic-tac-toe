# Tic-Tac-Toe AI (Minimax Algorithm)
An AI-powered Tic-Tac-Toe game using the Minimax Algorithm for optimal decision-making. The AI analyzes all possible moves to either win or force a draw. Play against an intelligent opponent that predicts and counters your moves strategically. 

## Objective
This project implements an AI for Tic-Tac-Toe using the **Minimax Algorithm**. The AI ensures optimal gameplay by analyzing all possible moves and selecting the best strategy to either win or force a draw.

## Getting Started
1. **Download & Unzip**: Extract the project files from the provided distribution.
2. **Install Dependencies**:
   ```bash
   pip3 install -r requirements.txt
   ```
   This installs the required `pygame` package.
3. **Run the Game**:
   ```bash
   python runner.py
   ```
   This launches the graphical interface to play against the AI.

## Project Structure
- **tictactoe.py**: Contains the core game logic and AI implementation.
- **runner.py**: Provides a graphical interface for playing the game.

## Implementation Details
The following functions are implemented in `tictactoe.py`:

### 1. Game Mechanics
- `player(board)`: Determines whose turn it is (`X` or `O`).
- `actions(board)`: Returns all possible moves as `(row, col)` tuples.
- `result(board, action)`: Returns the new board state after applying a move.
- `winner(board)`: Checks if there is a winner (`X` or `O`).
- `terminal(board)`: Determines if the game is over.
- `utility(board)`: Returns `1` if X wins, `-1` if O wins, or `0` for a tie.

### 2. Minimax AI
- `minimax(board)`: Implements the Minimax algorithm to choose the best move for the current player, ensuring optimal play.

## Notes
- The AI uses a **recursive Minimax algorithm** to evaluate future board states.
- The original board is not modified directly; deep copies are used for accurate simulations.
- Helper functions may be added, as long as they do not conflict with existing function names.
