# Exercise 1 — Determinant of a 2×2 Matrix

## 1. Problem Statement

Compute
$
\det\begin{pmatrix}3&-2\\5&4\end{pmatrix},
\qquad
\det\begin{pmatrix}1&7\\2&14\end{pmatrix}.
$
Determine which matrix is invertible and justify the answer.

## 2. Method and Key Formula

For a $2\times2$ matrix
$
M=\begin{pmatrix}a&b\\c&d\end{pmatrix},
$
the determinant is
$
\det M=ad-bc.
$
A square matrix is invertible if and only if its determinant is nonzero.

## 3. Detailed Step-by-Step Solution

For the first matrix,
$
M_1=\begin{pmatrix}3&-2\\5&4\end{pmatrix},
$
we have $a=3$, $b=-2$, $c=5$, and $d=4$. Substituting into the formula,
$\det M_1=3\cdot4-(-2)\cdot5$  
$=12-(-10)$  
$=12+10$  
$=22.$

For the second matrix,
$
M_2=\begin{pmatrix}1&7\\2&14\end{pmatrix},
$
the determinant is
$\det M_2=1\cdot14-7\cdot2$  
$=14-14$  
$=0.$

## 4. Verification and Consistency Checks

The second row of $M_2$ is twice the first row:
$
(2,14)=2(1,7).
$
Its rows are linearly dependent, which is consistent with $\det M_2=0$. The first matrix has a nonzero determinant.

## 5. Final Answer

$
\boxed{\det M_1=22,\qquad \det M_2=0}
$
Therefore, $M_1$ is invertible because its determinant is nonzero. $M_2$ is not invertible because its determinant is zero.