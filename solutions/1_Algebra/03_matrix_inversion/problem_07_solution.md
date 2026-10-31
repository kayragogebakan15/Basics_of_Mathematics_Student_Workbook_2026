# Exercise 7 — Inverse of a Product

## 1. Problem Statement
For
$$A=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad B=\begin{pmatrix}2&0\\0&3\end{pmatrix},$$
compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## 2. Method and Key Formula
For invertible square matrices,
$$(AB)^{-1}=B^{-1}A^{-1}.$$
The order is reversed because the operation performed last must be undone first.

## 3. Detailed Step-by-Step Solution
First calculate the product:
$$AB=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}2&0\\0&3\end{pmatrix}
=\begin{pmatrix}2&3\\0&3\end{pmatrix}.$$
Its determinant is $6$, so it is invertible. Using the $2\times2$ formula,
$$
(AB)^{-1}=\frac16\begin{pmatrix}3&-3\\0&2\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&\frac13\end{pmatrix}.
$$
Separately,
$$A^{-1}=\begin{pmatrix}1&-1\\0&1\end{pmatrix},\qquad
B^{-1}=\begin{pmatrix}\frac12&0\\0&\frac13\end{pmatrix}.$$
Then
$$
B^{-1}A^{-1}
=\begin{pmatrix}\frac12&0\\0&\frac13\end{pmatrix}
\begin{pmatrix}1&-1\\0&1\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&\frac13\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
The two calculations give identical matrices. The property can also be checked from the definition:
$$(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AIA^{-1}=I.$$

## 5. Final Answer
$$\boxed{(AB)^{-1}=B^{-1}A^{-1}=\begin{pmatrix}\frac12&-\frac12\\0&\frac13\end{pmatrix}.}$$