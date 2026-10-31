# Exercise 4 — Determinant of a Triangular Matrix

## 1. Problem Statement

Without expanding the determinant, compute
$$
\det\begin{pmatrix}2&4&1\\0&-3&5\\0&0&7\end{pmatrix}.
$$
State the rule for an arbitrary triangular matrix and explain it using this example.

## 2. Method and Key Formula

For any upper- or lower-triangular square matrix, the determinant equals the product of the entries on the main diagonal. A triangular matrix has all entries either above or below the main diagonal equal to zero.

## 3. Detailed Step-by-Step Solution

The matrix is upper triangular because every entry below the main diagonal is zero. Its diagonal entries are $2$, $-3$, and $7$. Therefore,
$$
\begin{aligned}
\det A&=2\cdot(-3)\cdot7\\
&=(-6)\cdot7\\
&=-42.
\end{aligned}
$$

For an $n\times n$ triangular matrix $T=(t_{ij})$, the general rule is
$$
\det T=\prod_{i=1}^{n}t_{ii}=t_{11}t_{22}\cdots t_{nn}.
$$
The zero entries on one side of the diagonal make all terms in the determinant expansion vanish except the product of the diagonal entries.

## 4. Verification and Consistency Checks

The sign is negative because exactly one diagonal factor, $-3$, is negative, while the other factors are positive. The product's magnitude is $2\cdot3\cdot7=42$.

## 5. Final Answer

$$
\boxed{\det A=-42}
$$