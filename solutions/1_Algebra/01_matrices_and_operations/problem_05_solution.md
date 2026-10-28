# Exercise 5 — Matrix Times Vector

## 1. Problem Statement

Let
\[
A=\begin{pmatrix}2&-1\\1&3\end{pmatrix},\qquad
x=\begin{pmatrix}4\\2\end{pmatrix}.
\]
Compute \(Ax\), then express it as a linear combination of the columns of \(A\).

## 2. Theoretical Background and Concepts

A matrix with size \(m\times n\) can multiply a column vector with \(n\) entries. If the columns of \(A\) are \(a_1,\ldots,a_n\) and \(x=(x_1,\ldots,x_n)^T\), then
\[
Ax=x_1a_1+\cdots+x_na_n.
\]

## 3. Detailed Step-by-Step Solution

Using row-by-column multiplication,
\[
Ax=\begin{pmatrix}2(4)+(-1)(2)\\1(4)+3(2)\end{pmatrix}
=\boxed{\begin{pmatrix}6\\10\end{pmatrix}}.
\]

The columns of \(A\) are
\[
a_1=\begin{pmatrix}2\\1\end{pmatrix},\qquad
a_2=\begin{pmatrix}-1\\3\end{pmatrix}.
\]
The vector entries are 4 and 2, so
\[
Ax=4a_1+2a_2
=4\begin{pmatrix}2\\1\end{pmatrix}
+2\begin{pmatrix}-1\\3\end{pmatrix}
=\begin{pmatrix}8\\4\end{pmatrix}
+\begin{pmatrix}-2\\6\end{pmatrix}
=\begin{pmatrix}6\\10\end{pmatrix}.
\]

## 4. Verification and Consistency Checks

The direct multiplication and the linear-combination method both produce \((6,10)^T\). The result is a two-entry column vector, consistent with the two rows of \(A\).

## Final Answer

\[
\boxed{Ax=\begin{pmatrix}6\\10\end{pmatrix}=4a_1+2a_2}.
\]
