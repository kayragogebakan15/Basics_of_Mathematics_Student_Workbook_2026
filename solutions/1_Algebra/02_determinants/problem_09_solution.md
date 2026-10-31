# Exercise 9 — Area and the Determinant

## 1. Problem Statement

The vectors
$$
u=\begin{pmatrix}3\\1\end{pmatrix},\qquad
v=\begin{pmatrix}1\\4\end{pmatrix}
$$
span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## 2. Method and Key Formula

Place the two vectors as columns of a $2\times2$ matrix. The absolute value of its determinant equals the area of the parallelogram:
$$
\text{Area}=|\det[u\ v]|.
$$
The determinant changes sign when two columns are swapped, but its absolute value remains unchanged.

## 3. Detailed Step-by-Step Solution

Place $u$ and $v$ in the columns:
$$
M=[u\ v]=\begin{pmatrix}3&1\\1&4\end{pmatrix}.
$$
Calculate:
$$
\begin{aligned}
\det M&=3\cdot4-1\cdot1\\
&=12-1\\
&=11.
\end{aligned}
$$
Therefore, the area is
$$
\text{Area}=|\det M|=|11|=11.
$$

Now reverse the columns:
$$
N=[v\ u]=\begin{pmatrix}1&3\\4&1\end{pmatrix}.
$$
Then
$$
\begin{aligned}
\det N&=1\cdot1-3\cdot4\\
&=1-12\\
&=-11.
\end{aligned}
$$
The new determinant is the negative of the original determinant, because the two columns have been swapped. However,
$$
\text{Area}=|\det N|=|-11|=11.
$$

## 4. Verification and Consistency Checks

Both column orders give an absolute determinant of 11. The sign describes orientation; area is nonnegative and uses the absolute value.

## 5. Final Answer

$$
\boxed{\text{Area}=11}
$$
Reversing the vectors changes the determinant from $11$ to $-11$, but the parallelogram's area remains $11$.