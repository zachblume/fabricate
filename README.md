# fabricate

A prompting and testing framework and compiler that makes use of OpenAI's codex to build a NextJS-based web application while you write.

## Examples

### A tick-tack-toe game
```fabricate
Homepage
  A game of tick-tack-toe UI that stores the state of the game in a json file as a database
  Checks on every render for a winner and displays a message if there is one
  The winner message is displayed in a modal and should be "X wins!" or "O wins!" or "Draw!"
  The nature of a win condition is that there are three pieces of the same type in a row either horizontally, vertically, or diagonally
  The game starts with an empty board
  The game ends when there is a winner or a draw
  The winner or draw modal should also have a reset button that resets the game

Components
  Board
  A 3x3 grid of squares

  Square
  A square that can be clicked on to place a piece of type X or O

  Piece
  A piece of type X or O

  X
  A piece of type X

  O
  A piece of type O

Tests
  The board is empty at the start of the game
  A board in the state of each of the possible win conditions should have a winner
  The game ends when there is a draw
  The board is unclickable after the game ends
  The board is clickable after the game ends once the user clicks the reset button
  The reset button results in an application state at every component indistinct from that of a new game
  The reset button results in a page screenshot-identical to that of a new game
```