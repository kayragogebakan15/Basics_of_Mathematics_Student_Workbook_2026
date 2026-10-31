# Exercise 6 — Solving a System Using the Inverse

## 1. Problem Statement
Solve $Ax=b$, where
$$A=\begin{pmatrix}2&1\\1&3\end{pmatrix},\qquad b=\begin{pmatrix}5\\7\end{pmatrix},$$
using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## 2. Method and Key Formula
If $A$ is invertible, multiply $Ax=b$ on the left by $A^{-1}$:
$$A^{-1}Ax=A^{-1}b\quad\Longrightarrow\quad x=A^{-1}b.$$
We first find the inverse and then multiply it by $b$.

## 3. Detailed Step-by-Step Solution
The determinant is
$$\det(A)=2\cdot3-1\cdot1=5\ne0.$$
Therefore,
$$A^{-1}=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}.$$
Now calculate:
$$
x=A^{-1}b
=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}
\begin{pmatrix}5\\7\end{pmatrix}
=\frac15\begin{pmatrix}15-7\\-5+14\end{pmatrix}
=\begin{pmatrix}\frac85\\\frac95\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
Substitute into the original system:
$$
Ax=\begin{pmatrix}2&1\\1&3\end{pmatrix}
\begin{pmatrix}\frac85\\\frac95\end{pmatrix}
=\begin{pmatrix}\frac{16}{5}+\frac95\\\frac85+\frac{27}{5}\end{pmatrix}
=\begin{pmatrix}5\\7\end{pmatrix}=b.
$$
Both equations are satisfied.

## 5. Final Answer
$$\boxed{x=\begin{pmatrix}\frac85\\\frac95\end{pmatrix}.}$$