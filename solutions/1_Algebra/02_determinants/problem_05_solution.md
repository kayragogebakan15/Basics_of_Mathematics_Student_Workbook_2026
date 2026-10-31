# Exercise 5 — Row Operations and Determinants

## 1. Problem Statement

For
$
A=\begin{pmatrix}1&2&3\\2&1&0\\-1&4&2\end{pmatrix},
$
find $\det A$ by simplifying the matrix with row operations. At each step, state whether and how the determinant changes.

## 2. Method and Key Formula

Three row-operation rules are important:
1. Adding a multiple of one row to another row does **not** change the determinant.
2. Swapping two rows changes the sign of the determinant.
3. Multiplying one row by a scalar $c$ multiplies the determinant by $c$.

We will use only row replacements, so the determinant will remain unchanged at every step.

## 3. Detailed Step-by-Step Solution

Start with
$
A=\begin{pmatrix}1&2&3\\2&1&0\\-1&4&2\end{pmatrix}.
$

**Step 1:** Apply $R_2\leftarrow R_2-2R_1$. This is a row replacement, so the determinant does not change:
$
A_1=\begin{pmatrix}1&2&3\\0&-3&-6\\-1&4&2\end{pmatrix},
\qquad \det A_1=\det A.
$

**Step 2:** Apply $R_3\leftarrow R_3+R_1$. This is also a row replacement:
$
A_2=\begin{pmatrix}1&2&3\\0&-3&-6\\0&6&5\end{pmatrix},
\qquad \det A_2=\det A_1.
$

**Step 3:** Apply $R_3\leftarrow R_3+2R_2$, eliminating the second entry of row 3:
$
A_3=\begin{pmatrix}1&2&3\\0&-3&-6\\0&0&-7\end{pmatrix},
\qquad \det A_3=\det A_2.
$
Again, the determinant is unchanged.

The final matrix is upper triangular, so its determinant is the product of its diagonal entries:
$
\det A_3=1\cdot(-3)\cdot(-7)=21.
$

## 4. Verification and Consistency Checks

Every operation was a row replacement, so
$
\det A=\det A_1=\det A_2=\det A_3.
$
The triangular-matrix rule therefore gives $\det A=21$. As a direct check, expansion along the first row gives
$\det A
=1(1\cdot2-0\cdot4)-2(2\cdot2-0\cdot(-1))
+3(2\cdot4-1\cdot(-1))$  
$=2-8+27=21.$

## 5. Final Answer

$
\boxed{\det A=21}
$