# Exercise 4 — Infinitely Many Solutions

## 1. Problem Statement
Solve
$$\begin{cases}x+y+z=2,\\2x+2y+2z=4,\\x-y+z=0.\end{cases}$$
Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point satisfies the system.

## 2. Method and Key Formula
Use elimination to identify dependent equations and free variables. A variable without a pivot is free and may be assigned a parameter. Substitute that parameter into the remaining equations.

## 3. Detailed Step-by-Step Solution
The augmented matrix is
$$\left[\begin{array}{ccc|c}1&1&1&2\\2&2&2&4\\1&-1&1&0\end{array}\right].$$
Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:
$$\left[\begin{array}{ccc|c}1&1&1&2\\0&0&0&0\\0&-2&0&-2\end{array}\right].$$
Swap rows 2 and 3 and divide the new second row by $-2$:
$$\left[\begin{array}{ccc|c}1&1&1&2\\0&1&0&1\\0&0&0&0\end{array}\right].$$
The second row gives $y=1$. The first row gives $x+z=1$. Let the free variable be $z=t$. Then $x=1-t$ and
$$
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb R.
$$

## 4. Verification and Consistency Checks
Choose $t=0$. Then $(x,y,z)=(1,1,0)$. Substitution gives $1+1+0=2$, $2+2+0=4$, and $1-1+0=0$. All equations hold. The second original equation is exactly twice the first, so it adds no new restriction.

## 5. Final Answer
$$\boxed{(x,y,z)=(1-t,1,t),\quad t\in\mathbb R.}$$