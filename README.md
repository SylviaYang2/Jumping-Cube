# Jumping-Cube

The KJumpingCube game is a two-person board game implemented in Java, with **Minimax** and **Alpha-Beta-Pruning** Algorithm. It is a pure strategy game, involving no element of chance. allowing a user to play against an AI or against another person, or to allow the computer to play itself.

Implemented a GUI interface for the game. Incorporated randomness and user interaction by allowing the users to enter seeds and choose to play manually or using an AI against the opponent.

## Rules
The game board consists of an N×N array of squares, where N>1. At any time, each square may have one of three colors: red, blue, or white (neutral), and some number of spots (as on dice). Initially, all squares are white and have one spot.

For purposes of naming squares in this description, we'll use the following notation: r:c refers to the square at row r and column c, where 1≤r,c≤N. Rows are numbered from top to bottom (top row is row 1) and columns are numbered from the left. When entering commands, we replace the colon with a space (this being easier to type).

The neighbors of a square are the horizontally and vertically adjacent squares (diagonally adjacent squares are not neighbors). We say that a square is _**overfull**_ if it contains more spots than it has neighbors. Thus, the four corner squares are overfull when they have more than two spots; other squares on the edge are overfull with more than three spots; and all others are overfull with more than four spots.

There are two players, whom we'll call Red and Blue. The players each move in turn, with Red going first. A move consists of adding one spot on any square that does not have the opponent's color (so Red may add a spot to either a red or white square). A spot placed on any square colors that square with the player's color.

## Example
For example, given the board on the top (N=4) in Figure 2, if Red adds a spot to square 2:1, we get the board on the bottom after all the spots stop jumping.

![image](https://user-images.githubusercontent.com/83314726/184467203-2b08054f-b445-42de-b6c7-c944d4f70c26.png)
![image](https://user-images.githubusercontent.com/83314726/184467224-f0b5e74e-a805-4715-a5a4-954627eab562.png)
(Square 2:2 becomes overfull after we add a spot to square 2:1 and perform the first jump, so we must jump again for square 2:2.)

For example, if, on Red's move, the board is as on the top of Figure 3 and Red moves to 3:1, then the board will turn entirely red. You are allowed to stop the process of redistributing spots when all squares are red, even though, depending on the order in which you do things, you could end up with the board on the bottom in the figure.

![image](https://user-images.githubusercontent.com/83314726/184467304-60639c1a-1727-4f0e-b608-4fdcb997bbdd.png)
![image](https://user-images.githubusercontent.com/83314726/184467321-65192932-2e0d-4640-bfb5-f4e3deebf50f.png)

(The board on the top shows a position just before Red's last move (to 3:1). The board on the bottom is one possible stopping point for spot redistribution (all squares now being one color), even though the squares at 1:3 and 4:1 are still overfull.)


