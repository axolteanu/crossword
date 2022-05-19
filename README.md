This repository contains source code for a web crossword presenter.

To use it, open the src/index.html in a browser and input a crossword data file.
The data file contains information about the location of all indexes and black squares on the grid as well as all the clues and the solution.

The data file must follow this format:

Line 1:  grid size.
Line 2: location of all black squares.
Line 3: location of all indexes.
Line 4: solution.

Line 1 is a single number representing the number of rows and columns.

For lines 2-4, imagine all rows are stringed together in order from left to right to form a single line.
For lines 2 and 3, all the numbers separated by dashes represent how many squares from left to right (starting at 0) to travel until the next clue or black square is encountered.
On line 4, '/' represents a black square.

All Across and Down clues follow. A clue should have the index number first followed by a space and the clue. All Across clues are preceded by ACROSS. All Down clues are preceded by DOWN.

A sample data file 'crossword-data.txt' is provided. 

This data comes from 'sample-crossword.pdf' which contains a crossword by Penny Dell taken from "https://www.arkadium.com/games/daily-crossword-pennydell/".
