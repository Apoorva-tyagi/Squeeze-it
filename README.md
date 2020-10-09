**Project: Squeeze-it**

**Category: Game Playing, Intelligent Systems**

**Class Project**

**Game Overview:**

Squeeze-it is a two-player board game with a board size of 8x8. Each play initially has eight pieces placed on the uppermost and lowermost row. The initial configuration of the game looks like this:

![](https://github.com/Apoorva-tyagi/Squeeze-it/blob/main/gameboard.PNG)

**Programming Language:** Python

**System requirements:**

- Disk space: 1 GB.
- Operating systems: Windows\* 7 or later, macOS, and Linux.
- Python versions: 2.7.X, 3.6.X.

**Program file included: squeezeAI.py**

**Game Play:** Since it&#39;s a two-player game, match can either be played between AI-human or human-human. Each player can pick a piece from any valid location and place it on a blank position.

Pieces can be squeezed in two cases:

- If the opponent captures the pieces of another player in inward direction.
- If the opponent squeezes the pieces in outward direction.

If both cases are valid, then both the squeezes will take place.

**Installation Instructions:**

A Python IDE is required to run the program.

**Configuration Instructions:**

Each time a user turn takes place, program will ask the user for starting position and ending position. These positions are stored in tuple and will be input in this format: starting\_position\_coordinate1\&lt;space\&gt;ending\_position\_coordinate2

![](https://github.com/Apoorva-tyagi/Squeeze-it/blob/main/moves.PNG)

**Program Overview:**

**Movement Restrictions: Horizontal and vertical on Non-empty positions without crossing over the opponent.**

**Functions used:**

- **initialize()** : For initializing the game board with default values
- **print\_board():** For displaying the initialized board.
- **selectmove():** For capturing the move from the user.
- **make\_a\_move()** : For making a move from starting to ending position.
- **isvalid():** For checking the validity of each move of the opponent.
- **cross\_movement()** : For ensuring that a move doesn&#39;t do cross movement over another piece.
- **out\_horizontal\_squeeze()**: For checking outward horizontal squeeze pattern.
- **in\_horizontal\_squeeze():** For checking inward horizontal squeeze pattern.
- **horizontal\_checker():** For calling both the horizontal checkers.
- **out\_vertical\_squeeze():** For checking outward horizontal squeeze pattern.
- **in\_vertical\_squeeze():** For checking inward horizontal squeeze pattern
- **vertical\_checker():** For checking both the vertical checkers.
- **max\_pieces():** For calculating maximum number of pieces present on the board.
- **is\_game\_ended()** : For checking maximum pieces remaining and deciding if the game ended and who is the winner.
- **max\_r():** For calculating the starting position for AI which is at maximum risk.
- **min\_r():** For calculating the minimum position for AI which is at the minimum risk.
- **main():** Main function

**Validations are placed on the following cases:**

- If the input value is incorrect
- If the piece is placed on non-empty position.
- If the piece tries to move out of board boundary.
- If the piece tries diagonal movement
- Restricted Jump movement
- Left, Right, Up and Down range checker

**Game Ending conditions:**

- If all the moves are exhausted
- If the Player is eliminated
- In either case, Player with the maximum pieces on the board wins.

**Team Members:**

Apoorva Tyagi – aptyagi@ttu.edu

Vaidehi Pandya -- vaidehi.pandya@ttu.edu

Nitisha Patange -- nitisha.patange@ttu.edu
