# Exercise 2 — Addition and Scalar Multiplication

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&2\\-1&3\end{pmatrix},\qquad
B=\begin{pmatrix}4&-2\\0&5\end{pmatrix},
\]
compute \(A+B\), \(A-B\), and \(3A-2B\). Explain why addition requires equal matrix sizes.

## 2. Theoretical Background and Concepts

Matrices of the same size are added or subtracted entry by entry. Scalar multiplication multiplies every entry by the scalar. Addition requires equal dimensions so that each entry has a corresponding entry in the other matrix.

## 3. Detailed Step-by-Step Solution

### A. Addition

\[
A+B=\begin{pmatrix}1+4&2+(-2)\\-1+0&3+5\end{pmatrix}
=\boxed{\begin{pmatrix}5&0\\-1&8\end{pmatrix}}.
\]

### B. Subtraction

\[
A-B=\begin{pmatrix}1-4&2-(-2)\\-1-0&3-5\end{pmatrix}
=\boxed{\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}}.
\]

### C. Scalar combination

\[
3A=\begin{pmatrix}3&6\\-3&9\end{pmatrix},\qquad
2B=\begin{pmatrix}8&-4\\0&10\end{pmatrix}.
\]
Therefore,
\[
3A-2B=\begin{pmatrix}3-8&6-(-4)\\-3-0&9-10\end{pmatrix}
=\boxed{\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}}.
\]

## 4. Verification and Consistency Checks

All results are \(2\times2\), as required. For example, the upper-right entry of \(3A-2B\) is \(3(2)-2(-2)=6+4=10\), confirming the sign handling.

## Final Answer

\[
\boxed{A+B=\begin{pmatrix}5&0\\-1&8\end{pmatrix}},\quad
\boxed{A-B=\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}}
\]
\[
\boxed{3A-2B=\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}}.
\]
