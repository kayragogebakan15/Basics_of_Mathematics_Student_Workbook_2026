# Exercise 2 — Determinant of a 3×3 Matrix

## 1. Problem Statement

For
$$
A=\begin{pmatrix}1&2&-1\\0&3&4\\2&1&5\end{pmatrix},
$$
compute $\det A$ using Sarrus' rule. Then check the result using one determinant property.

## 2. Method and Key Formula

For a $3\times3$ matrix, Sarrus' rule adds the products along the three downward diagonals and subtracts the products along the three upward diagonals. This rule applies to $3\times3$ determinants.

## 3. Detailed Step-by-Step Solution

Write the entries as
$$
A=\begin{pmatrix}a&b&c\\d&e&f\\g&h&i\end{pmatrix}.
$$
Sarrus' rule gives
$\det A=aei+bfg+cdh-ceg-bdi-afh.$
For the given matrix, the downward-diagonal products are
$$
1\cdot3\cdot5=15,\qquad
2\cdot4\cdot2=16,\qquad
(-1)\cdot0\cdot1=0.
$$
Their sum is $15+16+0=31$.

The upward-diagonal products are
$$
(-1)\cdot3\cdot2=-6,\qquad
1\cdot4\cdot1=4,\qquad
2\cdot0\cdot5=0.
$$
Their sum is $-6+4+0=-2$. Therefore,
$\det A=31-(-2)=33.$

## 4. Verification and Consistency Checks

Check by cofactor expansion along the first row:
$$
\begin{aligned}
\det A\\
&=1\begin{vmatrix}3&4\\
1&5\end{vmatrix}
-2\begin{vmatrix}0&4\\
2&5\end{vmatrix}
+(-1)\begin{vmatrix}0&3\\
2&1\end{vmatrix}\\
&=1(3\cdot5-4\cdot1)-2(0\cdot5-4\cdot2)
+(-1)(0\cdot1-3\cdot2)\\
&=1(11)-2(-8)+(-1)(-6)\\
&=11+16+6\\
&=33.
\end{aligned}
$$
This independent calculation agrees with Sarrus' rule.

## 5. Final Answer

$\boxed{\det A=33}$