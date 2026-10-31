# Exercise 2 — Formula for a 2×2 Matrix

## 1. Problem Statement
Find the inverse of
$$A=\begin{pmatrix}3&2\\5&4\end{pmatrix}$$
using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## 2. Method and Key Formula
For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, if $ad-bc\ne0$, then
$$A^{-1}=\frac{1}{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}.$$
The determinant must be nonzero; otherwise the inverse does not exist.

## 3. Detailed Step-by-Step Solution
Calculate the determinant:
$$\det(A)=3\cdot4-2\cdot5=12-10=2.$$
Since $2\ne0$, the inverse exists. Substitute the entries into the formula:
$$
A^{-1}=\frac12\begin{pmatrix}4&-2\\-5&3\end{pmatrix}
=\begin{pmatrix}2&-1\\-\frac52&\frac32\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
Multiply $A$ by the proposed inverse:
$$
AA^{-1}=\begin{pmatrix}3&2\\5&4\end{pmatrix}
\begin{pmatrix}2&-1\\-\frac52&\frac32\end{pmatrix}
=\begin{pmatrix}
6-5&-3+3\\
10-10&-5+6
\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$
The product is the identity, confirming the result.

## 5. Final Answer
$$\boxed{A^{-1}=\begin{pmatrix}2&-1\\-\frac52&\frac32\end{pmatrix}.}$$