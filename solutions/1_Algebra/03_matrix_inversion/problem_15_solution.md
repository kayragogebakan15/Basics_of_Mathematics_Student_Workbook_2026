# Exercise 15 — Two Methods for Solving the Same System

## 1. Problem Statement
For
$$A=\begin{pmatrix}2&1\\1&3\end{pmatrix},\qquad b=\begin{pmatrix}7\\8\end{pmatrix},$$
solve $Ax=b$ in two ways: (1) using $A^{-1}b$, and (2) using Gaussian elimination. Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## 2. Method and Key Formula
For a $2\times2$ matrix, the inverse rule is
$\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}
=\frac1{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix},\quad ad-bc\ne0.$
The inverse method calculates the determinant, constructs $A^{-1}$ using this formula, then computes $x=A^{-1}b$. Gaussian elimination instead works on $[A\mid b]$ by row swap, elimination below the first pivot, pivot scaling, and elimination above the second pivot.

## 3. Detailed Step-by-Step Solution
**Method 1: inverse matrix.** First,
$$\det(A)=2\cdot3-1\cdot1=5\ne0,$$
so
$$A^{-1}=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}.$$
Then
$$
x=A^{-1}b
=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}
\begin{pmatrix}7\\8\end{pmatrix}
=\frac15\begin{pmatrix}21-8\\-7+16\end{pmatrix}
=\begin{pmatrix}\frac{13}{5}\\\frac95\end{pmatrix}.
$$
**Method 2: Gaussian elimination.** Start with
$$\left[\begin{array}{cc|c}2&1&7\\1&3&8\end{array}\right].$$
Swap rows, then eliminate the entry below the first pivot:
$$
\left[\begin{array}{cc|c}1&3&8\\2&1&7\end{array}\right]
\xrightarrow{R_2\leftarrow R_2-2R_1}
\left[\begin{array}{cc|c}1&3&8\\0&-5&-9\end{array}\right].
$$
Divide the second row by $-5$:
$$
\left[\begin{array}{cc|c}1&3&8\\0&1&\frac95\end{array}\right].
$$
Eliminate the 3 above the pivot:
$$
\left[\begin{array}{cc|c}1&0&\frac{13}{5}\\0&1&\frac95\end{array}\right].
$$
Thus the two variables are determined.

## 4. Verification and Consistency Checks
Substitute into the original equations:
$$2\left(\frac{13}{5}\right)+\frac95=\frac{35}{5}=7,$$
$$\frac{13}{5}+3\left(\frac95\right)=\frac{40}{5}=8.$$
Both methods give the same vector and both original equations hold. The essential steps are:
- **Inverse method:** determinant calculation, inverse construction by the $2\times2$ formula, then matrix-vector multiplication.
- **Gaussian elimination:** row swap, elimination below the first pivot, scaling the second pivot row, then elimination above that pivot.

For this small system, Gaussian elimination is simpler because it finds the solution directly without constructing all four entries of the inverse. The inverse method is useful when the inverse is already available or reused for several right-hand sides.

## 5. Final Answer
$$\boxed{x=\begin{pmatrix}\frac{13}{5}\\\frac95\end{pmatrix}.}$$