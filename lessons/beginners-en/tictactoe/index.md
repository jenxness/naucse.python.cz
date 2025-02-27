# One-dimensional tic-tac-toe

You plan your 1D tic-tac-toe on a board that has one row with 20 spaces.

There are two players.
The first player makes a move by placing an `x` into an empty space.
The second player places an `o`. Then the first player plays again.

For example:
1. move: `-------x------------`
2. move: `-------x--o---------`
3. move: `-------xx-o---------`
4. move: `-------xxoo---------`
5. move: `------xxxoo---------`
   
The player who places three of their own marks next to each other wins.

Your task is to program the game!

## Step 1

Write a function `evaluate` that accepts the string with the board of 1D tic-tac-toe as argument 
and returns one character based on the state of the game:

- `"x"` – The player who uses crosses (Xs) has won (the board contains `xxx`)
- `"o"` – The player who uses noughts (Os) has won (the board contains `ooo`)
- `"!"` – Draw (the board is full but nobody has won)
- `"-"` – Rest (i.e. the game is not finished)

## Step 2

Write a `move` function that accepts the string with the game board, a position number (0-19)
and a (x or o) mark and returns a game board (i.e., a string with the given mark placed in the given position).
The function header could look something like this:

```python
def move(board, mark, position):
    # Returns the game board with the given mark in the given position.
    ...
```

## Step 3

Write a `player_move` function that accepts a string with the game board, asks the player 
which position he wants to play
and returns the updated game board with the player's move. The function should reject 
negative or too large numbers or moves to an occupied position. If the user has entered
a wrong argument, the function should ask again (to get correct answer).

## Step 4

Write a `pc_move` function that accepts the string with the game board.
It will select a position to play, and returns
the game board with the computer's move.<br>
Use a simple random "strategy":
* Select a random number from 0 to 19.
* If the position is empty, place the computer's mark there.
* If not, repeat from the first step (select another random number).
The function header should look something like this:

```python
def pc_move(board):
    # Returns a game board with the computer's move.
    ...
```


## Step 5

Write a `1D_tictactoe` function that creates a string with a game board and alternately calls the `player_move` and
`pc_move` functions until someone wins or draws.
Do not forget to check the status of the game after every turn.

## Step 6 - Optional
Can you think of better strategy for your computer? 
Let us know your ideas or try to program them directly.
