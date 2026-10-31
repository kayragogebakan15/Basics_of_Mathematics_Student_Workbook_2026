# Exercise 4 — Gauss–Jordan Elimination

## 1. Problem Statement
Find $A^{-1}$ using the Gauss–Jordan method for
$$A=\begin{pmatrix}1&2\\3&5\end{pmatrix}.$$
Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

## 2. Method and Key Formula
Gauss–Jordan elimination applies elementary row operations to $[A\mid I]$. Each row operation is equivalent to left multiplication by an invertible elementary matrix. If the left side becomes $I$, the same operations have transformed the right side into $A^{-1}$.

## 3. Detailed Step-by-Step Solution
Start with the augmented matrix:
$$
\left[\begin{array}{cc|cc}
1&2&1&0\\3&5&0&1
\end{array}\right].
$$
Eliminate the 3 below the first pivot using $R_2\leftarrow R_2-3R_1$:
$$
\left[\begin{array}{cc|cc}
1&2&1&0\\0&-1&-3&1
\end{array}\right].
$$
Make the second pivot equal to 1 using $R_2\leftarrow -R_2$:
$$
\left[\begin{array}{cc|cc}
1&2&1&0\\0&1&3&-1
\end{array}\right].
$$
Eliminate the 2 above the second pivot using $R_1\leftarrow R_1-2R_2$:
$$
\left[\begin{array}{cc|cc}
1&0&-5&2\\0&1&3&-1
\end{array}\right].
$$
The left block is now $I$, so the right block is the inverse.

## 4. Verification and Consistency Checks
Check by multiplication:
$$
\begin{pmatrix}1&2\\3&5\end{pmatrix}
\begin{pmatrix}-5&2\\3&-1\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$
The row operations are reversible, and the product check confirms the right block.

## 5. Final Answer
$$\boxed{A^{-1}=\begin{pmatrix}-5&2\\3&-1\end{pmatrix}.}$$