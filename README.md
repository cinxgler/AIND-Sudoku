# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?

A: The main idea behind constraint propagation is to forbid certain values on some variables of the problem, this allows to fulfill the problems constraints. For this sudoku problem the boxes are the variables and the domain is the digits from 1 to 9, the constraint is to have one different digit in the box per unit. We are using constraint propagation with the naked twins by removing possible values from other boxes in the same unit of the naked twins, the values to remove are the digits that are already used by the naked twins.


# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?

A: When we add the diagonal rule we are adding a new unit that must be verified to determine if the problem is solved. This makes the algorithm restrict the possible values using eliminate, only_choice and nake_twins for a box using this additional constraint per box.

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