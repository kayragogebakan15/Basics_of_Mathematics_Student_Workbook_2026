# Exercise 2 — Gaussian Elimination: One Solution

## 1. Problem Statement
Solve using Gaussian elimination:
$$\begin{cases}x+y+z=6,\\2x-y+z=3,\\x+2y-z=2.\end{cases}$$
After solving, substitute the result into all equations and check consistency.

## 2. Method and Key Formula
Write the augmented matrix $[A\mid b]$ and use elementary row operations to reach row echelon form. Then use back-substitution to find the unknowns. Row operations preserve the solution set.

## 3. Detailed Step-by-Step Solution
The augmented matrix is
$$\left[\begin{array}{ccc|c}1&1&1&6\\2&-1&1&3\\1&2&-1&2\end{array}\right].$$
Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:
$$\left[\begin{array}{ccc|c}1&1&1&6\\0&-3&-1&-9\\0&1&-2&-4\end{array}\right].$$
Swap rows 2 and 3, then eliminate the entry below the second pivot using $R_3\leftarrow R_3+3R_2$:
$$\left[\begin{array}{ccc|c}1&1&1&6\\0&1&-2&-4\\0&0&-7&-21\end{array}\right].$$
The third row gives $-7z=-21$, so $z=3$. The second row gives $y-2(3)=-4$, hence $y=2$. The first row gives $x+2+3=6$, hence $x=1$.

## 4. Verification and Consistency Checks
Substitute $(x,y,z)=(1,2,3)$:
- First equation: $1+2+3=6$.
- Second equation: $2(1)-2+3=3$.
- Third equation: $1+2(2)-3=2$.
All three equations hold, so the system is consistent.

## 5. Final Answer
$$\boxed{(x,y,z)=(1,2,3).}$$