What is Brute Force Algorithm? Brute Force Algorithms are exactly what they sound like – straightforward methods of solving a problem that
rely on sheer computing power and trying every possibility rather than advanced techniques to improve efficiency. For example, imagine you
have a small padlock with 4 digits.

Problem Facing: Brute Force Algorithm is easy to implement code are easily available. But the comparison one algorithms code not available so
the problem will be there on comparison.

Conclusion: Brute force search is the most common search algorithm as it does not require any domain knowledge, all that is required is a state
description, legal operators, the initial state and the description of a goal state. It does not improve the performance and completely relies on
the computing power to try out possible combinations.

Brute force algorithm :
Basic idea:
 The basic idea of the brute force algorithm is to place the queens on all possible 
positions and check each time if the queens cannot capture each other. 
If not then it has found a solution. Because of the vast amount of possible positions 
(NN for a table of size N while each row has 1 queen), this algorithm is not practical
 even for small table sizes (like N=12).

Advantages over other methods:
Probably none. The brute force algorithm is only mentioned to point out the superiority 
of the other algorithms, as a brute force approach is the last resort, when every other
 attempt failed.

Other thoughts:
 
But after "forcing" the algorithm to place only one queen on each row and one on 
each column the number of posible valid positions decreases to N! (N!=1*2*3....*(N-1)*N).
Using this algorithm we can found a solution for larger table sizes compared to the 
previous method (like N=17).
