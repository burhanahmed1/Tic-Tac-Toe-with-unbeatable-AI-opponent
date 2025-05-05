
# Tic Tac Toe AI Player

A Python implementation of Tic Tac Toe featuring an unbeatable AI opponent using the minimax algorithm with alpha-beta pruning. Play against an AI that optimally determines the best move to ensure it never loses!

## Features

- **Human vs. AI Gameplay**: Play as X or O against the AI.
- **Optimal AI Moves**: AI leverages the minimax algorithm with alpha-beta pruning for efficient decision-making.
- **Terminal-Based Interface**: Simple command-line interface for gameplay.
- **Win/Tie Detection**: Automatically detects game outcomes (win for X/O or tie).
- **Input Validation**: Handles invalid moves gracefully.

## Installation

**Clone the repository**:
```bash
git clone https://github.com/burhanahmed1/Tic-Tac-Toe-with-unbeatable-AI-opponent.git
cd Tic-Tac-Toe-with-unbeatable-AI-opponent
```


## Usage

- **Start the game**: Execute the script and choose your player (X or O). X moves first.
- **Make a move**: Enter row and column numbers (0-2) when prompted.
- **AI Turn**: Watch the AI instantly calculate and execute its optimal move.

**Example**:
```
Choose a player (X or O)
X
Enter the position to move (row, col) [0-2] for each:
Row: 1
Col: 1
[None, None, None]
[None, 'X', None]
[None, None, None]

AI is thinking...
['O', None, None]
[None, 'X', None]
[None, None, None]
```

## Code Overview

### Key Functions
- `initial_state()`: Returns an empty 3x3 board.
- `player(board)`: Determines which player's turn it is.
- `actions(board)`: Returns set of valid moves.
- `result(board, action)`: Applies a move to the board.
- `winner(board)`: Checks for a winner (X/O) or returns `None`.
- `terminal(board)`: Checks if the game is over.
- `utility(board)`: Returns 1 (X wins), -1 (O wins), or 0 (tie).
- `minimax(board)`: Uses alpha-beta pruning to return the optimal AI move.

### Algorithm: Minimax with Alpha-Beta Pruning
- **Minimax**: Recursively evaluates all possible moves to maximize the AI's chances of winning while minimizing the opponent's opportunities.
- **Alpha-Beta Pruning**: Optimizes minimax by pruning branches that cannot influence the final decision, reducing computation time.

## Contributing

Contributions are welcome! Open an issue or submit a pull request for improvements or bug fixes.

## License

Distributed under the Apache 2.0 License. See `LICENSE` for details.

```
