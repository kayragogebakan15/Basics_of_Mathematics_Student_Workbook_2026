# Exercise 1 — From a System to a Matrix

## 1. Problem Statement
Write the system
$$\begin{cases}2x-y+z=4,\\x+3y-2z=1,\\3x+y+z=7\end{cases}$$
in the form $Ax=b$. Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row corresponds to one equation.

## 2. Method and Key Formula
A linear system is written as $Ax=b$, where each row of $A$ contains the coefficients of the unknowns in one equation, $x$ is the column of unknowns, and $b$ contains the right-hand-side constants. The order of variables must be the same in every row.

## 3. Detailed Step-by-Step Solution
Choose the unknown vector in the order
$$x=\begin{pmatrix}x\\y\\z\end{pmatrix}.$$
Read the coefficients of $x,y,z$ from the first equation: $(2,-1,1)$, with right-hand side $4$. The second equation gives $(1,3,-2)$ and $1$. The third gives $(3,1,1)$ and $7$. Therefore,
$$
A=\begin{pmatrix}2&-1&1\\1&3&-2\\3&1&1\end{pmatrix},
\qquad
b=\begin{pmatrix}4\\1\\7\end{pmatrix}.
$$
The system is
$$
\begin{pmatrix}2&-1&1\\1&3&-2\\3&1&1\end{pmatrix}
\begin{pmatrix}x\\y\\z\end{pmatrix}
=
\begin{pmatrix}4\\1\\7\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
Multiplying row 1 by the unknown vector gives $2x-y+z$, row 2 gives $x+3y-2z$, and row 3 gives $3x+y+z$. These are exactly the left-hand sides of the original equations, in the same order.

## 5. Final Answer
$$\boxed{A=\begin{pmatrix}2&-1&1\\1&3&-2\\3&1&1\end{pmatrix},\quad
x=\begin{pmatrix}x\\y\\z\end{pmatrix},\quad
b=\begin{pmatrix}4\\1\\7\end{pmatrix},\quad Ax=b.}$$