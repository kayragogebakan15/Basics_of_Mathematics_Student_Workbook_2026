# Exercise 12 — A Parameter Revealed by a Row Operation

## 1. Problem Statement

For
$$
A(t)=\begin{pmatrix}1&2&3\\2&4&t\\0&1&1\end{pmatrix},
$$
find the values of $t$ for which the matrix is not invertible. First perform
$$
R_2\leftarrow R_2-2R_1,
$$
then use the resulting structure. Explain what happens to the rows for the exceptional value.

## 2. Method and Key Formula

A row replacement does not change the determinant. A square matrix is not invertible exactly when its determinant is zero. After the requested operation, expand along a row or column with zeros to simplify the calculation.

## 3. Detailed Step-by-Step Solution

Apply $R_2\leftarrow R_2-2R_1$:
$$
(2,4,t)-2(1,2,3)=(0,0,t-6).
$$
The resulting matrix is
$$
A_1(t)=\begin{pmatrix}1&2&3\\0&0&t-6\\0&1&1\end{pmatrix},
\qquad \det A_1(t)=\det A(t).
$$

Expand along the second row, which has two zeros. The only nonzero possible term is the entry $t-6$ in position $(2,3)$:
$$
\begin{aligned}
\det A(t)
&=\det A_1(t)\\
&=(t-6)(-1)^{2+3}
\begin{vmatrix}1&2\\0&1\end{vmatrix}\\
&=-(t-6)(1\cdot1-2\cdot0)\\
&=-(t-6)\\
&=6-t.
\end{aligned}
$$
The matrix is not invertible when
$$
6-t=0\quad\Longrightarrow\quad t=6.
$$

For $t=6$, the transformed second row is $(0,0,0)$. This means the transformed rows are linearly dependent, which explains why the determinant is zero.

## 4. Verification and Consistency Checks

A direct cofactor expansion along the first row of the original matrix gives
$$
\det A(t)=1(4-t)-2(2)+3(2)=4-t-4+6=6-t,
$$
which agrees with the row-operation result. At $t=6$, the determinant is $0$.

## 5. Final Answer

$$
\boxed{t=6}
$$
At this value, the second row becomes a zero row after the prescribed row replacement, so the matrix is singular.