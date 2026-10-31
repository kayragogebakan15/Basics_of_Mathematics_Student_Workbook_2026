# Exercise 11 — Simplifying a Determinant with Row Operations

## 1. Problem Statement

Compute
\[
\det\begin{pmatrix}1&2&3\\1&3&4\\1&4&6\end{pmatrix}
\]
by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## 2. Method and Key Formula

Replacing a row by itself plus a multiple of another row does not change the determinant. We can use such operations to create zeros below the first pivot, then use the triangular-matrix rule if the matrix becomes triangular.

## 3. Detailed Step-by-Step Solution

Start with
\[
A=\begin{pmatrix}1&2&3\\1&3&4\\1&4&6\end{pmatrix}.
\]

**Step 1:** Apply \(R_2\leftarrow R_2-R_1\). This row replacement leaves the determinant unchanged:
\[
A_1=\begin{pmatrix}1&2&3\\0&1&1\\1&4&6\end{pmatrix},
\qquad \det A_1=\det A.
\]

**Step 2:** Apply \(R_3\leftarrow R_3-R_1\). This also leaves the determinant unchanged:
\[
A_2=\begin{pmatrix}1&2&3\\0&1&1\\0&2&3\end{pmatrix},
\qquad \det A_2=\det A_1.
\]

**Step 3:** Apply \(R_3\leftarrow R_3-2R_2\):
\[
A_3=\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix},
\qquad \det A_3=\det A_2.
\]
The matrix is now upper triangular, so
\(\det A_3=1\cdot1\cdot1=1.\)

## 4. Verification and Consistency Checks

All three operations were row replacements; none changed the determinant. Therefore,
\(\det A=\det A_1=\det A_2=\det A_3=1.\)
As a check, direct expansion along the first row gives
\[
\det A=1(3\cdot6-4\cdot4)-2(1\cdot6-4\cdot1)
+3(1\cdot4-3\cdot1)=2-4+3=1.
\]

## 5. Final Answer

\(\boxed{\det A=1}\)