# Exercise 10 — Inverse of a Diagonal Matrix

## 1. Problem Statement
Given
$$D=\begin{pmatrix}2&0&0\\0&-3&0\\0&0&5\end{pmatrix},\qquad
E=\begin{pmatrix}2&0&0\\0&0&0\\0&0&5\end{pmatrix},$$
without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## 2. Method and Key Formula
The determinant of a diagonal matrix is the product of its diagonal entries. It is invertible exactly when every diagonal entry is nonzero. Its inverse is obtained by taking the reciprocal of each diagonal entry.

## 3. Detailed Step-by-Step Solution
For $D$,
$$\det(D)=2(-3)(5)=-30\ne0,$$
so $D$ is invertible and
$$D^{-1}=\begin{pmatrix}\frac12&0&0\\0&-\frac13&0\\0&0&\frac15\end{pmatrix}.$$
For $E$,
$$\det(E)=2\cdot0\cdot5=0.$$
The zero on the diagonal means one coordinate is mapped to zero, so the transformation cannot be reversed.

## 4. Verification and Consistency Checks
Multiplication gives
$$DD^{-1}=\begin{pmatrix}2(\frac12)&0&0\\0&(-3)(-\frac13)&0\\0&0&5(\frac15)\end{pmatrix}=I_3.$$
This confirms the inverse. The determinant test excludes $E$.

## 5. Final Answer
$$\boxed{D^{-1}=\begin{pmatrix}\frac12&0&0\\0&-\frac13&0\\0&0&\frac15\end{pmatrix},\qquad E^{-1}\text{ does not exist.}}$$