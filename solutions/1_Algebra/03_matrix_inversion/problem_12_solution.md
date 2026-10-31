# Exercise 12 — Finding Inverses Without Starting from Scratch

## 1. Problem Statement
It is known that
$$A^{-1}=\begin{pmatrix}2&-1\\-3&2\end{pmatrix}.$$
Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## 2. Method and Key Formula
For an invertible matrix $A$ and nonzero scalar $c$:
$$(cA)^{-1}=\frac1cA^{-1},\qquad (A^T)^{-1}=(A^{-1})^T,\qquad (A^2)^{-1}=(A^{-1})^2.$$
These follow by multiplying each proposed inverse by the original matrix and obtaining the identity.

## 3. Detailed Step-by-Step Solution
**1. Scalar multiple**
$$
(3A)^{-1}=\frac13A^{-1}
=\begin{pmatrix}\frac23&-\frac13\\-1&\frac23\end{pmatrix}.
$$
**2. Transpose**
$$
(A^T)^{-1}=(A^{-1})^T
=\begin{pmatrix}2&-3\\-1&2\end{pmatrix}.
$$
**3. Square**
$$
(A^2)^{-1}=(A^{-1})^2
=\begin{pmatrix}2&-1\\-3&2\end{pmatrix}
\begin{pmatrix}2&-1\\-3&2\end{pmatrix}
=\begin{pmatrix}4+3&-2-2\\-6-6&3+4\end{pmatrix}
=\begin{pmatrix}7&-4\\-12&7\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
For the scalar case, $(3A)(\frac13A^{-1})=AA^{-1}=I$. For the transpose case, $(A^T)(A^{-1})^T=(A^{-1}A)^T=I$. For the square case, $A^2(A^{-1})^2=A(AA^{-1})A^{-1}=I$.

## 5. Final Answer
$$
\boxed{(3A)^{-1}=\begin{pmatrix}\frac23&-\frac13\\-1&\frac23\end{pmatrix},\quad
(A^T)^{-1}=\begin{pmatrix}2&-3\\-1&2\end{pmatrix},\quad
(A^2)^{-1}=\begin{pmatrix}7&-4\\-12&7\end{pmatrix}.}
$$