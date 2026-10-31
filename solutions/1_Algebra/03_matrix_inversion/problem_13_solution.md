# Exercise 13 — Undoing a Composite Transformation

## 1. Problem Statement
The matrices
$$S=\begin{pmatrix}2&0\\0&1\end{pmatrix},\qquad H=\begin{pmatrix}1&1\\0&1\end{pmatrix}$$
describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways: (1) first compute $T$, then its inverse; (2) use $(HS)^{-1}=S^{-1}H^{-1}$. Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## 2. Method and Key Formula
For invertible matrices, $(AB)^{-1}=B^{-1}A^{-1}$. The order reverses because the last transformation applied must be undone first.

## 3. Detailed Step-by-Step Solution
**Method 1: calculate $T$ first.**
$$
T=HS=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}2&0\\0&1\end{pmatrix}
=\begin{pmatrix}2&1\\0&1\end{pmatrix}.
$$
Its determinant is $2$, so
$$
T^{-1}=\frac12\begin{pmatrix}1&-1\\0&2\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.
$$
**Method 2: reverse the factors.**
$$
S^{-1}=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix},\qquad
H^{-1}=\begin{pmatrix}1&-1\\0&1\end{pmatrix}.
$$
Therefore,
$$
S^{-1}H^{-1}
=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}
\begin{pmatrix}1&-1\\0&1\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.
$$
The incorrect order gives
$$
H^{-1}S^{-1}
=\begin{pmatrix}1&-1\\0&1\end{pmatrix}
\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}
=\begin{pmatrix}\frac12&-1\\0&1\end{pmatrix},
$$
which is different.

## 4. Verification and Consistency Checks
Multiplying $T$ by the proposed inverse:
$$
\begin{pmatrix}2&1\\0&1\end{pmatrix}
\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$
The two correct methods agree, while reversing the factors incorrectly does not produce the inverse.

## 5. Final Answer
$$\boxed{T^{-1}=S^{-1}H^{-1}=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.}$$