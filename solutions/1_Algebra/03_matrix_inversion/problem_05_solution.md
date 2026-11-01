# Exercise 5 — Inverse of a 3×3 Matrix

## 1. Problem Statement
Use Gauss–Jordan elimination to find the inverse of
$$A=\begin{pmatrix}1&1&0\\0&1&1\\1&0&1\end{pmatrix}.$$
Check the result by multiplication.

## 2. Method and Key Formula
Apply elementary row operations to $[A\mid I_3]$ until the left block becomes $I_3$. The right block will then be $A^{-1}$. Every row operation must be applied to the entire augmented matrix.

## 3. Detailed Step-by-Step Solution
Start with
$$
\left[\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
1&0&1&0&0&1
\end{array}\right].
$$
First use $R_3\leftarrow R_3-R_1$:
$$
\left[\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&-1&1&-1&0&1
\end{array}\right].
$$
Next use $R_3\leftarrow R_3+R_2$:
$$
\left[\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&2&-1&1&1
\end{array}\right].
$$
Scale the third row: $R_3\leftarrow\frac12R_3$:
$$
\left[\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}\right].
$$
Eliminate above the third pivot with $R_2\leftarrow R_2-R_3$:
$$
\left[\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}\right].
$$
Finally use $R_1\leftarrow R_1-R_2$:
$$
\left[\begin{array}{ccc|ccc}
1&0&0&\frac12&-\frac12&\frac12\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}\right].
$$
The right block is the inverse.

## 4. Verification and Consistency Checks
Let
$M=\begin{pmatrix}1&-1&1\\1&1&-1\\-1&1&1\end{pmatrix}.$
Use the row-by-column rule to calculate $AM$:
$
\begin{aligned}
\text{Row 1: }&(1\cdot1+1\cdot1+0\cdot(-1),\;1\cdot(-1)+1\cdot1+0\cdot1,\;1\cdot1+1\cdot(-1)+0\cdot1)=(2,0,0),\\
\text{Row 2: }&(0\cdot1+1\cdot1+1\cdot(-1),\;0\cdot(-1)+1\cdot1+1\cdot1,\;0\cdot1+1\cdot(-1)+1\cdot1)=(0,2,0),\\
\text{Row 3: }&(1\cdot1+0\cdot1+1\cdot(-1),\;1\cdot(-1)+0\cdot1+1\cdot1,\;1\cdot1+0\cdot(-1)+1\cdot1)=(0,0,2).
\end{aligned}
$
Thus
$AM=\begin{pmatrix}2&0&0\\0&2&0\\0&0&2\end{pmatrix}=2I_3.$
Since $A^{-1}=\frac12M$, it follows that $AA^{-1}=A(\frac12M)=I_3$. This verifies all nine entries explicitly.

## 5. Final Answer
$$\boxed{A^{-1}=\frac12\begin{pmatrix}1&-1&1\\1&1&-1\\-1&1&1\end{pmatrix}.}$$