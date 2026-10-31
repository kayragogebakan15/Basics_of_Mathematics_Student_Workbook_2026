# Exercise 3 — Inconsistent System

## 1. Problem Statement
Solve or show that the system is inconsistent:
$$\begin{cases}x+2y=3,\\2x+4y=7.\end{cases}$$
Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## 2. Method and Key Formula
Use Gaussian elimination on the augmented matrix. A row of the form $[0\quad0\mid c]$ with $c\ne0$ represents the impossible equation $0=c$, proving that no solution exists.

## 3. Detailed Step-by-Step Solution
The augmented matrix is
$$\left[\begin{array}{cc|c}1&2&3\\2&4&7\end{array}\right].$$
Apply $R_2\leftarrow R_2-2R_1$:
$$\left[\begin{array}{cc|c}1&2&3\\0&0&1\end{array}\right].$$
The second row represents
$$0x+0y=1\quad\Longleftrightarrow\quad 0=1,$$
which is a contradiction.

In equation form, the left-hand side of the second original equation is twice the first, so its right-hand side would also have to be $2\cdot3=6$. It is instead $7$.

## 4. Verification and Consistency Checks
If the first equation holds, doubling it gives $2x+4y=6$, which cannot equal the second equation's required value $7$. Thus no pair $(x,y)$ can satisfy both equations.

## 5. Final Answer
$$\boxed{\text{The system is inconsistent and has no solution.}}$$