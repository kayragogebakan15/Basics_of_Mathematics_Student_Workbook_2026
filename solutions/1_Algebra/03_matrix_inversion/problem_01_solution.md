# Exercise 1 — Definition of the Inverse

## 1. Problem Statement
For
$$A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad B=\begin{pmatrix}1&-1\\-1&2\end{pmatrix},$$
check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## 2. Method and Key Formula
A square matrix $B$ is the inverse of $A$ if both products equal the identity matrix:
$$AB=BA=I.$$
For a $2\times2$ matrix, $I=\begin{pmatrix}1&0\\0&1\end{pmatrix}$. We will verify the definition directly by row-by-column multiplication.

## 3. Detailed Step-by-Step Solution
First calculate $AB$:
$$
AB=\begin{pmatrix}2&1\\1&1\end{pmatrix}
\begin{pmatrix}1&-1\\-1&2\end{pmatrix}
=\begin{pmatrix}
2(1)+1(-1)&2(-1)+1(2)\\
1(1)+1(-1)&1(-1)+1(2)
\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$
Now calculate the product in the opposite order:
$$
BA=\begin{pmatrix}1&-1\\-1&2\end{pmatrix}
\begin{pmatrix}2&1\\1&1\end{pmatrix}
=\begin{pmatrix}
1(2)+(-1)(1)&1(1)+(-1)(1)\\
(-1)(2)+2(1)&(-1)(1)+2(1)
\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
Both products equal the identity matrix. The dimensions are also valid: both factors are $2\times2$, so both products are defined and are $2\times2$.

## 5. Final Answer
$$\boxed{B=A^{-1}=\begin{pmatrix}1&-1\\-1&2\end{pmatrix}.}$$