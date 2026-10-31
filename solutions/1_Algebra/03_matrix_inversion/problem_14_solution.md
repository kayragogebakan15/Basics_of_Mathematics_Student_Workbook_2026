# Exercise 14 — A Matrix That Is Its Own Inverse

## 1. Problem Statement
Assume that a square matrix $A$ satisfies $A^2=I$. Show that $A^{-1}=A$. Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

## 2. Method and Key Formula
By definition, $A^{-1}$ is a matrix that multiplies with $A$ on either side to give the identity. The equation $A^2=I$ means $AA=I$.

## 3. Detailed Step-by-Step Solution
Since $A^2=I$, we have
$$AA=I\quad\text{and}\quad AA=I.$$
Thus $A$ itself is both a left and right inverse of $A$. By uniqueness of the inverse, $A^{-1}=A$.

Choose the matrix
$$A=\begin{pmatrix}0&1\\1&0\end{pmatrix}.$$
It is not equal to $I$ or $-I$. Its square is
$$
A^2=\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}=I.
$$

## 4. Verification and Consistency Checks
The multiplication confirms the condition exactly. Therefore this example is its own inverse, as the general argument predicts.

## 5. Final Answer
$$\boxed{A^{-1}=A\text{ whenever }A^2=I.\quad
\text{Example: }A=\begin{pmatrix}0&1\\1&0\end{pmatrix}.}$$