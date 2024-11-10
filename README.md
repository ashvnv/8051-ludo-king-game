# Single Player vs 8051 Ludo King game

![GitHub](https://img.shields.io/github/license/ashvnv/8051-ludo-king-game)

Program is written in Assembly Language on Keil uVision and simulation was done on Proteus 8.15

## Proteus Schematic
<img src="https://raw.githubusercontent.com/ashvnv/8051-ludo-king-game/refs/heads/main/Pics/pic1.png?raw=true">

<img src="https://raw.githubusercontent.com/ashvnv/8051-ludo-king-game/refs/heads/main/Pics/pic2.gif?raw=true" width=500>

### Gameplay Overview:
This game is played between a single player (Red) and an automated opponent (Green), controlled by the 8051 microcontroller. The game follows most of the standard rules of Ludo.

When the simulation starts, the Red Player gets the first turn to roll the dice. The LCD screen displays **ROLL** followed by a series of changing characters, simulating the dice roll. The player must then press the **ON/C** button on the matrix keyboard to confirm the dice roll. Once the dice roll is completed and dice score is indicated on the LCD. 
If the player rolls a **6**, they are given an additional turn to roll the dice. Furthermore, they can choose which pawn to bring into play.
There are 4 pawns in total, indexed from 1 to 4. The player selects a pawn by pressing the corresponding index on the matrix keyboard.
The chosen pawn enters the game and is placed in the highlighted Red area (the player's starting area).
After selecting a pawn, if the player rolls a **6**, they get another chance to roll the dice and take another action (either move a pawn or bring out another pawn).
If the player rolls any other number, they move a pawn according to the number rolled.

### Green Player’s Turn
Once the Red Player’s turn is complete, the Green Player (automated by the 8051 microcontroller) takes its turn. The 8051 will automatically roll the dice and move its pawns according to the results.

### Winning the Game
The game ends when either the Red Player or the Green Player successfully parks all four of their pawns in their respective home area, after navigating the entire game board.

### Reset the game ###
To reset the game, click the **÷** key on the matrix keyboard.
