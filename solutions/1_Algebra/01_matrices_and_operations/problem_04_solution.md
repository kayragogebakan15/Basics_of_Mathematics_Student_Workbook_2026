# Exercise 4 — Matrix Multiplication and Noncommutativity

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},\qquad
B=\begin{pmatrix}2&0\\3&1\end{pmatrix},
\]
compute \(AB\) and \(BA\), and determine whether they are equal.

## 2. Theoretical Background and Concepts

For matrix multiplication, each entry is the dot product of a row of the first matrix and a column of the second. Matrix multiplication is generally not commutative: changing the order of the factors can change the result.

## 3. Detailed Step-by-Step Solution

### A. Compute \(AB\)

\[
AB=\begin{pmatrix}
1(2)+2(3)&1(0)+2(1)\\
0(2)+1(3)&0(0)+1(1)
\end{pmatrix}
=\boxed{\begin{pmatrix}8&2\\3&1\end{pmatrix}}.
\]

### B. Compute \(BA\)

\[
BA=\begin{pmatrix}
2(1)+0(0)&2(2)+0(1)\\
3(1)+1(0)&3(2)+1(1)
\end{pmatrix}
=\boxed{\begin{pmatrix}2&4\\3&7\end{pmatrix}}.
\]

The two matrices are different, for example their upper-left entries are 8 and 2.

## 4. Verification and Consistency Checks

Both products are defined and have size \(2\times2\). Recomputing the row-by-column products gives the same entries above. Since at least one corresponding entry differs, \(AB\ne BA\).

## Final Answer

\[
\boxed{AB=\begin{pmatrix}8&2\\3&1\end{pmatrix}},\qquad
\boxed{BA=\begin{pmatrix}2&4\\3&7\end{pmatrix}},\qquad
\boxed{AB\ne BA}.
\]
Noncommutativity means that the order of matrix factors generally matters.
