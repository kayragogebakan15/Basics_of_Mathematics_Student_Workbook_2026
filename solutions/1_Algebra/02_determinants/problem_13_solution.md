# Exercise 13 — Determinant by Elimination

## 1. Problem Statement

Compute the determinant of
\[
A=\begin{pmatrix}1&2&3\\2&5&7\\1&0&2\end{pmatrix}
\]
using elimination. Record the effect of every row operation on the determinant.

## 2. Method and Key Formula

Use row replacements to create zeros below the first pivot. Row replacements of the form \(R_i\leftarrow R_i+cR_j\) do not change the determinant. Once the matrix is upper triangular, its determinant is the product of its diagonal entries.

## 3. Detailed Step-by-Step Solution

Begin with
\[
A=\begin{pmatrix}1&2&3\\2&5&7\\1&0&2\end{pmatrix}.
\]

**Step 1:** Apply \(R_2\leftarrow R_2-2R_1\):
\((2,5,7)-2(1,2,3)=(0,1,1).\)
Thus,
\[
A_1=\begin{pmatrix}1&2&3\\0&1&1\\1&0&2\end{pmatrix},
\qquad \det A_1=\det A.
\]
The determinant is unchanged because this is a row replacement.

**Step 2:** Apply \(R_3\leftarrow R_3-R_1\):
\((1,0,2)-(1,2,3)=(0,-2,-1).\)
Therefore,
\[
A_2=\begin{pmatrix}1&2&3\\0&1&1\\0&-2&-1\end{pmatrix},
\qquad \det A_2=\det A_1.
\]

**Step 3:** Apply \(R_3\leftarrow R_3+2R_2\):
\((0,-2,-1)+2(0,1,1)=(0,0,1).\)
Hence,
\[
A_3=\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix},
\qquad \det A_3=\det A_2.
\]
The resulting matrix is upper triangular, so
\(\det A_3=1\cdot1\cdot1=1.\)

## 4. Verification and Consistency Checks

All three steps are row replacements, so no determinant sign or scale factor was introduced. Therefore,
\(\det A=\det A_1=\det A_2=\det A_3=1.\)
A direct expansion along the first row confirms this:
\[
\begin{aligned}
\det A\\
&=1(5\cdot2-7\cdot0)-2(2\cdot2-7\cdot1)
+3(2\cdot0-5\cdot1)\\
&=10-2(-3)+3(-5)\\
&=10+6-15\\
&=1.
\end{aligned}
\]

## 5. Final Answer

\(\boxed{\det A=1}\)