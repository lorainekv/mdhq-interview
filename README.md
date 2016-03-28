Install test dependencies from root directory:  
`gem bundle install`
`bundle`

# Ruby Factorial
- Use `rspec` from the /factorials directory to view tests

# C Factorial
- Compile with `cc factorial.c`
- Run `./a.out`

# Sudoku
- Use `rspec` from the /sudoku directory to run tests


Currently, solve.rb loads the CSV into a hash map for processing, following the following coordinates:
![sudoku grid map](https://github.com/lorainekv/mdhq-interview/blob/master/sudoku/grid.jpg)

I didn't get as far as I wanted to with the sudoku exercise - I spent a bit too long working on the C factorial. 

- Idiosyncrasies: Cataloging all the grids in another hash for reference

1) Had I gotten further along in the implementation, my algorithm would have 
    - Checked cols for numbers 1 - 9, then suggested candidates based on missing number
    - Checked rows for numbers 1 - 9, then filled in the blanks based on suggested candidates 
    - Run the filled-out board through col, row, and grid validations
    - If all three validators are green, return completed board

2) Big O notation: It seems like the best case scenario would have been O(n), even with a completed input board, since all rows and cols would need to be validated. Worst case...hm. Maybe O(n^2) because it seems like it would be jumping back and forth between validation and filling out the blanks. 

3) I wanted to use hash tables so that I could easily lookup coordinates and access elements at a constant runtime. 

4) Time management. I spent too much time on the other portions of this homework, and found myself running out of time for sudoku! 
