# Exercise 10 — Detecting Linear Dependence

## 1. Problem Statement

Without carrying out a full determinant calculation, explain why
$
\det\begin{pmatrix}1&2&3\\2&4&6\\0&1&5\end{pmatrix}=0.
$
Identify a dependence between the rows and connect it with noninvertibility.

## 2. Method and Key Formula

If a square matrix has two linearly dependent rows, its determinant is zero. In particular, multiplying a row by a scalar to obtain another row creates dependence. A square matrix with determinant zero is not invertible.

## 3. Detailed Step-by-Step Solution

Let the rows be
$
r_1=(1,2,3),\quad r_2=(2,4,6),\quad r_3=(0,1,5).
$
Observe that
$
r_2=2r_1.
$
Equivalently,
$
r_2-2r_1=(0,0,0).
$
Thus, the rows are linearly dependent: one row is a scalar multiple of another. A determinant with linearly dependent rows equals zero, so no full determinant expansion is necessary:
$
\det A=0.
$

Since $\det A=0$, the matrix is singular and therefore not invertible.

## 4. Verification and Consistency Checks

The dependence is exact:
$
2(1,2,3)=(2,4,6).
$
This directly verifies that the second row adds no independent information.

## 5. Final Answer

$
\boxed{\det A=0}
$
The second row equals twice the first row, so the rows are linearly dependent and the matrix is not invertible.