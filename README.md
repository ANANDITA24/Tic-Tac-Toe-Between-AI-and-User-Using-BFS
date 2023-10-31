# Tic-Tac-Toe-Between-AI-and-User-Using-BFS
This is Tic Tac Toe game between AI and user using Breadth First search Approach (for AI move selection) using Python.

1. **Importing Required Libraries:**
   ```python
   import queue
   ```
   The code begins by importing the `queue` module. This module provides the `Queue` class, which is used to implement a queue data structure.

2. **Defining Functions:**
   The code defines several functions for various purposes:

   - `print_board(board)`: This function takes the game board as input and prints it in a user-friendly format, displaying the current state of the game.
   - `is_winner(board, player)`: It checks if the specified player has won the game by examining the rows, columns, and diagonals of the board.
   - `is_draw(board)`: This function checks if the game has ended in a draw by verifying if there are any empty spaces left on the board.
   - `is_valid_move(board, row, col)`: It checks if a move (specified by row and column) is a valid move within the game board.
   - `bfs_ai_move(board, player)`: This function uses the Breadth-First Search (BFS) algorithm to explore possible game states and determine the best move for the AI (Player O).

3. **Main Game Loop:**
   The `play_tic_tac_toe` function is the main game loop where the Tic Tac Toe game is played. It sets up the game board, defines the players ("X" and "O"), and initializes the current player as "X."

4. **Game Execution:**
   The game proceeds as follows:

   - The current state of the board is displayed using the `print_board` function.
   - Depending on the current player, the user is prompted to enter their move (row and column) for Player "X," or the AI (Player "O") determines its move.
   - For the AI's move, the code first calls the `bfs_ai_move` function to find a winning move using BFS. If a winning move is found, the AI selects that move. Otherwise, it makes a random move (0,0 by default).
   - The code checks if the chosen move is valid using `is_valid_move`. If the move is valid, it updates the game board with the player's move.
   - The code then checks for a win using `is_winner`, and if there is a winner, it prints a message and exits the game.
   - It also checks for a draw using `is_draw`, and if there's a draw, it prints a message and ends the game.
   - The current player is then updated, and the game proceeds with the next turn.

5. **Main Function:**
   Finally, the `if __name__ == "__main__":` block ensures that the `play_tic_tac_toe` function is executed when the Python script is run. This is where the game is initiated.


