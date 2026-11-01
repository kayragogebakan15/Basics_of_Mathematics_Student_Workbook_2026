# Exercise 9 — Matrix Equation

## 1. Problem Statement
Given
$$A=\begin{pmatrix}1&2\\0&1\end{pmatrix},\qquad B=\begin{pmatrix}3&1\\2&4\end{pmatrix},$$
solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## 2. Method and Key Formula
Since $A$ multiplies $X$ on the left, multiply both sides on the left by $A^{-1}$:
$$A^{-1}(AX)=A^{-1}B\quad\Longrightarrow\quad X=A^{-1}B.$$
Matrix multiplication is not generally commutative, so the side matters.

## 3. Detailed Step-by-Step Solution
The determinant is $\det A=1\cdot1-2\cdot0=1$. By the $2\times2$ inverse formula,
$A^{-1}=\frac11\begin{pmatrix}1&-2\\0&1\end{pmatrix}
=\begin{pmatrix}1&-2\\0&1\end{pmatrix}.$
Because $A$ multiplies $X$ on the left, multiply $AX=B$ on the left by $A^{-1}$:
$A^{-1}(AX)=(A^{-1}A)X=IX=X=A^{-1}B.$
This explains the side on which the inverse must be applied. Therefore,
$$
X=A^{-1}B
=\begin{pmatrix}1&-2\\0&1\end{pmatrix}
\begin{pmatrix}3&1\\2&4\end{pmatrix}
=\begin{pmatrix}3-4&1-8\\2&4\end{pmatrix}
=\begin{pmatrix}-1&-7\\2&4\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
Compute the original left-hand side:
$$
AX=\begin{pmatrix}1&2\\0&1\end{pmatrix}
\begin{pmatrix}-1&-7\\2&4\end{pmatrix}
=\begin{pmatrix}-1+4&-7+8\\2&4\end{pmatrix}
=\begin{pmatrix}3&1\\2&4\end{pmatrix}=B.
$$
The equation is satisfied.

## 5. Final Answer
$$\boxed{X=\begin{pmatrix}-1&-7\\2&4\end{pmatrix}.}$$