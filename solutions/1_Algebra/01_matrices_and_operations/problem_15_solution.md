# Exercise 15 — Associativity of Multiplication and Different Calculation Paths

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},\quad
C=\begin{pmatrix}2&1\\0&-1\end{pmatrix},
\]
compute \((AB)C\) and \(A(BC)\), compare them, and explain associativity.

## 2. Theoretical Background and Concepts

Matrix multiplication is associative: \((AB)C=A(BC)\) whenever the products are defined. Associativity allows the grouping of factors to change without changing their order or the final result. Different groupings can involve different intermediate calculations.

## 3. Detailed Step-by-Step Solution

### A. Calculate \((AB)C\)

First,
\[
AB=\begin{pmatrix}
1(1)+2(2)+0(-1)&1(0)+2(1)+0(3)\\
0(1)+1(2)+1(-1)&0(0)+1(1)+1(3)
\end{pmatrix}
=\begin{pmatrix}5&2\\1&4\end{pmatrix}.
\]
Then,
\[
(AB)C=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=\boxed{\begin{pmatrix}10&3\\2&-3\end{pmatrix}}.
\]

### B. Calculate \(A(BC)\)

First,
\[
BC=
\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}.
\]
Then,
\[
A(BC)=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}
=\boxed{\begin{pmatrix}10&3\\2&-3\end{pmatrix}}.
\]

## 4. Verification and Consistency Checks

Both paths give the same \(2\times2\) matrix:
\[
(AB)C=A(BC)=\begin{pmatrix}10&3\\2&-3\end{pmatrix}.
\]
The intermediate dimensions are valid: \(AB\) is \(2\times2\), \((AB)C\) is \(2\times2\); \(BC\) is \(3\times2\), and \(A(BC)\) is also \(2\times2\). Associativity allows the grouping to change, not the order of the factors.

## Final Answer

\[
\boxed{(AB)C=A(BC)=\begin{pmatrix}10&3\\2&-3\end{pmatrix}}.
\]
