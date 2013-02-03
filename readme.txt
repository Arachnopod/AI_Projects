nns282, nona.sirakova@utexas.edu
ecp456, ethanp@utexas.edu

Partner names: 
Nona Sirakova
Ethan Petuchowski

__________________________________________________________________________________________________

Contribution of each team member to the work:
We did the first 5 questions using pair programming. 
For questions 6 and 7 we bounced heuristics ideas off each other. 
We each implemented our own ideas and compared the results. 
Question 8 used code which was largely already implemented, so Nona did question 8,
and Ethan dobule-checked that it is correct.

Throughout the assignment we contrived test cases, both together and separately. 
Also, each one of us tried to derive an admissibility proof for each heuristic he/she came up with, 
and we discussed the proofs as well as the results in order to decide which heuristic best suits 
our solution.

__________________________________________________________________________________________________


Brief description that includes the main ideas of your implementation:

In order to implement BFS, DFS and A*, we consulted the pseudocode given in the book
for each of these algorithms.

The heuristics we used for questions 6 and 7 are as follows: 
Question 6 (Corners heuristic):
Finds the Manhattan distance between Pacman and the closest corner. 
From there finds the perimeter of the maze and subtracts the longest side from the perimeter.
Note: We subtract the longest side from the perimeter, because pacman will not make a full 
trail from corner1 to corner 1. It will travel at most along three out of the four sides of the
maze.

Question 7 (food heuristic): 
For each food x, find the distance to the food y, which is closest food to x. 
Add up all distances.
Subtract the smallest distance between two points. We do this, because given n points, if we just
add up the distances between each two neighbors, we consider the weight of n edges. 
In fact, if we are to travel a path from node 1 to node n, there are n-1 edges. 
Thus, without the subtraction we may be overcounting. With the subtraction, we are never overcounting

__________________________________________________________________________________________________

Running the code: We ran our code on Python 2.7
Our code compiles and runs with the commands and flags provided in the assignment.
__________________________________________________________________________________________________

