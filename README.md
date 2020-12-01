#DAA 109 Fall 2020: Course Repository#
###PROJECT MEMBERS###
61869 | Wajahat Ali Khalid
61870 | Afroz Alam
61913 | Faizan Sidd
------------ | -------------
**61869** | **Wajahat Ali Khalid**
61870 | Afroz Alam
61913 | Faizan Sidd


## Description ##
This repository contains assignments and project submitted to DAA course offered in Fall 2020 at PafKiet.

## DYNAMIC PROGRAMMING ##

Dynamic Programming underscore more in enhancement as opposed to outright recursion. Recursive arrangement normally has continous call precisely comparative sources of info consequently at whatever point we see them we need to enhance is by applying Dynamic Programming 

We need to utilize Dynamic programming answer for taking care of this n-sovereign issue. In n sovereign issue the n sovereigns are to be put in the chess in way that no sovereign danger other sovereign. The sovereign assault evenly, vertically and askew in this way new sovereign should be put in a position which isn't undermined by recently positioned sovereigns. 

This issue is comprehended by basic O(f(n)8^n) arrangement which depends on unique programming In which f(n) is a low request polynomial which is demonstrated to be first non paltry upper headed for the issue. 

One of the principle bit of leeway of dynamic writing computer programs is its cycle separates any difficult that is mind boggling and convert it into interrelated arrangement for some sub issues it generally gives the knowledge to the issues nature AND it is done.

## What is backtracking?

Backtracking is finding the solution of a problem whereby the solution depends on the previous steps taken. For example, in a maze problem, the solution depends on all the steps you take one-by-one. If any of those steps is wrong, then it will not lead us to the solution. In a maze problem, we first choose a path and continue moving along it. But once we understand that the particular path is incorrect, then we just come back and change it. This is what backtracking basically is.
In backtracking, we first take a step and then we see if this step taken is correct or not i.e., whether it will give a correct answer or not. And if it doesn’t, then we just come back and change our first step. In general, this is accomplished by recursion. Thus, in backtracking, we first start with a partial sub-solution of the problem (which may or may not lead us to the solution) and then check if we can proceed further with this sub-solution or not. If not, then we just come back and change it.
Thus, the general steps of backtracking are:
•	start with a sub-solution
•	check if this sub-solution will lead to the solution or not
•	If not, then come back and change the sub-solution and continue again
N queens on NxN chessboard
________________________________________
One of the most common examples of the backtracking is to arrange N queens on an NxN chessboard such that no queen can strike down any other queen. A queen can attack horizontally, vertically, or diagonally. The solution to this problem is also attempted in a similar way. We first place the first queen anywhere arbitrarily and then place the next queen in any of the safe places. We continue this process until the number of unplaced queens becomes zero (a solution is found) or no safe place is left. If no safe place is left, then we change the position of the previously placed queen.
Explanation of the code
________________________________________
is_attack(int i,int j) →  This is a function to check if the cell (i,j) is under attack by any other queen or not. We are just checking if there is any other queen in the row ‘i’ or column ‘j’. Then we are checking if there is any queen on the diagonal cells of the cell (i,j) or not. Any cell (k,l) will be diagonal to the cell (i,j) if k+l is equal to i+j or k-l is equal to i-j.
N_queen → This is the function where we are really implementing the backtracking algorithm.
if(n==0) → If there is no queen left, it means all queens are placed and we have got a solution.
if((!is_attack(i,j)) && (board[i][j]!=1)) → We are just checking if the cell is available to place a queen or not. is_attack function will check if the cell is under attack by any other queen and board[i][j]!=1 is making sure that the cell is vacant. If these conditions are met then we can put a queen in the cell – board[i][j] = 1.
if(N_queen(n-1)==1) → Now, we are calling the function again to place the remaining queens and this is where we are doing backtracking. If this function (for placing the remaining queen) is not true, then we are just changing our current move – board[i][j] = 0 and the loop will place the queen on some another position this time.


## Brute force algorithm :

## Basic idea:
 The basic idea of the brute force algorithm is to place the queens on all possible 
positions and check each time if the queens cannot capture each other. 
If not then it has found a solution. Because of the vast amount of possible positions 
(NN for a table of size N while each row has 1 queen), this algorithm is not practical
 even for small table sizes (like N=12).

## Advantages over other methods:
Probably none. The brute force algorithm is only mentioned to point out the superiority 
of the other algorithms, as a brute force approach is the last resort, when every other
 attempt failed.

## Other thoughts:
 
But after "forcing" the algorithm to place only one queen on each row and one on 
each column the number of posible valid positions decreases to N! (N!=1*2*3....*(N-1)*N).
Using this algorithm we can found a solution for larger table sizes compared to the 
previous method (like N=17).

## Backtracking algorithms :

 Backtracking algo are applicable for NP-Complete problems. Priestley and Ward 
presented the details about the backtracking and its applications. They have clearly explained
 the preliminaries of the algorithm and gave a clear picture of the 8-queen puzzle. 
The solution for the problem could be achieved through tree structure representation of the
 choices. The proposed procedure could reduce the number of test cases to a sum of 15,720.
 The time complexity was reduced by reducing test cases. Pre –analysis was used to reduce 
the test cases. They used bush pruning technique for further improvement. Finally hybrid
 approach of pre-analysis and bust pruning gave better result. Ginsberg introduced dynamic
 backtracking algorithm but that does not solve constraint satisfaction problem dynamically. 
Gerald and Thomas proposed some alteration to support a dynamic constraint satisfaction.
 But this method suffers due to heavy time complexities. Lijo V. P. et al, / (IJCSIT) 
International Journal of Computer Science and Information Technologies, M M Noori and 
B T Razaie expose and implemented an improved backtracking algorithm for identifying 
t-designs which is proposed by J. Combin. Des. According to Noori, the algorithm uses a
 systematic method to derive new useful equations from the initial equations which are useful
 in speeding up the classical backtracking algorithm. The reader can refer to get brief 
description of backtracking algorithms and their applications. Bessière et al. proposed a 
asynchronous backtracking algorithm for distributed constraint satisfaction problems. 
This is based on distributed backtracking with storage of the previous results to reduce 
the total number of trials. M.A. Gutierrez-Naranjo et al. presented the N-queen problem 
in conjunctive normal form. They described the queen problem as a SAT problem by 
assuming the each Psystems send truth values as Yes or No. Pioneer solution have 
presented to the N-queens puzzle based on Membrane Computing. Algorithm 1 gives 
an insight on back tracking algorithm which is based on depth-first recursive search.

## Backtracking-Algorithm :

Backtracking general algorithm 
Checks whether solution has been found 
If found solution, return it 
else for each choice that can be made 
take that choice
Recurrence 
If recursion gives a positive result, return it
          If no choices remain, return failure


