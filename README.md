# cpp_sudoku
Sudoku is one of the most popular puzzle games of all time. The goal of Sudoku is to fill a 9×9 grid with numbers so that each row, column and 3×3 section contain all of the digits between 1 and 9. As a logic puzzle, Sudoku is also an excellent brain game. If you play Sudoku daily, you will soon start to see improvements in your concentration and overall brain power. Start a game now. 

## How to play Sudoku
The goal of Sudoku is to fill in a 9×9 grid with digits so that each column, row, and 3×3 section contain the numbers between 1 to 9. At the beginning of the game, the 9×9 grid will have some of the squares filled in. Your job is to use logic to fill in the missing digits and complete the grid. Don’t forget, a move is incorrect if:

## Sudoku Tips
Sudoku is a fun puzzle game once you get the hang of it. At the same time, learning to play Sudoku can be a bit intimidating for beginners. So, if you are a complete beginner, here are a few Sudoku tips that you can use to improve your Sudoku skills.

Tip 1: Look for rows, columns of 3×3 sections that contain 5 or more numbers. Work through the remaining empty cells, trying the numbers that have not been used. In many cases, you will find numbers that can only be placed in one position considering the other numbers that are already in its row, column, and 3×3 grid.

Tip 2: Break the grid up visually into 3 columns and 3 rows. Each large column will have 3, 3×3 grids and each row will have 3, 3×3 grids. Now, look for columns or grids that have 2 of the same number. Logically, there must be a 3rd copy of the same number in the only remaining 9-cell section. Look at each of the remaining 9 positions and see if you can find the location of the missing number.



## Follow the steps below to solve the problem:
1. Create a function that checks if the given matrix is valid sudoku or not. Keep Hashmap for the row, column and boxes. If any number has a frequency greater than 1 in the hashMap return false else return true;
2. Create a recursive function that takes a grid and the current row and column index.
3. Check some base cases. 
If the index is at the end of the matrix, i.e. i=N-1 and j=N then check if the grid is safe or not, if safe print the grid and return true else return false. 
The other base case is when the value of column is N, i.e j = N, then move to next row, i.e. i++ and j = 0.
4. If the current index is not assigned then fill the element from 1 to 9 and recur for all 9 cases with the index of next element, i.e. i, j+1. if the recursive call returns true then break the loop and return true.
5. If the current index is assigned then call the recursive function with the index of the next element, i.e. i, j+1
