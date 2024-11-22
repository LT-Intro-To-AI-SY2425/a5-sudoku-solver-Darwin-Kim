# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

Overall, the depth first search was more efficient. However, in a situation where the number of solutions can be lowered by checking different solutions against each other, the breadth first search could use data from previous searches to help it solve the puzzle.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

I am entirely unfamiliar with data structures, so I have literally no idea. I guess you could take a list and use it as a queue by popping the last value, or you could use it as a stack by popping the first value, or if you really wanted to you could just be a complete anarchist and pop values at random, which could be more effective in a large puzzle with a very large number of possible answers, as eventually the chances of randomly selecting the correct answer *MAY* outweigh the benefits of logical thought (Don't quote me on that, it could be completely absurd and absolutely objectively wrong).

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

This could be a good way to solve a very large tic-tac-toe board with smaller tic-tac-toe boards inside of it, since that seems very similar to solving a sudoku board, which can be solved in small segments similar to smaller boards inside a larger board

