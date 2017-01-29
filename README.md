# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Naked twins technique sets some additional constraints on the peers of the boxes containing these naked twins.
   By setting additional constraints we reduce the search space and our sudoku solver works more efficiently.
   Constraints are set on peers the same way as we used in Eliminate technique, only if in Eliminate we had only one value for one box, in Naked Twins we have two values for two boxes, so we can remove these two values from the peers.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Constraints set by adding Diagonal unit enlarges peers space of the boxes on diagonal.
   Therefore we have additional constraints that may improve our Eliminate, Only Choice and Naked Twins techniques for the boxes on diagonal and in the end reduce the search space to find the solution.
   However the solution space is narrowed by these constraints.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
