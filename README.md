# labview-picross
A LabVIEW VI that allows the player to play a 10x10 game of picross.

This works by using 100 2D pictures that the user can click on to change the appearance and value.
The back panel of the VI has a 2D boolean array the same size as the 2D picture array that serves as the reference for the answer.
The 2D picture array is constantly checked against the solution array to check if the user has solved the puzzle, and when they have, there is a popup and the VI stops.
Every time the VI starts, it wipes the board clean and autocalculates the values on the top and left of the board and prints them there.
