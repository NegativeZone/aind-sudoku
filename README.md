# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: The naked twins heuristic finds two peers with two matching values. Since those values can only exist in either of those two boxes, it eliminates those options from every other mutual peer. This allows for a more thorough elimination process than what is already provided for by the eliminate heuristic. This heuristic is applied over and over again until the puzzle cannot be reduced any further or is solved.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: The two diagonals (top left to bottom right, and top right to bottom left) are just an additional unit for the solution to handle. Aside from the definition of the diagonals as additional units, the solution follows the same propagation of the eliminate, naked twins, and only choice constraints (with the depth first search as needed) to reduce the puzzle to the solution.
