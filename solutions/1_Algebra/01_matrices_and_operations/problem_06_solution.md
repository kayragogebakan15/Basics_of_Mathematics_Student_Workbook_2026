# Exercise 6 — Transpose

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix},\qquad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},
\]
compute \(A^T\), \(B^T\), and \(AB\), then verify \((AB)^T=B^TA^T\).

## 2. Theoretical Background and Concepts

The transpose interchanges rows and columns. If \(A\) is \(m\times n\), then \(A^T\) is \(n\times m\). A key identity is \((AB)^T=B^TA^T\), where the order of factors reverses.

## 3. Detailed Step-by-Step Solution

The transposes are
\[
A^T=\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix},\qquad
B^T=\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}.
\]

Since \(A\) is \(2\times3\) and \(B\) is \(3\times2\), \(AB\) is defined and has size \(2\times2\):
\[
AB=\begin{pmatrix}
1(1)+2(2)+3(-1)&1(0)+2(1)+3(3)\\
4(1)+5(2)+6(-1)&4(0)+5(1)+6(3)
\end{pmatrix}
=\boxed{\begin{pmatrix}2&11\\8&23\end{pmatrix}}.
\]
Therefore,
\[
(AB)^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}.
\]

Now calculate the other side:
\[
B^TA^T=
\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}
=\begin{pmatrix}
1+4-3&4+10-6\\
0+2+9&0+5+18
\end{pmatrix}
=\begin{pmatrix}2&8\\11&23\end{pmatrix}.
\]

## 4. Verification and Consistency Checks

Both sides equal \(\begin{pmatrix}2&8\\11&23\end{pmatrix}\). The dimensions also agree: \(AB\) is \(2\times2\), so its transpose is \(2\times2\); \(B^T\) is \(2\times3\) and \(A^T\) is \(3\times2\), making their product \(2\times2\).

## Final Answer

\[
\boxed{A^T=\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}},\quad
\boxed{B^T=\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}},\quad
\boxed{AB=\begin{pmatrix}2&11\\8&23\end{pmatrix}}
\]
and \(\boxed{(AB)^T=B^TA^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}}\).
