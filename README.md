# 2DSliderGame
It's a 2d Slider Puzzle Game for the Terminal/CMD designed in C language.

Gameplay:
Numbers (1 to 15) are shown randomly on a 4*4 grid. The objective of the game is to rearrange the numbers in ascending order (1,2,3...).
You have to use W/A/S/D to move the blank place along the grid. 


Code: 

The structure "Blocks" will hold x,y coordinates and value of each position of the grid (16). 
At the start of the program, an array num[15] is declared. 
Then Num gets filled with random numbers. 

Then a function isSolvable() check whether by using the random numbers a slider puzzle would be solvable. (Check Wikipedia for the algorithm)

If the Game is Solvable, the values from the num array are assigned in the Struct pieces. And gameplay starts.
Else num array is reassigned and checked again with isSolvable().

Then by calling assignXY() function initial x,y coordinates are stored into the STructure Blocks "pieces".

gameplay() : This function takes the inputs (W/A/S/D) and then Swaps the blank space with appropriate value.
swaps. The player is inside this function until win() function retuns as true.

The visuals are updated by the display() function.





