<<<<<<< HEAD
# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: The first constraint is if only two digits in each box, so firstly finding these
   two-digits's boxes in each unit by coding "len_2 = [values[box] for box in unit if len(values[box]) == 2]".
   Then, the second constraint is if there are two completely same two-digits's boxes in one unit, by comparing the
   len(len_2) with the len(set(len_2)), we can easily know whether the twins exist and then get all the twins into twins.
   Last, the third constraint is the naked_twins being eliminated and so it makes constraint into other units.
   In the whole process, it is in a for loop, so every time it makes something constraint and then it propagates its
   constraints into next loop and do it again and again.


# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: A diagonal sudoku is like a regular sudoku, except that among the two main diagonals, the numbers 1 to 9 should all
   appear exactly once. So when the boxes are in diagonals, its peers should include the boxes in diagonals and then
   taking the method of eliminate(). Therefore, at the first beginning, finding the diagonal peers and adding them to the
   unitlist and reusing the method of solving a regular sudoku is just solving the problem.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solution.py` - Fill in the required functions in this file to complete the project.
* `test_solution.py` - You can test your solution by running `python -m unittest`.
* `PySudoku.py` - This is code for visualizing your solution.
* `visualize.py` - This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the `assign_value` function provided in solution.py

### Submission
Before submitting your solution to a reviewer, you are required to submit your project to Udacity's Project Assistant, which will provide some initial feedback.  

The setup is simple.  If you have not installed the client tool already, then you may do so with the command `pip install udacity-pa`.  

To submit your code to the project assistant, run `udacity submit` from within the top-level directory of this project.  You will be prompted for a username and password.  If you login using google or facebook, visit [this link](https://project-assistant.udacity.com/auth_tokens/jwt_login) for alternate login instructions.

This process will create a zipfile in your top-level directory named sudoku-<id>.zip.  This is the file that you should submit to the Udacity reviews system.

=======
# MyAINDSudokuProject
>>>>>>> fb52346d5dae2266b8d6ee1960929832de6bca33
