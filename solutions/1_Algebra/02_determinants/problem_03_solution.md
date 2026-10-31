# Exercise 3 — Swapping Two Rows

## 1. Problem Statement

For
$$
A=\begin{pmatrix}1&2&0\\0&3&1\\2&1&1\end{pmatrix},
$$
compute $\det A$. Form $B$ by swapping the first and second rows of $A$. Predict $\det B$ using a determinant property, then verify it by calculation.

## 2. Method and Key Formula

Swapping two rows of a matrix changes the sign of its determinant:
$$
\det B=-\det A.
$$
For a $3\times3$ matrix, we can calculate the determinant by cofactor expansion along a row.

## 3. Detailed Step-by-Step Solution

Expand $\det A$ along its first row:
$$
\begin{aligned}
\det A
&=1\begin{vmatrix}3&1\\1&1\end{vmatrix}
-2\begin{vmatrix}0&1\\2&1\end{vmatrix}
+0\begin{vmatrix}0&3\\2&1\end{vmatrix}\\
&=1(3\cdot1-1\cdot1)-2(0\cdot1-1\cdot2)+0\\
&=1(2)-2(-2)\\
&=2+4\\
&=6.
\end{aligned}
$$

Swap the first and second rows:
$$
B=\begin{pmatrix}0&3&1\\1&2&0\\2&1&1\end{pmatrix}.
$$
The row-swap property predicts
$$
\det B=-\det A=-6.
$$

Verify this by expanding along the first row of $B$:
$$
\begin{aligned}
\det B
&=0\begin{vmatrix}2&0\\1&1\end{vmatrix}
-3\begin{vmatrix}1&0\\2&1\end{vmatrix}
+1\begin{vmatrix}1&2\\2&1\end{vmatrix}\\
&=0-3(1\cdot1-0\cdot2)+(1\cdot1-2\cdot2)\\
&=-3+(1-4)\\
&=-3-3\\
&=-6.
\end{aligned}
$$

## 4. Verification and Consistency Checks

The direct calculation gives $\det B=-6$, exactly as predicted by $\det B=-\det A$. The magnitude remains 6 while the sign changes.

## 5. Final Answer

$$
\boxed{\det A=6,\qquad \det B=-6}
$$