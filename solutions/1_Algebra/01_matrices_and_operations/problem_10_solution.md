# Exercise 10 — Columns of a Matrix Product

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},\qquad
B=\begin{pmatrix}1&2\\-1&0\\3&1\end{pmatrix},
\]
let the columns of \(B\) be \(b_1,b_2\). Compute \(Ab_1\), \(Ab_2\), and \(AB\), then explain the relationship.

## 2. Theoretical Background and Concepts

If \(B=[b_1\ b_2\ \cdots\ b_n]\), then
\[
AB=[Ab_1\ Ab_2\ \cdots\ Ab_n].
\]
Each column of the product is obtained by multiplying \(A\) by the corresponding column of \(B\). In detail, the entry in row \(i\), column \(j\) of \(AB\) is the dot product of row \(i\) of \(A\) with column \(j\) of \(B\). This is exactly the \(i\)-th entry of \(Ab_j\). Since this holds for every row \(i\), the entire \(j\)-th column of \(AB\) equals \(Ab_j\`.

## 3. Detailed Step-by-Step Solution

The columns of \(B\) are
\[
b_1=\begin{pmatrix}1\\-1\\3\end{pmatrix},\qquad
b_2=\begin{pmatrix}2\\0\\1\end{pmatrix}.
\]

First,
\[
Ab_1=\begin{pmatrix}1(1)+2(-1)+0(3)\\0(1)+1(-1)+1(3)\end{pmatrix}
=\boxed{\begin{pmatrix}-1\\2\end{pmatrix}}.
\]
Second,
\[
Ab_2=\begin{pmatrix}1(2)+2(0)+0(1)\\0(2)+1(0)+1(1)\end{pmatrix}
=\boxed{\begin{pmatrix}2\\1\end{pmatrix}}.
\]

Therefore,
\[
AB=\begin{pmatrix}-1&2\\2&1\end{pmatrix}.
\]

## 4. Verification and Consistency Checks

The first column of the computed product is \((-1,2)^T=Ab_1\), and the second is \((2,1)^T=Ab_2\). The product dimensions are also consistent: \((2\times3)(3\times2)\) produces a \(2\times2\) matrix.

## Final Answer

\[
\boxed{Ab_1=\begin{pmatrix}-1\\2\end{pmatrix},\quad
Ab_2=\begin{pmatrix}2\\1\end{pmatrix},\quad
AB=\begin{pmatrix}-1&2\\2&1\end{pmatrix}}.
\]
