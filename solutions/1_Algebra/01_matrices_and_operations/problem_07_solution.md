# Exercise 7 — Identity Matrix, Zero Matrix, and Powers

## 1. Problem Statement

For
\[
A=\begin{pmatrix}2&1\\0&2\end{pmatrix},
\]
compute \(AI\), \(IA\), \(A+0\), \(A^2\), and \(A^3\). Explain the roles of the identity and zero matrices and identify the pattern in the powers.

## 2. Theoretical Background and Concepts

For square matrices, the identity matrix \(I\) has 1s on the main diagonal and 0s elsewhere; it is the multiplicative identity. The zero matrix \(0\) has only zero entries and is the additive identity. Matrix powers are repeated products: \(A^2=AA\) and \(A^3=AAA\).

## 3. Detailed Step-by-Step Solution

For this problem,
\[
I=\begin{pmatrix}1&0\\0&1\end{pmatrix},\qquad
0=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
\]
Thus,
\[
AI=IA=A=\begin{pmatrix}2&1\\0&2\end{pmatrix},\qquad
A+0=A=\begin{pmatrix}2&1\\0&2\end{pmatrix}.
\]

For the square, each entry is the dot product of a row of \(A\) with a column of \(A\):
\[
\begin{aligned}
(A^2)_{11}&=2\cdot2+1\cdot0=4,\\
(A^2)_{12}&=2\cdot1+1\cdot2=4,\\
(A^2)_{21}&=0\cdot2+2\cdot0=0,\\
(A^2)_{22}&=0\cdot1+2\cdot2=4.
\end{aligned}
\]
Therefore,
\[
A^2=\begin{pmatrix}2&1\\0&2\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
=\boxed{\begin{pmatrix}4&4\\0&4\end{pmatrix}}.
\]

For the cube, use \(A^3=A^2A\) and apply the same row-by-column rule:
\[
\begin{aligned}
(A^3)_{11}&=4\cdot2+4\cdot0=8,\\
(A^3)_{12}&=4\cdot1+4\cdot2=12,\\
(A^3)_{21}&=0\cdot2+4\cdot0=0,\\
(A^3)_{22}&=0\cdot1+4\cdot2=8.
\end{aligned}
\]
Thus,
\[
A^3=\begin{pmatrix}4&4\\0&4\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
=\boxed{\begin{pmatrix}8&12\\0&8\end{pmatrix}}.
\]

The pattern is
\[
A^n=\begin{pmatrix}2^n&n2^{n-1}\\0&2^n\end{pmatrix}
\quad(n\geq1).
\]
The diagonal entries double with each new power, and the upper-right entry follows \(1,4,12,\ldots\), given by \(n2^{n-1}\).

## 4. Verification and Consistency Checks

Multiplying the proposed formula for \(A^n\) by \(A\) gives
\[
\begin{pmatrix}2^n&n2^{n-1}\\0&2^n\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
=\begin{pmatrix}2^{n+1}&2^n+n2^n\\0&2^{n+1}\end{pmatrix}
=\begin{pmatrix}2^{n+1}&(n+1)2^n\\0&2^{n+1}\end{pmatrix},
\]
which confirms the pattern advances correctly.

## Final Answer

\[
\boxed{AI=IA=A,\quad A+0=A}
\]
\[
\boxed{A^2=\begin{pmatrix}4&4\\0&4\end{pmatrix},\quad
A^3=\begin{pmatrix}8&12\\0&8\end{pmatrix}}.
\]
