# TIC TAC TOE
Goal: The system could be run in BOT mode to print on the screen all player's moves (with a 2 seconds timeout between each round) until someone won or the game ends with a draw.
## Test Cases
* Create the game board with no X's and O's
* Game board has 6 | , 6 - , 4 +
* The game starts with player X
* Generate a random x, y coordinate to make a move
* The game detects a winner
* The game prints the correct winner

## Technical Approach
* build out a 2x2 array to hold the game internally and detect a winner
* print out the modified string at each step
* loop while there is no winner

## Tech Debt (Refactored Code)
* Only use the string to print to the console. For the actual gameboard, store an internal 2D array.
* Track all strings representing each step in the game, in an array
* Simplify 2D array with an array of size 9. Each index represents a spot on the grid.
* Restructure printing of statements into separate parts instead of one large string. Made each string part dynamic.
* Instead of storing game in an array, simply track it in the gridMapping.