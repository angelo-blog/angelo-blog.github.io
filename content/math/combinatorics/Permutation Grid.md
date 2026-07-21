---
title: "The Permutation Grid" 
date: 2026-06-22
draft: false
---

## Weekly puzzles

*Hurray! this is the first in a series of math puzzles that I will writing about in the course of the next few months before I go to college.*
*Hopefully, the procrastination monster doesn't get me.*

### Puzzle 1

### Puzzle Statement
 
Consider a $2025 \times 2025$ grid with the rows numbered  $1$ to $2025$ from top to bottom and columns numbered 1 to 2025 from left to right. Each cell of the grid is assigned a number between 1 and 2025 such that the following two conditions hold :

i)  for a given row/ column, all the number in said row/ column are all distinct. 

ii) the number are symmetric along one of the main diagonals, more formally $a_{i,j} = a_{j,i}$ for all pairs $(i , j)$.

Prove that no two cells in the main diagonal are equal i.e every pair cells $(i,i)$ ,  $(j,j)$ s.t $i \neq j$ we have that $a_{i,i} \neq a_{j,j}$. 

*I'm too lazy to figure out how to hide solutions in drop downs, so **STOP** reading from this point and draw some examples*

### Solution

***Difficulty*** : Easy.

***Hint*** : Try constructing a grid that satisfies the first two conditions but not the statement you need to prove for a $5 \times 5$ grid. What obstacle do you face ? 

The above hint is essentially the key insight you need to solve the problem. Like most *easy* puzzles all you need to do is just look at small cases to figure it out, and this puzzle is no different. 

Firstly, it's not hard to see that we will have $2025$ instances of each number from $1$ to $2025$ in the grid as a result of condition i). You can easily prove this by considering what happens when place a number in some cell $(r,c)$, we have that the number of rows and number of columns that you can place the said number  decreases by one for each placement  and since  there are a total of $2025$ rows and $2025$ columns, we have exactly 2025 instances of each number. 

Next, consider what condition two implies : the instances of a number can be grouped into **PAIRS**. However, we have $2025$ instances for each number which is odd therefore there is exactly one instance which will lack a pair and therefore this instance will have to lie in the main diagonal. 


