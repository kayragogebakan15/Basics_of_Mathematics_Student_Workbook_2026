# Exercise 8 — Determinant of a Product

## 1. Problem Statement

Let \(A\) and \(B\) be square matrices with \(\det A=3\) and \(\det B=-5\). Compute
\[
\det(AB),\qquad \det(BA),\qquad \det(A^{-1}B)
\]
if the last expression exists. Explain why the first two results are equal even though usually \(AB\neq BA\).

## 2. Method and Key Formula

For square matrices of the same size,
\[
\det(AB)=\det A\,\det B.
\]
If \(\det A\neq0\), then \(A^{-1}\) exists and
\[
\det(A^{-1})=\frac{1}{\det A}.
\]

## 3. Detailed Step-by-Step Solution

For \(AB\),
\[
\det(AB)=\det A\det B=3(-5)=-15.
\]

For \(BA\),
\[
\det(BA)=\det B\det A=(-5)(3)=-15.
\]
The scalar factors commute, so \(\det A\det B=\det B\det A\), even though the matrices \(A\) and \(B\) themselves need not commute.

Because \(\det A=3\neq0\), \(A^{-1}\) exists. Therefore,
\[
\det(A^{-1})=\frac{1}{3}.
\]
It follows that
\[
\det(A^{-1}B)=\det(A^{-1})\det B
=\frac13(-5)=-\frac53.
\]

## 4. Verification and Consistency Checks

The determinant product rule gives the same scalar product in either order:
\[
\det(AB)=3(-5)=(-5)3=\det(BA).
\]
This does not imply \(AB=BA\); a determinant records a scalar property of a matrix, not all of its entries.

## 5. Final Answer

\[
\boxed{\det(AB)=-15,\quad \det(BA)=-15,\quad
\det(A^{-1}B)=-\frac53}
\]
The inverse expression exists because \(\det A\neq0\).