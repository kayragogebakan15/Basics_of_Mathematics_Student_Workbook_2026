# Exercise 15 — Two Methods for Solving the Same System

## 1. Problem Statement
For
$$A=\begin{pmatrix}2&1\\1&3\end{pmatrix},\qquad b=\begin{pmatrix}7\\8\end{pmatrix},$$
solve $Ax=b$ in two ways: (1) using $A^{-1}b$, and (2) using Gaussian elimination. Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## 2. Method and Key Formula
The inverse method uses $x=A^{-1}b$ when $A$ is invertible. Gaussian elimination applies elementary row operations to the augmented matrix $[A\mid b]$ until the unknowns can be read from an equivalent triangular or reduced system.

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
Both methods give the same vector and both original equations hold. In this small example, Gaussian elimination is simpler because it avoids calculating and displaying the full inverse. The inverse method is useful when the inverse is already available or reused for several right-hand sides.

## 5. Final Answer
$$\boxed{x=\begin{pmatrix}\frac{13}{5}\\\frac95\end{pmatrix}.}$$