# Exercise 7 — Using Determinant Properties

## 1. Problem Statement

Suppose \(A\) is a \(3\times3\) matrix and \(\det A=-4\). Compute
\(\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).\)
Justify each answer using determinant properties.

## 2. Method and Key Formula

For an \(n\times n\) matrix and scalar \(c\),
\(\det(cA)=c^n\det A.\)
Also,
\(\det(A^T)=\det A,\qquad \det(AB)=\det A\det B.\)
Since \(A\) is \(3\times3\), the scalar factor is raised to the third power.

## 3. Detailed Step-by-Step Solution

**First, \(\det(2A)\):**
\(\det(2A)=2^3\det A=8(-4)=-32.\)

**Second, \(\det(A^T)\):** Transposition does not change the determinant:
\(\det(A^T)=\det A=-4.\)

**Third, \(\det(A^2)\):** Since \(A^2=AA\), use the product property:
\(\det(A^2)=\det(AA)=\det A\cdot\det A=(-4)(-4)=16.\)

**Fourth, \(\det(-A)\):** Here the scalar is \(-1\), and the matrix has order 3:
\(\det(-A)=(-1)^3\det A=(-1)(-4)=4.\)

## 4. Verification and Consistency Checks

Both scalar-multiple results use the dimension \(3\times3\); using \(2\det A\) instead of \(2^3\det A\) would be incorrect. Also, the square of a determinant is nonnegative here: \(\det(A^2)=(-4)^2=16\).

## 5. Final Answer

\[
\boxed{\det(2A)=-32,\quad \det(A^T)=-4,\quad
\det(A^2)=16,\quad \det(-A)=4}
\]