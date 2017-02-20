# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A:
* *Constraint propogation is a technique involving use of local constraints to reduce the problem complexity.*
* *In the case of Naked Twins we first get the **Naked Twins List** using the constraint of **value length two***
* *After that we form a **peerList** by constraining the list to **intersection of peer sets** of the naked twins*
* *In the end we traverse our obtained Lists and update the corresponding values again by constraining the **value of elements** to be updated have **length greater than two***
* *This reduces our search space to a great extent thus helping us solve the problem*

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: 
* *In the case of Diagonal Sudoku,we first get the list of **solved boxes** by constraining the **search space** to **only the diagonals** of the sudoku*
* *After getting the solved Diagonals List we traverse both the diagonals and remove the values in the solved boxes from the diagonal elements,here the local constraints are **length of values of elements** to be updated should be **>=2***
* *Thus both the diagonals are solved in the same manner and we can see that constraint propogation reduces our problem complexity to a great extent*
