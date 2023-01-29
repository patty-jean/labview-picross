# LabVIEW Picross ![big fish border](https://user-images.githubusercontent.com/84546784/215360814-528d2256-0501-4950-9d60-008afcb80ceb.png)
### A LabVIEW VI that allows the player to play a 10x10 game of picross.<br />



The following is a brief description of how this works: <br />
This works by using 100 2D pictures that the user can click on to change the appearance and value.
The back panel of the VI has a 2D boolean array the same size as the 2D picture array that serves as the reference for the answer.
The 2D picture array is constantly checked against the solution array to check if the user has solved the puzzle, and when they have, there is a popup and the VI stops.
Every time the VI starts, it wipes the board clean and autocalculates the values on the top and left of the board and prints them there.
picross-complete.vi is the full program, and it is reliant on 'Untitled 5 (SubVI).vi' for the 2D pictures to work.<br />



The following gif shows the behavior of the front panel at the start of a game and when it is reset:<br />
![board-reset](https://user-images.githubusercontent.com/84546784/215360413-c8080a0f-ce3d-4fa8-9f87-880b24733e97.gif)<br />

The following gif shows what happens when the user completes the puzzle:<br />
![complete](https://user-images.githubusercontent.com/84546784/215360439-a5b5f737-c1c5-4da4-bc7c-9ebcabdf2c8b.gif)<br />

The following is the back panel of picross-complete.vi:<br />
![image](https://user-images.githubusercontent.com/84546784/215360478-ffff1437-d378-45bc-9b3c-3af3bfaa0262.png)<br />
The back panel of this project consists of two main parts, and their 'delimiter' is the sequence structure.  Above the sequence structure is the chunk of code that takes in user input and checks if the puzzle is solved.  Inside the sequence structure, the first frame wipes the board clear of numbers and user input.  The second frame is the chunk of code that calculates what numbers should be on the top and left of the puzzle, formats them, and displays them there.<br />

The following are different conditions of case structures in the above back panel:<br />
![image](https://user-images.githubusercontent.com/84546784/215360498-67aff135-9d0a-4a4c-811e-d013b5a649af.png)<br />
![image](https://user-images.githubusercontent.com/84546784/215360501-3431df27-98c0-451e-bf3e-d17c982a1dee.png)<br />
![image](https://user-images.githubusercontent.com/84546784/215360505-f482ac16-21d4-4463-b55a-8c0581508bea.png)<br />
![image](https://user-images.githubusercontent.com/84546784/215360509-c2216145-18e0-4d20-86bc-5e371e9ff785.png)<br />


Next, the following is the back panel of "Untitled 5 (SubVI).vi"<br />

On each 2D picture, the player can left click to mark it correct, right click to mark it wrong, and middle click to make it neutral.<br />

Neutral button state:<br />
![image](https://user-images.githubusercontent.com/84546784/215360551-3274dcaf-2ad0-48f9-a267-55f6c601773f.png)

Selected as correct button state:<br />
![image](https://user-images.githubusercontent.com/84546784/215360553-4547deb5-fb6c-45ab-bdc0-c501709a960c.png)

Selected as incorrect button state:<br />
![image](https://user-images.githubusercontent.com/84546784/215360555-7f2eb70d-dbd7-448e-aee7-3465ea882791.png)
<br />
(The alternative name for this project is Fishcross, as the puzzle solution I made for this resembles, of course, a fish.)
