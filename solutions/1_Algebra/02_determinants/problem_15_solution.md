# Exercise 15 — Combining Determinant Properties

## 1. Problem Statement

Let $A$ and $B$ be invertible $2\times2$ matrices with
$$
\det A=-2,\qquad \det B=3.
$$
Without finding the matrix entries, compute
$$
\det\left(B^{-1}A^TB\right).
$$
State the determinant properties in the order used and explain why the factors involving $B$ cancel.

## 2. Method and Key Formula

Use the product rule, transpose rule, and inverse rule:
$$
\det(XY)=\det X\det Y,\qquad
\det(A^T)=\det A,\qquad
\det(B^{-1})=\frac1{\det B}.
$$
The determinant is a scalar, so its factors can be rearranged.

## 3. Detailed Step-by-Step Solution

Apply the product rule to the three factors:
$$
\det(B^{-1}A^TB)=\det(B^{-1})\det(A^T)\det(B).
$$
Since transposition preserves determinants,
$$
\det(A^T)=\det A=-2.
$$
Since $B$ is invertible and $\det B=3$,
$$
\det(B^{-1})=\frac{1}{\det B}=\frac13.
$$
Substitute:
$$
\begin{aligned}
\det(B^{-1}A^TB)
&=\frac13\cdot(-2)\cdot3\\
&=(-2)\left(\frac13\cdot3\right)\\
&=(-2)\cdot1\\
&=-2.
\end{aligned}
$$
The factors involving $B$ cancel because $\det(B^{-1})\det(B)=\frac13\cdot3=1$.

## 4. Verification and Consistency Checks

The matrix inside the determinant is a product of invertible matrices, so it is invertible. The result $-2\neq0$ is consistent with that fact. More generally,
$$
\det(B^{-1}A^TB)=\det(A^T)=\det A,
$$
because the determinant factors from $B^{-1}$ and $B$ multiply to 1.

## 5. Final Answer

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$