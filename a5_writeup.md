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

DFS is less effcient than BFS because it takes alot more iterations to solve the sudoku board. DFS is more likely to start off wrong which also makes it have to go through more iterations than BFS. Since BFS considers the neighbors first it's not suitable for decsion making trees in puzzes. BFS is more suitable for puzzles because its technique is more efficent.
Use BFS for searching vertices closer to given source while DFS is better for when the solution is away from the source.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The choice of using Stacks for DFS and Queues for BFS was for efficency. BFS is ale to scan through the scenrios and eliminate scenrios when needed while DFS scans through data all the way through. You can use an array, linked list, and deque. A deque is an ordered collection of items similiar  to the queue. An array is a linear data structure that collects elements of the same data type and stores in contingous memory location. A linked list is a collection of nodes that contain data. 


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

You would first have to extend the size of the board to be used for bigger boards.This can be adapted to to solve other logic puzzles when given a data set. We can use this to solve problems of sorting people into groups, sorting markets or goods.

