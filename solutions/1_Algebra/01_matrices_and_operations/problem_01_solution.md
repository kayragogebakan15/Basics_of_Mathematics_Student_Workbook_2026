# Exercise 1 — Matrix Size and Entries

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}2&-1&3\\0&4&5\end{pmatrix},\qquad
B=\begin{pmatrix}1&0\\-2&3\\4&1\end{pmatrix}.
\]
Find the sizes of the matrices, identify the requested entries, and write the specified row and column as vectors.

## 2. Theoretical Background and Concepts

The size of a matrix is written as number of rows \(\times\) number of columns. The entry \(a_{ij}\) is in row \(i\), column \(j\). A row vector is written horizontally, while a column vector is written vertically.

## 3. Detailed Step-by-Step Solution

1. Matrix \(A\) has 2 rows and 3 columns, so \(A\) is \(2\times3\).
2. Matrix \(B\) has 3 rows and 2 columns, so \(B\) is \(3\times2\).
3. Reading row first and column second:
   - \(a_{12}=-1\),
   - \(a_{23}=5\),
   - \(b_{21}=-2\),
   - \(b_{32}=1\).
4. The second row of \(A\) is the row vector \((0,4,5)\).
5. The first column of \(B\) is the column vector
\[
\begin{pmatrix}1\\-2\\4\end{pmatrix}.
\]

## 4. Verification and Consistency Checks

The indices match the row and column positions in the displayed matrices. The number of entries in the second row of \(A\) is 3, matching its 3 columns; the first column of \(B\) has 3 entries, matching its 3 rows.

## Final Answer

\[
\boxed{\operatorname{size}(A)=2\times3,\quad \operatorname{size}(B)=3\times2}
\]
\[
\boxed{a_{12}=-1,\ a_{23}=5,\ b_{21}=-2,\ b_{32}=1}
\]
